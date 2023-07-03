# Comparing `tmp/mypy-boto3-inspector2-1.26.37.tar.gz` & `tmp/mypy-boto3-inspector2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector2-1.26.37.tar", last modified: Fri Dec 23 20:32:30 2022, max compression
+gzip compressed data, was "mypy-boto3-inspector2-1.27.0.tar", last modified: Mon Jul  3 19:50:52 2023, max compression
```

## Comparing `mypy-boto3-inspector2-1.26.37.tar` & `mypy-boto3-inspector2-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.596941 mypy-boto3-inspector2-1.26.37/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2022-12-23 20:32:30.584941 mypy-boto3-inspector2-1.26.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19539 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.580941 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27094 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27046 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16050 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16048 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56438 2022-12-23 20:32:22.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56373 2022-12-23 20:32:20.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.584941 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-23 20:32:30.000000 mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 20:32:30.596941 mypy-boto3-inspector2-1.26.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2022-12-23 20:32:19.000000 mypy-boto3-inspector2-1.26.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.403394 mypy-boto3-inspector2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-03 19:50:52.395394 mypy-boto3-inspector2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21720 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.395394 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35728 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72406 2023-07-03 19:39:14.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72325 2023-07-03 19:39:13.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:12.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.395394 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-03 19:50:52.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:52.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:52.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:52.000000 mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:52.403394 mypy-boto3-inspector2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:39:11.000000 mypy-boto3-inspector2-1.27.0/setup.py
```

### Comparing `mypy-boto3-inspector2-1.26.37/LICENSE` & `mypy-boto3-inspector2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-inspector2-1.26.37/PKG-INFO` & `mypy-boto3-inspector2-1.27.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.26.37
-Summary: Type annotations for boto3.Inspector2 1.26.37 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Inspector2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-inspector2"></a>
 
 # mypy-boto3-inspector2
 
 [![PyPI - mypy-boto3-inspector2](https://img.shields.io/pypi/v/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,14 +288,15 @@
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 
 client: Inspector2Client = Session().client("inspector2")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator(
@@ -311,14 +312,17 @@
 list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
 list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator(
     "list_finding_aggregations"
 )
 list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator(
+    "search_vulnerabilities"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_inspector2.literals` module contains literals extracted from shapes
@@ -329,19 +333,21 @@
     AccountSortByType,
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
+    CodeSnippetErrorCodeType,
     CoverageMapComparisonType,
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     CurrencyType,
     DelegatedAdminStatusType,
+    Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
@@ -373,28 +379,33 @@
     PackageManagerType,
     PackageSortByType,
     PackageTypeType,
     RelationshipStatusType,
     ReportFormatType,
     ReportingErrorCodeType,
     RepositorySortByType,
+    ResourceMapComparisonType,
     ResourceScanTypeType,
+    ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
+    SbomReportFormatType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
+    SearchVulnerabilitiesPaginatorName,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
     StatusType,
     StringComparisonType,
     TitleSortByType,
     UsageTypeType,
+    VulnerabilitySourceType,
     Inspector2ServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -415,68 +426,115 @@
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateMemberResponseTypeDef,
+    AtigDataTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
+    BatchGetCodeSnippetRequestRequestTypeDef,
+    CodeSnippetErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
+    FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    MemberAccountEc2DeepInspectionStatusStateTypeDef,
+    MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportRequestRequestTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CisaDataTypeDef,
+    CodeFilePathTypeDef,
+    CodeLineTypeDef,
+    SuggestedFixTypeDef,
     CountsTypeDef,
+    CoverageDateFilterTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
+    CreateFilterResponseTypeDef,
     DestinationTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    Cvss2TypeDef,
+    Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
+    DeleteFilterResponseTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
+    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
+    EpssDetailsTypeDef,
+    EpssTypeDef,
+    ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyRequestRequestTypeDef,
+    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
+    GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
+    ResetEncryptionKeyRequestRequestTypeDef,
+    ResourceMapFilterTypeDef,
+    ResourceStringFilterTypeDef,
+    ResponseMetadataTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateEncryptionKeyRequestRequestTypeDef,
+    UpdateFilterResponseTypeDef,
+    UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
     ImageLayerAggregationResponseTypeDef,
@@ -491,68 +549,66 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
-    AssociateMemberResponseTypeDef,
-    CancelFindingsReportResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    DeleteFilterResponseTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
-    DisassociateMemberResponseTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
+    CodeVulnerabilityDetailsTypeDef,
+    CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
+    VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaTypeDef,
+    SearchVulnerabilitiesRequestRequestTypeDef,
+    SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
+    BatchGetCodeSnippetResponseTypeDef,
     ListCoverageRequestListCoveragePaginateTypeDef,
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
+    GetSbomExportResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
@@ -576,42 +632,42 @@
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

### Comparing `mypy-boto3-inspector2-1.26.37/README.md` & `mypy-boto3-inspector2-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-inspector2"></a>
 
 # mypy-boto3-inspector2
 
 [![PyPI - mypy-boto3-inspector2](https://img.shields.io/pypi/v/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -256,14 +256,15 @@
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 
 client: Inspector2Client = Session().client("inspector2")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator(
@@ -279,14 +280,17 @@
 list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
 list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator(
     "list_finding_aggregations"
 )
 list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator(
+    "search_vulnerabilities"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_inspector2.literals` module contains literals extracted from shapes
@@ -297,19 +301,21 @@
     AccountSortByType,
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
+    CodeSnippetErrorCodeType,
     CoverageMapComparisonType,
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     CurrencyType,
     DelegatedAdminStatusType,
+    Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
@@ -341,28 +347,33 @@
     PackageManagerType,
     PackageSortByType,
     PackageTypeType,
     RelationshipStatusType,
     ReportFormatType,
     ReportingErrorCodeType,
     RepositorySortByType,
+    ResourceMapComparisonType,
     ResourceScanTypeType,
+    ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
+    SbomReportFormatType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
+    SearchVulnerabilitiesPaginatorName,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
     StatusType,
     StringComparisonType,
     TitleSortByType,
     UsageTypeType,
+    VulnerabilitySourceType,
     Inspector2ServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -383,68 +394,115 @@
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateMemberResponseTypeDef,
+    AtigDataTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
+    BatchGetCodeSnippetRequestRequestTypeDef,
+    CodeSnippetErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
+    FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    MemberAccountEc2DeepInspectionStatusStateTypeDef,
+    MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportRequestRequestTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CisaDataTypeDef,
+    CodeFilePathTypeDef,
+    CodeLineTypeDef,
+    SuggestedFixTypeDef,
     CountsTypeDef,
+    CoverageDateFilterTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
+    CreateFilterResponseTypeDef,
     DestinationTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    Cvss2TypeDef,
+    Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
+    DeleteFilterResponseTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
+    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
+    EpssDetailsTypeDef,
+    EpssTypeDef,
+    ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyRequestRequestTypeDef,
+    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
+    GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
+    ResetEncryptionKeyRequestRequestTypeDef,
+    ResourceMapFilterTypeDef,
+    ResourceStringFilterTypeDef,
+    ResponseMetadataTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateEncryptionKeyRequestRequestTypeDef,
+    UpdateFilterResponseTypeDef,
+    UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
     ImageLayerAggregationResponseTypeDef,
@@ -459,68 +517,66 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
-    AssociateMemberResponseTypeDef,
-    CancelFindingsReportResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    DeleteFilterResponseTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
-    DisassociateMemberResponseTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
+    CodeVulnerabilityDetailsTypeDef,
+    CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
+    VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaTypeDef,
+    SearchVulnerabilitiesRequestRequestTypeDef,
+    SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
+    BatchGetCodeSnippetResponseTypeDef,
     ListCoverageRequestListCoveragePaginateTypeDef,
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
+    GetSbomExportResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
@@ -544,42 +600,42 @@
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

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.py` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,41 +13,44 @@
         ListCoverageStatisticsPaginator,
         ListDelegatedAdminAccountsPaginator,
         ListFiltersPaginator,
         ListFindingAggregationsPaginator,
         ListFindingsPaginator,
         ListMembersPaginator,
         ListUsageTotalsPaginator,
+        SearchVulnerabilitiesPaginator,
     )
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
 
     list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")
     list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_coverage_statistics_paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")
     list_delegated_admin_accounts_paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+    search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
 from .client import Inspector2Client
 from .paginator import (
     ListAccountPermissionsPaginator,
     ListCoveragePaginator,
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 
 Client = Inspector2Client
 
 
 __all__ = (
     "Client",
@@ -57,8 +60,9 @@
     "ListCoverageStatisticsPaginator",
     "ListDelegatedAdminAccountsPaginator",
     "ListFiltersPaginator",
     "ListFindingAggregationsPaginator",
     "ListFindingsPaginator",
     "ListMembersPaginator",
     "ListUsageTotalsPaginator",
+    "SearchVulnerabilitiesPaginator",
 )
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__init__.pyi` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -13,41 +13,44 @@
         ListCoverageStatisticsPaginator,
         ListDelegatedAdminAccountsPaginator,
         ListFiltersPaginator,
         ListFindingAggregationsPaginator,
         ListFindingsPaginator,
         ListMembersPaginator,
         ListUsageTotalsPaginator,
+        SearchVulnerabilitiesPaginator,
     )
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
 
     list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")
     list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_coverage_statistics_paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")
     list_delegated_admin_accounts_paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+    search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
 from .client import Inspector2Client
 from .paginator import (
     ListAccountPermissionsPaginator,
     ListCoveragePaginator,
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 
 Client = Inspector2Client
 
 __all__ = (
     "Client",
     "Inspector2Client",
@@ -56,8 +59,9 @@
     "ListCoverageStatisticsPaginator",
     "ListDelegatedAdminAccountsPaginator",
     "ListFiltersPaginator",
     "ListFindingAggregationsPaginator",
     "ListFindingsPaginator",
     "ListMembersPaginator",
     "ListUsageTotalsPaginator",
+    "SearchVulnerabilitiesPaginator",
 )
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/__main__.py` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector2 1.26.37\nVersion:         1.26.37\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.Inspector2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.37")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.py` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -20,96 +20,109 @@
 
 from .literals import (
     AggregationTypeType,
     FilterActionType,
     GroupKeyType,
     ReportFormatType,
     ResourceScanTypeType,
+    ResourceTypeType,
+    SbomReportFormatType,
+    ScanTypeType,
     ServiceType,
 )
 from .paginator import (
     ListAccountPermissionsPaginator,
     ListCoveragePaginator,
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AutoEnableTypeDef,
     BatchGetAccountStatusResponseTypeDef,
+    BatchGetCodeSnippetResponseTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CreateFilterResponseTypeDef,
     CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
     DeleteFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
     FilterCriteriaTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
+    GetSbomExportResponseTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
+    MemberAccountEc2DeepInspectionStatusTypeDef,
+    ResourceFilterCriteriaTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Inspector2Client",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class Inspector2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/)
     """
 
     meta: ClientMeta
@@ -118,69 +131,99 @@
     def exceptions(self) -> Exceptions:
         """
         Inspector2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#exceptions)
         """
-
     def associate_member(self, *, accountId: str) -> AssociateMemberResponseTypeDef:
         """
         Associates an Amazon Web Services account with an Amazon Inspector delegated
         administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.associate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#associate_member)
         """
-
     def batch_get_account_status(
         self, *, accountIds: Sequence[str] = ...
     ) -> BatchGetAccountStatusResponseTypeDef:
         """
         Retrieves the Amazon Inspector status of multiple Amazon Web Services accounts
         within your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_account_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_account_status)
         """
+    def batch_get_code_snippet(
+        self, *, findingArns: Sequence[str]
+    ) -> BatchGetCodeSnippetResponseTypeDef:
+        """
+        Retrieves code snippets from findings that Amazon Inspector detected code
+        vulnerabilities in.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_code_snippet)
+        """
     def batch_get_free_trial_info(
         self, *, accountIds: Sequence[str]
     ) -> BatchGetFreeTrialInfoResponseTypeDef:
         """
         Gets free trial status for multiple Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_free_trial_info)
         """
+    def batch_get_member_ec2_deep_inspection_status(
+        self, *, accountIds: Sequence[str] = ...
+    ) -> BatchGetMemberEc2DeepInspectionStatusResponseTypeDef:
+        """
+        Retrieves Amazon Inspector deep inspection activation status of multiple member
+        accounts within your organization.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_member_ec2_deep_inspection_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_member_ec2_deep_inspection_status)
+        """
+    def batch_update_member_ec2_deep_inspection_status(
+        self, *, accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef]
+    ) -> BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef:
+        """
+        Activates or deactivates Amazon Inspector deep inspection for the provided
+        member accounts in your organization.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_update_member_ec2_deep_inspection_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_update_member_ec2_deep_inspection_status)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#can_paginate)
         """
-
     def cancel_findings_report(self, *, reportId: str) -> CancelFindingsReportResponseTypeDef:
         """
         Cancels the given findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_findings_report)
         """
+    def cancel_sbom_export(self, *, reportId: str) -> CancelSbomExportResponseTypeDef:
+        """
+        Cancels a software bill of materials (SBOM) report.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_sbom_export)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_sbom_export)
+        """
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
-
     def create_filter(
         self,
         *,
         action: FilterActionType,
         filterCriteria: FilterCriteriaTypeDef,
         name: str,
         description: str = ...,
@@ -189,217 +232,237 @@
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_filter)
         """
-
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
         filterCriteria: FilterCriteriaTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
+    def create_sbom_export(
+        self,
+        *,
+        reportFormat: SbomReportFormatType,
+        s3Destination: DestinationTypeDef,
+        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+    ) -> CreateSbomExportResponseTypeDef:
+        """
+        Creates a software bill of materials (SBOM) report.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
+        """
     def delete_filter(self, *, arn: str) -> DeleteFilterResponseTypeDef:
         """
         Deletes a filter resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.delete_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#delete_filter)
         """
-
     def describe_organization_configuration(
         self,
     ) -> DescribeOrganizationConfigurationResponseTypeDef:
         """
         Describe Amazon Inspector configuration settings for an Amazon Web Services
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.describe_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#describe_organization_configuration)
         """
-
     def disable(
         self,
         *,
         accountIds: Sequence[str] = ...,
         resourceTypes: Sequence[ResourceScanTypeType] = ...
     ) -> DisableResponseTypeDef:
         """
         Disables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable)
         """
-
     def disable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str
     ) -> DisableDelegatedAdminAccountResponseTypeDef:
         """
         Disables the Amazon Inspector delegated administrator for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable_delegated_admin_account)
         """
-
     def disassociate_member(self, *, accountId: str) -> DisassociateMemberResponseTypeDef:
         """
         Disassociates a member account from an Amazon Inspector delegated administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disassociate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disassociate_member)
         """
-
     def enable(
         self,
         *,
         resourceTypes: Sequence[ResourceScanTypeType],
         accountIds: Sequence[str] = ...,
         clientToken: str = ...
     ) -> EnableResponseTypeDef:
         """
         Enables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable)
         """
-
     def enable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str, clientToken: str = ...
     ) -> EnableDelegatedAdminAccountResponseTypeDef:
         """
         Enables the Amazon Inspector delegated administrator for your Organizations
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable_delegated_admin_account)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#generate_presigned_url)
         """
-
     def get_configuration(self) -> GetConfigurationResponseTypeDef:
         """
         Retrieves setting configurations for Inspector scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_configuration)
         """
-
     def get_delegated_admin_account(self) -> GetDelegatedAdminAccountResponseTypeDef:
         """
         Retrieves information about the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_delegated_admin_account)
         """
+    def get_ec2_deep_inspection_configuration(
+        self,
+    ) -> GetEc2DeepInspectionConfigurationResponseTypeDef:
+        """
+        Retrieves the activation status of Amazon Inspector deep inspection and custom
+        paths associated with your account.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_ec2_deep_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_ec2_deep_inspection_configuration)
+        """
+    def get_encryption_key(
+        self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
+    ) -> GetEncryptionKeyResponseTypeDef:
+        """
+        Gets an encryption key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_encryption_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_encryption_key)
+        """
     def get_findings_report_status(
         self, *, reportId: str = ...
     ) -> GetFindingsReportStatusResponseTypeDef:
         """
         Gets the status of a findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_findings_report_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_findings_report_status)
         """
-
     def get_member(self, *, accountId: str) -> GetMemberResponseTypeDef:
         """
         Gets member information for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_member)
         """
+    def get_sbom_export(self, *, reportId: str) -> GetSbomExportResponseTypeDef:
+        """
+        Gets details of a software bill of materials (SBOM) report.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_sbom_export)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_sbom_export)
+        """
     def list_account_permissions(
         self, *, maxResults: int = ..., nextToken: str = ..., service: ServiceType = ...
     ) -> ListAccountPermissionsResponseTypeDef:
         """
         Lists the permissions an account has to configure Amazon Inspector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_account_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_account_permissions)
         """
-
     def list_coverage(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for you environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage)
         """
-
     def list_coverage_statistics(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
         nextToken: str = ...
     ) -> ListCoverageStatisticsResponseTypeDef:
         """
         Lists Amazon Inspector coverage statistics for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage_statistics)
         """
-
     def list_delegated_admin_accounts(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDelegatedAdminAccountsResponseTypeDef:
         """
         Lists information about the Amazon Inspector delegated administrator of your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_delegated_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_delegated_admin_accounts)
         """
-
     def list_filters(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFiltersResponseTypeDef:
         """
         Lists the filters associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_filters)
         """
-
     def list_finding_aggregations(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
         maxResults: int = ...,
@@ -407,83 +470,112 @@
     ) -> ListFindingAggregationsResponseTypeDef:
         """
         Lists aggregated finding data for your environment based on specific criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
-
     def list_findings(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_findings)
         """
-
     def list_members(
         self, *, maxResults: int = ..., nextToken: str = ..., onlyAssociated: bool = ...
     ) -> ListMembersResponseTypeDef:
         """
         List members associated with the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_members)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags attached to a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_tags_for_resource)
         """
-
     def list_usage_totals(
         self, *, accountIds: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListUsageTotalsResponseTypeDef:
         """
         Lists the Amazon Inspector usage totals over the last 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_usage_totals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_usage_totals)
         """
+    def reset_encryption_key(
+        self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
+    ) -> Dict[str, Any]:
+        """
+        Resets an encryption key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.reset_encryption_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#reset_encryption_key)
+        """
+    def search_vulnerabilities(
+        self, *, filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef, nextToken: str = ...
+    ) -> SearchVulnerabilitiesResponseTypeDef:
+        """
+        Lists Amazon Inspector coverage details for a specific vulnerability.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.search_vulnerabilities)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#search_vulnerabilities)
+        """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#untag_resource)
         """
-
     def update_configuration(self, *, ecrConfiguration: EcrConfigurationTypeDef) -> Dict[str, Any]:
         """
         Updates setting configurations for your Amazon Inspector account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_configuration)
         """
+    def update_ec2_deep_inspection_configuration(
+        self, *, activateDeepInspection: bool = ..., packagePaths: Sequence[str] = ...
+    ) -> UpdateEc2DeepInspectionConfigurationResponseTypeDef:
+        """
+        Activates, deactivates Amazon Inspector deep inspection, or updates custom paths
+        for your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_ec2_deep_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_ec2_deep_inspection_configuration)
+        """
+    def update_encryption_key(
+        self, *, kmsKeyId: str, resourceType: ResourceTypeType, scanType: ScanTypeType
+    ) -> Dict[str, Any]:
+        """
+        Updates an encryption key.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_encryption_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_encryption_key)
+        """
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
         filterCriteria: FilterCriteriaTypeDef = ...,
@@ -493,90 +585,97 @@
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_filter)
         """
+    def update_org_ec2_deep_inspection_configuration(
+        self, *, orgPackagePaths: Sequence[str]
+    ) -> Dict[str, Any]:
+        """
+        Updates the Amazon Inspector deep inspection custom paths for your organization.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_org_ec2_deep_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_org_ec2_deep_inspection_configuration)
+        """
     def update_organization_configuration(
         self, *, autoEnable: AutoEnableTypeDef
     ) -> UpdateOrganizationConfigurationResponseTypeDef:
         """
         Updates the configurations for your Amazon Inspector organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_organization_configuration)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_account_permissions"]
     ) -> ListAccountPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_coverage"]) -> ListCoveragePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_coverage_statistics"]
     ) -> ListCoverageStatisticsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_delegated_admin_accounts"]
     ) -> ListDelegatedAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_filters"]) -> ListFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_finding_aggregations"]
     ) -> ListFindingAggregationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_findings"]) -> ListFindingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_members"]) -> ListMembersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_usage_totals"]
     ) -> ListUsageTotalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["search_vulnerabilities"]
+    ) -> SearchVulnerabilitiesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/client.pyi` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,92 +20,113 @@
 
 from .literals import (
     AggregationTypeType,
     FilterActionType,
     GroupKeyType,
     ReportFormatType,
     ResourceScanTypeType,
+    ResourceTypeType,
+    SbomReportFormatType,
+    ScanTypeType,
     ServiceType,
 )
 from .paginator import (
     ListAccountPermissionsPaginator,
     ListCoveragePaginator,
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 from .type_defs import (
     AggregationRequestTypeDef,
     AssociateMemberResponseTypeDef,
     AutoEnableTypeDef,
     BatchGetAccountStatusResponseTypeDef,
+    BatchGetCodeSnippetResponseTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CreateFilterResponseTypeDef,
     CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
     DeleteFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
     FilterCriteriaTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
+    GetSbomExportResponseTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
+    MemberAccountEc2DeepInspectionStatusTypeDef,
+    ResourceFilterCriteriaTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("Inspector2Client",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class Inspector2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/)
     """
 
     meta: ClientMeta
@@ -114,62 +135,110 @@
     def exceptions(self) -> Exceptions:
         """
         Inspector2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#exceptions)
         """
+
     def associate_member(self, *, accountId: str) -> AssociateMemberResponseTypeDef:
         """
         Associates an Amazon Web Services account with an Amazon Inspector delegated
         administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.associate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#associate_member)
         """
+
     def batch_get_account_status(
         self, *, accountIds: Sequence[str] = ...
     ) -> BatchGetAccountStatusResponseTypeDef:
         """
         Retrieves the Amazon Inspector status of multiple Amazon Web Services accounts
         within your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_account_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_account_status)
         """
+
+    def batch_get_code_snippet(
+        self, *, findingArns: Sequence[str]
+    ) -> BatchGetCodeSnippetResponseTypeDef:
+        """
+        Retrieves code snippets from findings that Amazon Inspector detected code
+        vulnerabilities in.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_code_snippet)
+        """
+
     def batch_get_free_trial_info(
         self, *, accountIds: Sequence[str]
     ) -> BatchGetFreeTrialInfoResponseTypeDef:
         """
         Gets free trial status for multiple Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_free_trial_info)
         """
+
+    def batch_get_member_ec2_deep_inspection_status(
+        self, *, accountIds: Sequence[str] = ...
+    ) -> BatchGetMemberEc2DeepInspectionStatusResponseTypeDef:
+        """
+        Retrieves Amazon Inspector deep inspection activation status of multiple member
+        accounts within your organization.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_member_ec2_deep_inspection_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_get_member_ec2_deep_inspection_status)
+        """
+
+    def batch_update_member_ec2_deep_inspection_status(
+        self, *, accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef]
+    ) -> BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef:
+        """
+        Activates or deactivates Amazon Inspector deep inspection for the provided
+        member accounts in your organization.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_update_member_ec2_deep_inspection_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#batch_update_member_ec2_deep_inspection_status)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#can_paginate)
         """
+
     def cancel_findings_report(self, *, reportId: str) -> CancelFindingsReportResponseTypeDef:
         """
         Cancels the given findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_findings_report)
         """
+
+    def cancel_sbom_export(self, *, reportId: str) -> CancelSbomExportResponseTypeDef:
+        """
+        Cancels a software bill of materials (SBOM) report.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_sbom_export)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#cancel_sbom_export)
+        """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#close)
         """
+
     def create_filter(
         self,
         *,
         action: FilterActionType,
         filterCriteria: FilterCriteriaTypeDef,
         name: str,
         description: str = ...,
@@ -178,198 +247,260 @@
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_filter)
         """
+
     def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
         filterCriteria: FilterCriteriaTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_findings_report)
         """
+
+    def create_sbom_export(
+        self,
+        *,
+        reportFormat: SbomReportFormatType,
+        s3Destination: DestinationTypeDef,
+        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+    ) -> CreateSbomExportResponseTypeDef:
+        """
+        Creates a software bill of materials (SBOM) report.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#create_sbom_export)
+        """
+
     def delete_filter(self, *, arn: str) -> DeleteFilterResponseTypeDef:
         """
         Deletes a filter resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.delete_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#delete_filter)
         """
+
     def describe_organization_configuration(
         self,
     ) -> DescribeOrganizationConfigurationResponseTypeDef:
         """
         Describe Amazon Inspector configuration settings for an Amazon Web Services
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.describe_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#describe_organization_configuration)
         """
+
     def disable(
         self,
         *,
         accountIds: Sequence[str] = ...,
         resourceTypes: Sequence[ResourceScanTypeType] = ...
     ) -> DisableResponseTypeDef:
         """
         Disables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable)
         """
+
     def disable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str
     ) -> DisableDelegatedAdminAccountResponseTypeDef:
         """
         Disables the Amazon Inspector delegated administrator for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disable_delegated_admin_account)
         """
+
     def disassociate_member(self, *, accountId: str) -> DisassociateMemberResponseTypeDef:
         """
         Disassociates a member account from an Amazon Inspector delegated administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disassociate_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#disassociate_member)
         """
+
     def enable(
         self,
         *,
         resourceTypes: Sequence[ResourceScanTypeType],
         accountIds: Sequence[str] = ...,
         clientToken: str = ...
     ) -> EnableResponseTypeDef:
         """
         Enables Amazon Inspector scans for one or more Amazon Web Services accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable)
         """
+
     def enable_delegated_admin_account(
         self, *, delegatedAdminAccountId: str, clientToken: str = ...
     ) -> EnableDelegatedAdminAccountResponseTypeDef:
         """
         Enables the Amazon Inspector delegated administrator for your Organizations
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#enable_delegated_admin_account)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#generate_presigned_url)
         """
+
     def get_configuration(self) -> GetConfigurationResponseTypeDef:
         """
         Retrieves setting configurations for Inspector scans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_configuration)
         """
+
     def get_delegated_admin_account(self) -> GetDelegatedAdminAccountResponseTypeDef:
         """
         Retrieves information about the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_delegated_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_delegated_admin_account)
         """
+
+    def get_ec2_deep_inspection_configuration(
+        self,
+    ) -> GetEc2DeepInspectionConfigurationResponseTypeDef:
+        """
+        Retrieves the activation status of Amazon Inspector deep inspection and custom
+        paths associated with your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_ec2_deep_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_ec2_deep_inspection_configuration)
+        """
+
+    def get_encryption_key(
+        self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
+    ) -> GetEncryptionKeyResponseTypeDef:
+        """
+        Gets an encryption key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_encryption_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_encryption_key)
+        """
+
     def get_findings_report_status(
         self, *, reportId: str = ...
     ) -> GetFindingsReportStatusResponseTypeDef:
         """
         Gets the status of a findings report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_findings_report_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_findings_report_status)
         """
+
     def get_member(self, *, accountId: str) -> GetMemberResponseTypeDef:
         """
         Gets member information for your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_member)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_member)
         """
+
+    def get_sbom_export(self, *, reportId: str) -> GetSbomExportResponseTypeDef:
+        """
+        Gets details of a software bill of materials (SBOM) report.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_sbom_export)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_sbom_export)
+        """
+
     def list_account_permissions(
         self, *, maxResults: int = ..., nextToken: str = ..., service: ServiceType = ...
     ) -> ListAccountPermissionsResponseTypeDef:
         """
         Lists the permissions an account has to configure Amazon Inspector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_account_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_account_permissions)
         """
+
     def list_coverage(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListCoverageResponseTypeDef:
         """
         Lists coverage details for you environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage)
         """
+
     def list_coverage_statistics(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
         nextToken: str = ...
     ) -> ListCoverageStatisticsResponseTypeDef:
         """
         Lists Amazon Inspector coverage statistics for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_coverage_statistics)
         """
+
     def list_delegated_admin_accounts(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDelegatedAdminAccountsResponseTypeDef:
         """
         Lists information about the Amazon Inspector delegated administrator of your
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_delegated_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_delegated_admin_accounts)
         """
+
     def list_filters(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFiltersResponseTypeDef:
         """
         Lists the filters associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_filters)
         """
+
     def list_finding_aggregations(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
         maxResults: int = ...,
@@ -377,75 +508,124 @@
     ) -> ListFindingAggregationsResponseTypeDef:
         """
         Lists aggregated finding data for your environment based on specific criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_finding_aggregations)
         """
+
     def list_findings(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_findings)
         """
+
     def list_members(
         self, *, maxResults: int = ..., nextToken: str = ..., onlyAssociated: bool = ...
     ) -> ListMembersResponseTypeDef:
         """
         List members associated with the Amazon Inspector delegated administrator for
         your organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_members)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_members)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags attached to a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_tags_for_resource)
         """
+
     def list_usage_totals(
         self, *, accountIds: Sequence[str] = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListUsageTotalsResponseTypeDef:
         """
         Lists the Amazon Inspector usage totals over the last 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_usage_totals)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#list_usage_totals)
         """
+
+    def reset_encryption_key(
+        self, *, resourceType: ResourceTypeType, scanType: ScanTypeType
+    ) -> Dict[str, Any]:
+        """
+        Resets an encryption key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.reset_encryption_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#reset_encryption_key)
+        """
+
+    def search_vulnerabilities(
+        self, *, filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef, nextToken: str = ...
+    ) -> SearchVulnerabilitiesResponseTypeDef:
+        """
+        Lists Amazon Inspector coverage details for a specific vulnerability.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.search_vulnerabilities)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#search_vulnerabilities)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#untag_resource)
         """
+
     def update_configuration(self, *, ecrConfiguration: EcrConfigurationTypeDef) -> Dict[str, Any]:
         """
         Updates setting configurations for your Amazon Inspector account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_configuration)
         """
+
+    def update_ec2_deep_inspection_configuration(
+        self, *, activateDeepInspection: bool = ..., packagePaths: Sequence[str] = ...
+    ) -> UpdateEc2DeepInspectionConfigurationResponseTypeDef:
+        """
+        Activates, deactivates Amazon Inspector deep inspection, or updates custom paths
+        for your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_ec2_deep_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_ec2_deep_inspection_configuration)
+        """
+
+    def update_encryption_key(
+        self, *, kmsKeyId: str, resourceType: ResourceTypeType, scanType: ScanTypeType
+    ) -> Dict[str, Any]:
+        """
+        Updates an encryption key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_encryption_key)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_encryption_key)
+        """
+
     def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
         filterCriteria: FilterCriteriaTypeDef = ...,
@@ -455,80 +635,109 @@
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_filter)
         """
+
+    def update_org_ec2_deep_inspection_configuration(
+        self, *, orgPackagePaths: Sequence[str]
+    ) -> Dict[str, Any]:
+        """
+        Updates the Amazon Inspector deep inspection custom paths for your organization.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_org_ec2_deep_inspection_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_org_ec2_deep_inspection_configuration)
+        """
+
     def update_organization_configuration(
         self, *, autoEnable: AutoEnableTypeDef
     ) -> UpdateOrganizationConfigurationResponseTypeDef:
         """
         Updates the configurations for your Amazon Inspector organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#update_organization_configuration)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_account_permissions"]
     ) -> ListAccountPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_coverage"]) -> ListCoveragePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_coverage_statistics"]
     ) -> ListCoverageStatisticsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_delegated_admin_accounts"]
     ) -> ListDelegatedAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_filters"]) -> ListFiltersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_finding_aggregations"]
     ) -> ListFindingAggregationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_findings"]) -> ListFindingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_members"]) -> ListMembersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_usage_totals"]
     ) -> ListUsageTotalsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["search_vulnerabilities"]
+    ) -> SearchVulnerabilitiesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.py` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,21 @@
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
     "AwsEcrContainerSortByType",
+    "CodeSnippetErrorCodeType",
     "CoverageMapComparisonType",
     "CoverageResourceTypeType",
     "CoverageStringComparisonType",
     "CurrencyType",
     "DelegatedAdminStatusType",
+    "Ec2DeepInspectionStatusType",
     "Ec2InstanceSortByType",
     "Ec2PlatformType",
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
@@ -67,38 +69,45 @@
     "PackageManagerType",
     "PackageSortByType",
     "PackageTypeType",
     "RelationshipStatusType",
     "ReportFormatType",
     "ReportingErrorCodeType",
     "RepositorySortByType",
+    "ResourceMapComparisonType",
     "ResourceScanTypeType",
+    "ResourceStringComparisonType",
     "ResourceTypeType",
     "RuntimeType",
+    "SbomReportFormatType",
     "ScanStatusCodeType",
     "ScanStatusReasonType",
     "ScanTypeType",
+    "SearchVulnerabilitiesPaginatorName",
     "ServiceType",
     "SeverityType",
     "SortFieldType",
     "SortOrderType",
     "StatusType",
     "StringComparisonType",
     "TitleSortByType",
     "UsageTypeType",
+    "VulnerabilitySourceType",
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
-AggregationFindingTypeType = Literal["NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
+AggregationFindingTypeType = Literal[
+    "CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"
+]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
 AggregationTypeType = Literal[
     "ACCOUNT",
     "AMI",
     "AWS_EC2_INSTANCE",
@@ -110,21 +119,25 @@
     "PACKAGE",
     "REPOSITORY",
     "TITLE",
 ]
 AmiSortByType = Literal["AFFECTED_INSTANCES", "ALL", "CRITICAL", "HIGH"]
 ArchitectureType = Literal["ARM64", "X86_64"]
 AwsEcrContainerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
+CodeSnippetErrorCodeType = Literal[
+    "ACCESS_DENIED", "CODE_SNIPPET_NOT_FOUND", "INTERNAL_ERROR", "INVALID_INPUT"
+]
 CoverageMapComparisonType = Literal["EQUALS"]
 CoverageResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_ECR_REPOSITORY", "AWS_LAMBDA_FUNCTION"
 ]
 CoverageStringComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 CurrencyType = Literal["USD"]
 DelegatedAdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
+Ec2DeepInspectionStatusType = Literal["ACTIVATED", "DEACTIVATED", "FAILED", "PENDING"]
 Ec2InstanceSortByType = Literal["ALL", "CRITICAL", "HIGH", "NETWORK_FINDINGS"]
 Ec2PlatformType = Literal["LINUX", "UNKNOWN", "WINDOWS"]
 EcrRescanDurationStatusType = Literal["FAILED", "PENDING", "SUCCESS"]
 EcrRescanDurationType = Literal["DAYS_180", "DAYS_30", "LIFETIME"]
 EcrScanFrequencyType = Literal["CONTINUOUS_SCAN", "MANUAL", "SCAN_ON_PUSH"]
 ErrorCodeType = Literal[
     "ACCESS_DENIED",
@@ -143,19 +156,19 @@
     "SUSPEND_IN_PROGRESS",
 ]
 ExploitAvailableType = Literal["NO", "YES"]
 ExternalReportStatusType = Literal["CANCELLED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 FilterActionType = Literal["NONE", "SUPPRESS"]
 FindingStatusType = Literal["ACTIVE", "CLOSED", "SUPPRESSED"]
 FindingTypeSortByType = Literal["ALL", "CRITICAL", "HIGH"]
-FindingTypeType = Literal["NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
+FindingTypeType = Literal["CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 FixAvailableType = Literal["NO", "PARTIAL", "YES"]
 FreeTrialInfoErrorCodeType = Literal["ACCESS_DENIED", "INTERNAL_ERROR"]
 FreeTrialStatusType = Literal["ACTIVE", "INACTIVE"]
-FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA"]
+FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
 GroupKeyType = Literal[
     "ACCOUNT_ID", "ECR_REPOSITORY_NAME", "RESOURCE_TYPE", "SCAN_STATUS_CODE", "SCAN_STATUS_REASON"
 ]
 ImageLayerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 LambdaFunctionSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 LambdaLayerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 ListAccountPermissionsPaginatorName = Literal["list_account_permissions"]
@@ -172,14 +185,15 @@
 OperationType = Literal[
     "DISABLE_REPOSITORY", "DISABLE_SCANNING", "ENABLE_REPOSITORY", "ENABLE_SCANNING"
 ]
 PackageManagerType = Literal[
     "BUNDLER",
     "CARGO",
     "COMPOSER",
+    "GEMSPEC",
     "GOBINARY",
     "GOMOD",
     "JAR",
     "NODEPKG",
     "NPM",
     "NUGET",
     "OS",
@@ -212,36 +226,45 @@
     "INCOMPATIBLE_BUCKET_REGION",
     "INTERNAL_ERROR",
     "INVALID_PERMISSIONS",
     "MALFORMED_KMS_KEY",
     "NO_FINDINGS_FOUND",
 ]
 RepositorySortByType = Literal["AFFECTED_IMAGES", "ALL", "CRITICAL", "HIGH"]
-ResourceScanTypeType = Literal["EC2", "ECR", "LAMBDA"]
+ResourceMapComparisonType = Literal["EQUALS"]
+ResourceScanTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
+ResourceStringComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 ResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_ECR_REPOSITORY", "AWS_LAMBDA_FUNCTION"
 ]
 RuntimeType = Literal[
     "GO_1_X",
     "JAVA_11",
+    "JAVA_17",
     "JAVA_8",
     "JAVA_8_AL2",
     "NODEJS",
     "NODEJS_12_X",
     "NODEJS_14_X",
     "NODEJS_16_X",
     "NODEJS_18_X",
+    "PYTHON_3_10",
     "PYTHON_3_7",
     "PYTHON_3_8",
     "PYTHON_3_9",
     "UNSUPPORTED",
 ]
+SbomReportFormatType = Literal["CYCLONEDX_1_4", "SPDX_2_3"]
 ScanStatusCodeType = Literal["ACTIVE", "INACTIVE"]
 ScanStatusReasonType = Literal[
     "ACCESS_DENIED",
+    "DEEP_INSPECTION_COLLECTION_TIME_LIMIT_EXCEEDED",
+    "DEEP_INSPECTION_DAILY_SSM_INVENTORY_LIMIT_EXCEEDED",
+    "DEEP_INSPECTION_NO_INVENTORY",
+    "DEEP_INSPECTION_PACKAGE_COLLECTION_LIMIT_EXCEEDED",
     "EC2_INSTANCE_STOPPED",
     "EXCLUDED_BY_TAG",
     "IMAGE_SIZE_EXCEEDED",
     "INTERNAL_ERROR",
     "NO_INVENTORY",
     "NO_RESOURCES_FOUND",
     "PENDING_DISABLE",
@@ -249,26 +272,30 @@
     "RESOURCE_TERMINATED",
     "SCAN_ELIGIBILITY_EXPIRED",
     "SCAN_FREQUENCY_MANUAL",
     "SCAN_FREQUENCY_SCAN_ON_PUSH",
     "STALE_INVENTORY",
     "SUCCESSFUL",
     "UNMANAGED_EC2_INSTANCE",
+    "UNSUPPORTED_CONFIG_FILE",
+    "UNSUPPORTED_MEDIA_TYPE",
     "UNSUPPORTED_OS",
     "UNSUPPORTED_RUNTIME",
 ]
-ScanTypeType = Literal["NETWORK", "PACKAGE"]
+ScanTypeType = Literal["CODE", "NETWORK", "PACKAGE"]
+SearchVulnerabilitiesPaginatorName = Literal["search_vulnerabilities"]
 ServiceType = Literal["EC2", "ECR", "LAMBDA"]
 SeverityType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM", "UNTRIAGED"]
 SortFieldType = Literal[
     "AWS_ACCOUNT_ID",
     "COMPONENT_TYPE",
     "ECR_IMAGE_PUSHED_AT",
     "ECR_IMAGE_REGISTRY",
     "ECR_IMAGE_REPOSITORY_NAME",
+    "EPSS_SCORE",
     "FINDING_STATUS",
     "FINDING_TYPE",
     "FIRST_OBSERVED_AT",
     "INSPECTOR_SCORE",
     "LAST_OBSERVED_AT",
     "NETWORK_PROTOCOL",
     "RESOURCE_TYPE",
@@ -278,16 +305,21 @@
     "VULNERABILITY_SOURCE",
 ]
 SortOrderType = Literal["ASC", "DESC"]
 StatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING", "SUSPENDED", "SUSPENDING"]
 StringComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX"]
 TitleSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 UsageTypeType = Literal[
-    "EC2_INSTANCE_HOURS", "ECR_INITIAL_SCAN", "ECR_RESCAN", "LAMBDA_FUNCTION_HOURS"
+    "EC2_INSTANCE_HOURS",
+    "ECR_INITIAL_SCAN",
+    "ECR_RESCAN",
+    "LAMBDA_FUNCTION_CODE_HOURS",
+    "LAMBDA_FUNCTION_HOURS",
 ]
+VulnerabilitySourceType = Literal["NVD"]
 Inspector2ServiceName = Literal["inspector2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -296,14 +328,15 @@
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
@@ -324,31 +357,34 @@
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
@@ -427,14 +463,15 @@
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
@@ -445,18 +482,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -487,14 +526,15 @@
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
@@ -513,16 +553,19 @@
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
@@ -602,18 +645,21 @@
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
@@ -641,14 +687,15 @@
     "list_coverage_statistics",
     "list_delegated_admin_accounts",
     "list_filters",
     "list_finding_aggregations",
     "list_findings",
     "list_members",
     "list_usage_totals",
+    "search_vulnerabilities",
 ]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/literals.pyi` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,21 @@
     "AccountSortByType",
     "AggregationFindingTypeType",
     "AggregationResourceTypeType",
     "AggregationTypeType",
     "AmiSortByType",
     "ArchitectureType",
     "AwsEcrContainerSortByType",
+    "CodeSnippetErrorCodeType",
     "CoverageMapComparisonType",
     "CoverageResourceTypeType",
     "CoverageStringComparisonType",
     "CurrencyType",
     "DelegatedAdminStatusType",
+    "Ec2DeepInspectionStatusType",
     "Ec2InstanceSortByType",
     "Ec2PlatformType",
     "EcrRescanDurationStatusType",
     "EcrRescanDurationType",
     "EcrScanFrequencyType",
     "ErrorCodeType",
     "ExploitAvailableType",
@@ -66,37 +68,44 @@
     "PackageManagerType",
     "PackageSortByType",
     "PackageTypeType",
     "RelationshipStatusType",
     "ReportFormatType",
     "ReportingErrorCodeType",
     "RepositorySortByType",
+    "ResourceMapComparisonType",
     "ResourceScanTypeType",
+    "ResourceStringComparisonType",
     "ResourceTypeType",
     "RuntimeType",
+    "SbomReportFormatType",
     "ScanStatusCodeType",
     "ScanStatusReasonType",
     "ScanTypeType",
+    "SearchVulnerabilitiesPaginatorName",
     "ServiceType",
     "SeverityType",
     "SortFieldType",
     "SortOrderType",
     "StatusType",
     "StringComparisonType",
     "TitleSortByType",
     "UsageTypeType",
+    "VulnerabilitySourceType",
     "Inspector2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AccountSortByType = Literal["ALL", "CRITICAL", "HIGH"]
-AggregationFindingTypeType = Literal["NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
+AggregationFindingTypeType = Literal[
+    "CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"
+]
 AggregationResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_LAMBDA_FUNCTION"
 ]
 AggregationTypeType = Literal[
     "ACCOUNT",
     "AMI",
     "AWS_EC2_INSTANCE",
@@ -108,21 +117,25 @@
     "PACKAGE",
     "REPOSITORY",
     "TITLE",
 ]
 AmiSortByType = Literal["AFFECTED_INSTANCES", "ALL", "CRITICAL", "HIGH"]
 ArchitectureType = Literal["ARM64", "X86_64"]
 AwsEcrContainerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
+CodeSnippetErrorCodeType = Literal[
+    "ACCESS_DENIED", "CODE_SNIPPET_NOT_FOUND", "INTERNAL_ERROR", "INVALID_INPUT"
+]
 CoverageMapComparisonType = Literal["EQUALS"]
 CoverageResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_ECR_REPOSITORY", "AWS_LAMBDA_FUNCTION"
 ]
 CoverageStringComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 CurrencyType = Literal["USD"]
 DelegatedAdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
+Ec2DeepInspectionStatusType = Literal["ACTIVATED", "DEACTIVATED", "FAILED", "PENDING"]
 Ec2InstanceSortByType = Literal["ALL", "CRITICAL", "HIGH", "NETWORK_FINDINGS"]
 Ec2PlatformType = Literal["LINUX", "UNKNOWN", "WINDOWS"]
 EcrRescanDurationStatusType = Literal["FAILED", "PENDING", "SUCCESS"]
 EcrRescanDurationType = Literal["DAYS_180", "DAYS_30", "LIFETIME"]
 EcrScanFrequencyType = Literal["CONTINUOUS_SCAN", "MANUAL", "SCAN_ON_PUSH"]
 ErrorCodeType = Literal[
     "ACCESS_DENIED",
@@ -141,19 +154,19 @@
     "SUSPEND_IN_PROGRESS",
 ]
 ExploitAvailableType = Literal["NO", "YES"]
 ExternalReportStatusType = Literal["CANCELLED", "FAILED", "IN_PROGRESS", "SUCCEEDED"]
 FilterActionType = Literal["NONE", "SUPPRESS"]
 FindingStatusType = Literal["ACTIVE", "CLOSED", "SUPPRESSED"]
 FindingTypeSortByType = Literal["ALL", "CRITICAL", "HIGH"]
-FindingTypeType = Literal["NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
+FindingTypeType = Literal["CODE_VULNERABILITY", "NETWORK_REACHABILITY", "PACKAGE_VULNERABILITY"]
 FixAvailableType = Literal["NO", "PARTIAL", "YES"]
 FreeTrialInfoErrorCodeType = Literal["ACCESS_DENIED", "INTERNAL_ERROR"]
 FreeTrialStatusType = Literal["ACTIVE", "INACTIVE"]
-FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA"]
+FreeTrialTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
 GroupKeyType = Literal[
     "ACCOUNT_ID", "ECR_REPOSITORY_NAME", "RESOURCE_TYPE", "SCAN_STATUS_CODE", "SCAN_STATUS_REASON"
 ]
 ImageLayerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 LambdaFunctionSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 LambdaLayerSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 ListAccountPermissionsPaginatorName = Literal["list_account_permissions"]
@@ -170,14 +183,15 @@
 OperationType = Literal[
     "DISABLE_REPOSITORY", "DISABLE_SCANNING", "ENABLE_REPOSITORY", "ENABLE_SCANNING"
 ]
 PackageManagerType = Literal[
     "BUNDLER",
     "CARGO",
     "COMPOSER",
+    "GEMSPEC",
     "GOBINARY",
     "GOMOD",
     "JAR",
     "NODEPKG",
     "NPM",
     "NUGET",
     "OS",
@@ -210,36 +224,45 @@
     "INCOMPATIBLE_BUCKET_REGION",
     "INTERNAL_ERROR",
     "INVALID_PERMISSIONS",
     "MALFORMED_KMS_KEY",
     "NO_FINDINGS_FOUND",
 ]
 RepositorySortByType = Literal["AFFECTED_IMAGES", "ALL", "CRITICAL", "HIGH"]
-ResourceScanTypeType = Literal["EC2", "ECR", "LAMBDA"]
+ResourceMapComparisonType = Literal["EQUALS"]
+ResourceScanTypeType = Literal["EC2", "ECR", "LAMBDA", "LAMBDA_CODE"]
+ResourceStringComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 ResourceTypeType = Literal[
     "AWS_EC2_INSTANCE", "AWS_ECR_CONTAINER_IMAGE", "AWS_ECR_REPOSITORY", "AWS_LAMBDA_FUNCTION"
 ]
 RuntimeType = Literal[
     "GO_1_X",
     "JAVA_11",
+    "JAVA_17",
     "JAVA_8",
     "JAVA_8_AL2",
     "NODEJS",
     "NODEJS_12_X",
     "NODEJS_14_X",
     "NODEJS_16_X",
     "NODEJS_18_X",
+    "PYTHON_3_10",
     "PYTHON_3_7",
     "PYTHON_3_8",
     "PYTHON_3_9",
     "UNSUPPORTED",
 ]
+SbomReportFormatType = Literal["CYCLONEDX_1_4", "SPDX_2_3"]
 ScanStatusCodeType = Literal["ACTIVE", "INACTIVE"]
 ScanStatusReasonType = Literal[
     "ACCESS_DENIED",
+    "DEEP_INSPECTION_COLLECTION_TIME_LIMIT_EXCEEDED",
+    "DEEP_INSPECTION_DAILY_SSM_INVENTORY_LIMIT_EXCEEDED",
+    "DEEP_INSPECTION_NO_INVENTORY",
+    "DEEP_INSPECTION_PACKAGE_COLLECTION_LIMIT_EXCEEDED",
     "EC2_INSTANCE_STOPPED",
     "EXCLUDED_BY_TAG",
     "IMAGE_SIZE_EXCEEDED",
     "INTERNAL_ERROR",
     "NO_INVENTORY",
     "NO_RESOURCES_FOUND",
     "PENDING_DISABLE",
@@ -247,26 +270,30 @@
     "RESOURCE_TERMINATED",
     "SCAN_ELIGIBILITY_EXPIRED",
     "SCAN_FREQUENCY_MANUAL",
     "SCAN_FREQUENCY_SCAN_ON_PUSH",
     "STALE_INVENTORY",
     "SUCCESSFUL",
     "UNMANAGED_EC2_INSTANCE",
+    "UNSUPPORTED_CONFIG_FILE",
+    "UNSUPPORTED_MEDIA_TYPE",
     "UNSUPPORTED_OS",
     "UNSUPPORTED_RUNTIME",
 ]
-ScanTypeType = Literal["NETWORK", "PACKAGE"]
+ScanTypeType = Literal["CODE", "NETWORK", "PACKAGE"]
+SearchVulnerabilitiesPaginatorName = Literal["search_vulnerabilities"]
 ServiceType = Literal["EC2", "ECR", "LAMBDA"]
 SeverityType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM", "UNTRIAGED"]
 SortFieldType = Literal[
     "AWS_ACCOUNT_ID",
     "COMPONENT_TYPE",
     "ECR_IMAGE_PUSHED_AT",
     "ECR_IMAGE_REGISTRY",
     "ECR_IMAGE_REPOSITORY_NAME",
+    "EPSS_SCORE",
     "FINDING_STATUS",
     "FINDING_TYPE",
     "FIRST_OBSERVED_AT",
     "INSPECTOR_SCORE",
     "LAST_OBSERVED_AT",
     "NETWORK_PROTOCOL",
     "RESOURCE_TYPE",
@@ -276,16 +303,21 @@
     "VULNERABILITY_SOURCE",
 ]
 SortOrderType = Literal["ASC", "DESC"]
 StatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING", "SUSPENDED", "SUSPENDING"]
 StringComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX"]
 TitleSortByType = Literal["ALL", "CRITICAL", "HIGH"]
 UsageTypeType = Literal[
-    "EC2_INSTANCE_HOURS", "ECR_INITIAL_SCAN", "ECR_RESCAN", "LAMBDA_FUNCTION_HOURS"
+    "EC2_INSTANCE_HOURS",
+    "ECR_INITIAL_SCAN",
+    "ECR_RESCAN",
+    "LAMBDA_FUNCTION_CODE_HOURS",
+    "LAMBDA_FUNCTION_HOURS",
 ]
+VulnerabilitySourceType = Literal["NVD"]
 Inspector2ServiceName = Literal["inspector2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -294,14 +326,15 @@
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
@@ -322,31 +355,34 @@
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
@@ -425,14 +461,15 @@
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
@@ -443,18 +480,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -485,14 +524,15 @@
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
@@ -511,16 +551,19 @@
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
@@ -600,18 +643,21 @@
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
@@ -639,14 +685,15 @@
     "list_coverage_statistics",
     "list_delegated_admin_accounts",
     "list_filters",
     "list_finding_aggregations",
     "list_findings",
     "list_members",
     "list_usage_totals",
+    "search_vulnerabilities",
 ]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.py` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,30 @@
         ListCoverageStatisticsPaginator,
         ListDelegatedAdminAccountsPaginator,
         ListFiltersPaginator,
         ListFindingAggregationsPaginator,
         ListFindingsPaginator,
         ListMembersPaginator,
         ListUsageTotalsPaginator,
+        SearchVulnerabilitiesPaginator,
     )
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
 
     list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")
     list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_coverage_statistics_paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")
     list_delegated_admin_accounts_paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+    search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
@@ -50,28 +52,31 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     PaginatorConfigTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
 )
 
 __all__ = (
     "ListAccountPermissionsPaginator",
     "ListCoveragePaginator",
     "ListCoverageStatisticsPaginator",
     "ListDelegatedAdminAccountsPaginator",
     "ListFiltersPaginator",
     "ListFindingAggregationsPaginator",
     "ListFindingsPaginator",
     "ListMembersPaginator",
     "ListUsageTotalsPaginator",
+    "SearchVulnerabilitiesPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -84,15 +89,15 @@
 class ListAccountPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
     """
 
     def paginate(
-        self, *, service: ServiceType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, service: ServiceType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
         """
 
 
@@ -102,15 +107,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
         """
 
 
@@ -121,30 +126,30 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 
 class ListDelegatedAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDelegatedAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
         """
 
 
@@ -155,15 +160,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfilterspaginator)
         """
 
 
@@ -175,15 +180,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 
@@ -194,43 +199,61 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
 
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, onlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
         """
 
 
 class ListUsageTotalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsageTotalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
         """
+
+
+class SearchVulnerabilitiesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[SearchVulnerabilitiesResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
+        """
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/paginator.pyi` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,30 @@
         ListCoverageStatisticsPaginator,
         ListDelegatedAdminAccountsPaginator,
         ListFiltersPaginator,
         ListFindingAggregationsPaginator,
         ListFindingsPaginator,
         ListMembersPaginator,
         ListUsageTotalsPaginator,
+        SearchVulnerabilitiesPaginator,
     )
 
     session = Session()
     client: Inspector2Client = session.client("inspector2")
 
     list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")
     list_coverage_paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
     list_coverage_statistics_paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")
     list_delegated_admin_accounts_paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")
     list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
     list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
     list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+    search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
@@ -50,28 +52,31 @@
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     PaginatorConfigTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
 )
 
 __all__ = (
     "ListAccountPermissionsPaginator",
     "ListCoveragePaginator",
     "ListCoverageStatisticsPaginator",
     "ListDelegatedAdminAccountsPaginator",
     "ListFiltersPaginator",
     "ListFindingAggregationsPaginator",
     "ListFindingsPaginator",
     "ListMembersPaginator",
     "ListUsageTotalsPaginator",
+    "SearchVulnerabilitiesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
@@ -81,15 +86,15 @@
 class ListAccountPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
     """
 
     def paginate(
-        self, *, service: ServiceType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, service: ServiceType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listaccountpermissionspaginator)
         """
 
 class ListCoveragePaginator(Paginator):
@@ -98,15 +103,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragepaginator)
         """
 
 class ListCoverageStatisticsPaginator(Paginator):
@@ -116,29 +121,29 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 class ListDelegatedAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDelegatedAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listdelegatedadminaccountspaginator)
         """
 
 class ListFiltersPaginator(Paginator):
@@ -148,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfilterspaginator)
         """
 
 class ListFindingAggregationsPaginator(Paginator):
@@ -167,15 +172,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 class ListFindingsPaginator(Paginator):
@@ -185,41 +190,58 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: FilterCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listfindingspaginator)
         """
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, onlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listmemberspaginator)
         """
 
 class ListUsageTotalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsageTotalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#listusagetotalspaginator)
         """
+
+class SearchVulnerabilitiesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[SearchVulnerabilitiesResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/paginators/#searchvulnerabilitiespaginator)
+        """
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.py` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,19 @@
     AccountSortByType,
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
+    CodeSnippetErrorCodeType,
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     DelegatedAdminStatusType,
+    Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
@@ -52,16 +54,18 @@
     PackageSortByType,
     PackageTypeType,
     RelationshipStatusType,
     ReportFormatType,
     ReportingErrorCodeType,
     RepositorySortByType,
     ResourceScanTypeType,
+    ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
+    SbomReportFormatType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
@@ -85,68 +89,115 @@
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateMemberResponseTypeDef",
+    "AtigDataTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
+    "BatchGetCodeSnippetRequestRequestTypeDef",
+    "CodeSnippetErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
+    "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    "MemberAccountEc2DeepInspectionStatusStateTypeDef",
+    "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
+    "CancelFindingsReportResponseTypeDef",
+    "CancelSbomExportRequestRequestTypeDef",
+    "CancelSbomExportResponseTypeDef",
+    "CisaDataTypeDef",
+    "CodeFilePathTypeDef",
+    "CodeLineTypeDef",
+    "SuggestedFixTypeDef",
     "CountsTypeDef",
+    "CoverageDateFilterTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
+    "CreateFilterResponseTypeDef",
     "DestinationTypeDef",
+    "CreateFindingsReportResponseTypeDef",
+    "CreateSbomExportResponseTypeDef",
+    "Cvss2TypeDef",
+    "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
+    "DeleteFilterResponseTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
+    "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
+    "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
+    "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
+    "EpssDetailsTypeDef",
+    "EpssTypeDef",
+    "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    "GetEncryptionKeyRequestRequestTypeDef",
+    "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
     "GetMemberRequestRequestTypeDef",
     "MemberTypeDef",
+    "GetSbomExportRequestRequestTypeDef",
     "LambdaFunctionMetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
     "ListAccountPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "SortCriteriaTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
+    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
+    "ResetEncryptionKeyRequestRequestTypeDef",
+    "ResourceMapFilterTypeDef",
+    "ResourceStringFilterTypeDef",
+    "ResponseMetadataTypeDef",
+    "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    "UpdateEncryptionKeyRequestRequestTypeDef",
+    "UpdateFilterResponseTypeDef",
+    "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     "UsageTypeDef",
     "AccountAggregationResponseTypeDef",
     "AmiAggregationResponseTypeDef",
     "AwsEcrContainerAggregationResponseTypeDef",
     "Ec2InstanceAggregationResponseTypeDef",
     "FindingTypeAggregationResponseTypeDef",
     "ImageLayerAggregationResponseTypeDef",
@@ -161,68 +212,66 @@
     "AmiAggregationTypeDef",
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
-    "AssociateMemberResponseTypeDef",
-    "CancelFindingsReportResponseTypeDef",
-    "CreateFilterResponseTypeDef",
-    "CreateFindingsReportResponseTypeDef",
-    "DeleteFilterResponseTypeDef",
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    "DisassociateMemberResponseTypeDef",
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateFilterResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateOrganizationConfigurationResponseTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
+    "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
+    "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
+    "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    "CodeVulnerabilityDetailsTypeDef",
+    "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
+    "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaTypeDef",
+    "SearchVulnerabilitiesRequestRequestTypeDef",
+    "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
+    "BatchGetCodeSnippetResponseTypeDef",
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
+    "SearchVulnerabilitiesResponseTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
+    "GetSbomExportResponseTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
@@ -276,14 +325,15 @@
         "ecr": StatusType,
     },
 )
 _OptionalResourceStatusTypeDef = TypedDict(
     "_OptionalResourceStatusTypeDef",
     {
         "lambda": StatusType,
+        "lambdaCode": StatusType,
     },
     total=False,
 )
 
 
 class ResourceStatusTypeDef(_RequiredResourceStatusTypeDef, _OptionalResourceStatusTypeDef):
     pass
@@ -311,36 +361,45 @@
 AssociateMemberRequestRequestTypeDef = TypedDict(
     "AssociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateMemberResponseTypeDef = TypedDict(
+    "AssociateMemberResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AtigDataTypeDef = TypedDict(
+    "AtigDataTypeDef",
+    {
+        "firstSeen": datetime,
+        "lastSeen": datetime,
+        "targets": List[str],
+        "ttps": List[str],
+    },
+    total=False,
+)
+
 _RequiredAutoEnableTypeDef = TypedDict(
     "_RequiredAutoEnableTypeDef",
     {
         "ec2": bool,
         "ecr": bool,
     },
 )
 _OptionalAutoEnableTypeDef = TypedDict(
     "_OptionalAutoEnableTypeDef",
     {
         "lambda": bool,
+        "lambdaCode": bool,
     },
     total=False,
 )
 
 
 class AutoEnableTypeDef(_RequiredAutoEnableTypeDef, _OptionalAutoEnableTypeDef):
     pass
@@ -404,14 +463,30 @@
     "BatchGetAccountStatusRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
+BatchGetCodeSnippetRequestRequestTypeDef = TypedDict(
+    "BatchGetCodeSnippetRequestRequestTypeDef",
+    {
+        "findingArns": Sequence[str],
+    },
+)
+
+CodeSnippetErrorTypeDef = TypedDict(
+    "CodeSnippetErrorTypeDef",
+    {
+        "errorCode": CodeSnippetErrorCodeType,
+        "errorMessage": str,
+        "findingArn": str,
+    },
+)
+
 BatchGetFreeTrialInfoRequestRequestTypeDef = TypedDict(
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 
@@ -420,30 +495,161 @@
     {
         "accountId": str,
         "code": FreeTrialInfoErrorCodeType,
         "message": str,
     },
 )
 
+BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
+    "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    {
+        "accountIds": Sequence[str],
+    },
+    total=False,
+)
+
+_RequiredFailedMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_RequiredFailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalFailedMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_OptionalFailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "ec2ScanStatus": StatusType,
+        "errorMessage": str,
+    },
+    total=False,
+)
+
+
+class FailedMemberAccountEc2DeepInspectionStatusStateTypeDef(
+    _RequiredFailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    _OptionalFailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+):
+    pass
+
+
+_RequiredMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_RequiredMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_OptionalMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "errorMessage": str,
+        "status": Ec2DeepInspectionStatusType,
+    },
+    total=False,
+)
+
+
+class MemberAccountEc2DeepInspectionStatusStateTypeDef(
+    _RequiredMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    _OptionalMemberAccountEc2DeepInspectionStatusStateTypeDef,
+):
+    pass
+
+
+MemberAccountEc2DeepInspectionStatusTypeDef = TypedDict(
+    "MemberAccountEc2DeepInspectionStatusTypeDef",
+    {
+        "accountId": str,
+        "activateDeepInspection": bool,
+    },
+)
+
 CancelFindingsReportRequestRequestTypeDef = TypedDict(
     "CancelFindingsReportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
+CancelFindingsReportResponseTypeDef = TypedDict(
+    "CancelFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CancelSbomExportRequestRequestTypeDef = TypedDict(
+    "CancelSbomExportRequestRequestTypeDef",
+    {
+        "reportId": str,
+    },
+)
+
+CancelSbomExportResponseTypeDef = TypedDict(
+    "CancelSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CisaDataTypeDef = TypedDict(
+    "CisaDataTypeDef",
+    {
+        "action": str,
+        "dateAdded": datetime,
+        "dateDue": datetime,
+    },
+    total=False,
+)
+
+CodeFilePathTypeDef = TypedDict(
+    "CodeFilePathTypeDef",
+    {
+        "endLine": int,
+        "fileName": str,
+        "filePath": str,
+        "startLine": int,
+    },
+)
+
+CodeLineTypeDef = TypedDict(
+    "CodeLineTypeDef",
+    {
+        "content": str,
+        "lineNumber": int,
+    },
+)
+
+SuggestedFixTypeDef = TypedDict(
+    "SuggestedFixTypeDef",
+    {
+        "code": str,
+        "description": str,
+    },
+    total=False,
+)
+
 CountsTypeDef = TypedDict(
     "CountsTypeDef",
     {
         "count": int,
         "groupKey": GroupKeyType,
     },
     total=False,
 )
 
+CoverageDateFilterTypeDef = TypedDict(
+    "CoverageDateFilterTypeDef",
+    {
+        "endInclusive": Union[datetime, str],
+        "startInclusive": Union[datetime, str],
+    },
+    total=False,
+)
+
 _RequiredCoverageMapFilterTypeDef = TypedDict(
     "_RequiredCoverageMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -474,14 +680,22 @@
     "ScanStatusTypeDef",
     {
         "reason": ScanStatusReasonType,
         "statusCode": ScanStatusCodeType,
     },
 )
 
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -494,14 +708,48 @@
 )
 
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 
+CreateFindingsReportResponseTypeDef = TypedDict(
+    "CreateFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSbomExportResponseTypeDef = TypedDict(
+    "CreateSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+Cvss2TypeDef = TypedDict(
+    "Cvss2TypeDef",
+    {
+        "baseScore": float,
+        "scoringVector": str,
+    },
+    total=False,
+)
+
+Cvss3TypeDef = TypedDict(
+    "Cvss3TypeDef",
+    {
+        "baseScore": float,
+        "scoringVector": str,
+    },
+    total=False,
+)
+
 CvssScoreAdjustmentTypeDef = TypedDict(
     "CvssScoreAdjustmentTypeDef",
     {
         "metric": str,
         "reason": str,
     },
 )
@@ -546,21 +794,37 @@
 DeleteFilterRequestRequestTypeDef = TypedDict(
     "DeleteFilterRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DeleteFilterResponseTypeDef = TypedDict(
+    "DeleteFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
+DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisableRequestRequestTypeDef = TypedDict(
     "DisableRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
     total=False,
@@ -569,14 +833,22 @@
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
+DisassociateMemberResponseTypeDef = TypedDict(
+    "DisassociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMapFilterTypeDef = TypedDict(
     "_RequiredMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -655,14 +927,22 @@
 class EnableDelegatedAdminAccountRequestRequestTypeDef(
     _RequiredEnableDelegatedAdminAccountRequestRequestTypeDef,
     _OptionalEnableDelegatedAdminAccountRequestRequestTypeDef,
 ):
     pass
 
 
+EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
 )
 _OptionalEnableRequestRequestTypeDef = TypedDict(
@@ -677,14 +957,39 @@
 
 class EnableRequestRequestTypeDef(
     _RequiredEnableRequestRequestTypeDef, _OptionalEnableRequestRequestTypeDef
 ):
     pass
 
 
+EpssDetailsTypeDef = TypedDict(
+    "EpssDetailsTypeDef",
+    {
+        "score": float,
+    },
+    total=False,
+)
+
+EpssTypeDef = TypedDict(
+    "EpssTypeDef",
+    {
+        "score": float,
+    },
+    total=False,
+)
+
+ExploitObservedTypeDef = TypedDict(
+    "ExploitObservedTypeDef",
+    {
+        "firstSeen": datetime,
+        "lastSeen": datetime,
+    },
+    total=False,
+)
+
 ExploitabilityDetailsTypeDef = TypedDict(
     "ExploitabilityDetailsTypeDef",
     {
         "lastKnownExploitAt": datetime,
     },
     total=False,
 )
@@ -713,14 +1018,41 @@
         "end": datetime,
         "start": datetime,
         "status": FreeTrialStatusType,
         "type": FreeTrialTypeType,
     },
 )
 
+GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetEncryptionKeyRequestRequestTypeDef = TypedDict(
+    "GetEncryptionKeyRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "scanType": ScanTypeType,
+    },
+)
+
+GetEncryptionKeyResponseTypeDef = TypedDict(
+    "GetEncryptionKeyResponseTypeDef",
+    {
+        "kmsKeyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFindingsReportStatusRequestRequestTypeDef = TypedDict(
     "GetFindingsReportStatusRequestRequestTypeDef",
     {
         "reportId": str,
     },
     total=False,
 )
@@ -739,31 +1071,37 @@
         "delegatedAdminAccountId": str,
         "relationshipStatus": RelationshipStatusType,
         "updatedAt": datetime,
     },
     total=False,
 )
 
+GetSbomExportRequestRequestTypeDef = TypedDict(
+    "GetSbomExportRequestRequestTypeDef",
+    {
+        "reportId": str,
+    },
+)
+
 LambdaFunctionMetadataTypeDef = TypedDict(
     "LambdaFunctionMetadataTypeDef",
     {
         "functionName": str,
         "functionTags": Dict[str, str],
         "layers": List[str],
         "runtime": RuntimeType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "service": ServiceType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccountPermissionsRequestRequestTypeDef = TypedDict(
     "ListAccountPermissionsRequestRequestTypeDef",
     {
@@ -778,23 +1116,41 @@
     "PermissionTypeDef",
     {
         "operation": OperationType,
         "service": ServiceType,
     },
 )
 
+ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDelegatedAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "action": FilterActionType,
+        "arns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "arns": Sequence[str],
         "maxResults": int,
         "nextToken": str,
@@ -806,14 +1162,23 @@
     "SortCriteriaTypeDef",
     {
         "field": SortFieldType,
         "sortOrder": SortOrderType,
     },
 )
 
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": bool,
     },
@@ -823,14 +1188,31 @@
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
+ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListUsageTotalsRequestRequestTypeDef = TypedDict(
     "ListUsageTotalsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -879,23 +1261,89 @@
 
 class VulnerablePackageTypeDef(
     _RequiredVulnerablePackageTypeDef, _OptionalVulnerablePackageTypeDef
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Url": str,
         "text": str,
     },
     total=False,
 )
 
+ResetEncryptionKeyRequestRequestTypeDef = TypedDict(
+    "ResetEncryptionKeyRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "scanType": ScanTypeType,
+    },
+)
+
+_RequiredResourceMapFilterTypeDef = TypedDict(
+    "_RequiredResourceMapFilterTypeDef",
+    {
+        "comparison": Literal["EQUALS"],
+        "key": str,
+    },
+)
+_OptionalResourceMapFilterTypeDef = TypedDict(
+    "_OptionalResourceMapFilterTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class ResourceMapFilterTypeDef(
+    _RequiredResourceMapFilterTypeDef, _OptionalResourceMapFilterTypeDef
+):
+    pass
+
+
+ResourceStringFilterTypeDef = TypedDict(
+    "ResourceStringFilterTypeDef",
+    {
+        "comparison": ResourceStringComparisonType,
+        "value": str,
+    },
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
+SearchVulnerabilitiesFilterCriteriaTypeDef = TypedDict(
+    "SearchVulnerabilitiesFilterCriteriaTypeDef",
+    {
+        "vulnerabilityIds": Sequence[str],
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
@@ -904,14 +1352,58 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
+    {
+        "activateDeepInspection": bool,
+        "packagePaths": Sequence[str],
+    },
+    total=False,
+)
+
+UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateEncryptionKeyRequestRequestTypeDef = TypedDict(
+    "UpdateEncryptionKeyRequestRequestTypeDef",
+    {
+        "kmsKeyId": str,
+        "resourceType": ResourceTypeType,
+        "scanType": ScanTypeType,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
+    {
+        "orgPackagePaths": Sequence[str],
+    },
+)
+
 UsageTypeDef = TypedDict(
     "UsageTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedMonthlyCost": float,
         "total": float,
         "type": UsageTypeType,
@@ -1163,14 +1655,15 @@
         "ecr": StateTypeDef,
     },
 )
 _OptionalResourceStateTypeDef = TypedDict(
     "_OptionalResourceStateTypeDef",
     {
         "lambda": StateTypeDef,
+        "lambdaCode": StateTypeDef,
     },
     total=False,
 )
 
 
 class ResourceStateTypeDef(_RequiredResourceStateTypeDef, _OptionalResourceStateTypeDef):
     pass
@@ -1274,124 +1767,45 @@
     },
     total=False,
 )
 
 TitleAggregationTypeDef = TypedDict(
     "TitleAggregationTypeDef",
     {
+        "findingType": AggregationFindingTypeType,
         "resourceType": AggregationResourceTypeType,
         "sortBy": TitleSortByType,
         "sortOrder": SortOrderType,
         "titles": Sequence[StringFilterTypeDef],
         "vulnerabilityIds": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
-AssociateMemberResponseTypeDef = TypedDict(
-    "AssociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelFindingsReportResponseTypeDef = TypedDict(
-    "CancelFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFindingsReportResponseTypeDef = TypedDict(
-    "CreateFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFilterResponseTypeDef = TypedDict(
-    "DeleteFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateMemberResponseTypeDef = TypedDict(
-    "DisassociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
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
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
         "maxAccountLimitReached": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
     },
 )
 
 UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
     "UpdateOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1416,34 +1830,99 @@
 
 class AwsLambdaFunctionDetailsTypeDef(
     _RequiredAwsLambdaFunctionDetailsTypeDef, _OptionalAwsLambdaFunctionDetailsTypeDef
 ):
     pass
 
 
+BatchGetMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
+    "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
+    {
+        "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
+    "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
+    {
+        "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
+    "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    {
+        "accountIds": Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],
+    },
+)
+
+_RequiredCodeVulnerabilityDetailsTypeDef = TypedDict(
+    "_RequiredCodeVulnerabilityDetailsTypeDef",
+    {
+        "cwes": List[str],
+        "detectorId": str,
+        "detectorName": str,
+        "filePath": CodeFilePathTypeDef,
+    },
+)
+_OptionalCodeVulnerabilityDetailsTypeDef = TypedDict(
+    "_OptionalCodeVulnerabilityDetailsTypeDef",
+    {
+        "detectorTags": List[str],
+        "referenceUrls": List[str],
+        "ruleId": str,
+        "sourceLambdaLayerArn": str,
+    },
+    total=False,
+)
+
+
+class CodeVulnerabilityDetailsTypeDef(
+    _RequiredCodeVulnerabilityDetailsTypeDef, _OptionalCodeVulnerabilityDetailsTypeDef
+):
+    pass
+
+
+CodeSnippetResultTypeDef = TypedDict(
+    "CodeSnippetResultTypeDef",
+    {
+        "codeSnippet": List[CodeLineTypeDef],
+        "endLine": int,
+        "findingArn": str,
+        "startLine": int,
+        "suggestedFixes": List[SuggestedFixTypeDef],
+    },
+    total=False,
+)
+
 ListCoverageStatisticsResponseTypeDef = TypedDict(
     "ListCoverageStatisticsResponseTypeDef",
     {
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CoverageFilterCriteriaTypeDef = TypedDict(
     "CoverageFilterCriteriaTypeDef",
     {
         "accountId": Sequence[CoverageStringFilterTypeDef],
         "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
         "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
         "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
         "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
         "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
         "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
+        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
         "resourceId": Sequence[CoverageStringFilterTypeDef],
         "resourceType": Sequence[CoverageStringFilterTypeDef],
         "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
         "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
         "scanType": Sequence[CoverageStringFilterTypeDef],
     },
     total=False,
@@ -1473,23 +1952,23 @@
 
 
 ListDelegatedAdminAccountsResponseTypeDef = TypedDict(
     "ListDelegatedAdminAccountsResponseTypeDef",
     {
         "delegatedAdminAccounts": List[DelegatedAdminAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": Sequence[StringFilterTypeDef],
@@ -1526,14 +2005,48 @@
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
 )
 
+_RequiredVulnerabilityTypeDef = TypedDict(
+    "_RequiredVulnerabilityTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalVulnerabilityTypeDef = TypedDict(
+    "_OptionalVulnerabilityTypeDef",
+    {
+        "atigData": AtigDataTypeDef,
+        "cisaData": CisaDataTypeDef,
+        "cvss2": Cvss2TypeDef,
+        "cvss3": Cvss3TypeDef,
+        "cwes": List[str],
+        "description": str,
+        "detectionPlatforms": List[str],
+        "epss": EpssTypeDef,
+        "exploitObserved": ExploitObservedTypeDef,
+        "referenceUrls": List[str],
+        "relatedVulnerabilities": List[str],
+        "source": Literal["NVD"],
+        "sourceUrl": str,
+        "vendorCreatedAt": datetime,
+        "vendorSeverity": str,
+        "vendorUpdatedAt": datetime,
+    },
+    total=False,
+)
+
+
+class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
+    pass
+
+
 PackageFilterTypeDef = TypedDict(
     "PackageFilterTypeDef",
     {
         "architecture": StringFilterTypeDef,
         "epoch": NumberFilterTypeDef,
         "name": StringFilterTypeDef,
         "release": StringFilterTypeDef,
@@ -1552,89 +2065,44 @@
     },
 )
 
 GetMemberResponseTypeDef = TypedDict(
     "GetMemberResponseTypeDef",
     {
         "member": MemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceScanMetadataTypeDef = TypedDict(
     "ResourceScanMetadataTypeDef",
     {
         "ec2": Ec2MetadataTypeDef,
         "ecrImage": EcrContainerImageMetadataTypeDef,
         "ecrRepository": EcrRepositoryMetadataTypeDef,
         "lambdaFunction": LambdaFunctionMetadataTypeDef,
     },
     total=False,
 )
 
-ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
-    {
-        "service": ServiceType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "action": FilterActionType,
-        "arns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListAccountPermissionsResponseTypeDef = TypedDict(
     "ListAccountPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkPathTypeDef = TypedDict(
     "NetworkPathTypeDef",
     {
         "steps": List[StepTypeDef],
@@ -1675,14 +2143,73 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+ResourceFilterCriteriaTypeDef = TypedDict(
+    "ResourceFilterCriteriaTypeDef",
+    {
+        "accountId": Sequence[ResourceStringFilterTypeDef],
+        "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
+        "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
+        "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
+        "lambdaFunctionName": Sequence[ResourceStringFilterTypeDef],
+        "lambdaFunctionTags": Sequence[ResourceMapFilterTypeDef],
+        "resourceId": Sequence[ResourceStringFilterTypeDef],
+        "resourceType": Sequence[ResourceStringFilterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredSearchVulnerabilitiesRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchVulnerabilitiesRequestRequestTypeDef",
+    {
+        "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
+    },
+)
+_OptionalSearchVulnerabilitiesRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchVulnerabilitiesRequestRequestTypeDef",
+    {
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class SearchVulnerabilitiesRequestRequestTypeDef(
+    _RequiredSearchVulnerabilitiesRequestRequestTypeDef,
+    _OptionalSearchVulnerabilitiesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
+    "_RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
+    {
+        "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
+    },
+)
+_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
+    "_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(
+    _RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
+    _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
+):
+    pass
+
+
 UsageTotalTypeDef = TypedDict(
     "UsageTotalTypeDef",
     {
         "accountId": str,
         "usage": List[UsageTypeDef],
     },
     total=False,
@@ -1716,42 +2243,51 @@
 )
 
 DisableResponseTypeDef = TypedDict(
     "DisableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableResponseTypeDef = TypedDict(
     "EnableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEc2Instance": AwsEc2InstanceDetailsTypeDef,
         "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
         "awsLambdaFunction": AwsLambdaFunctionDetailsTypeDef,
     },
     total=False,
 )
 
+BatchGetCodeSnippetResponseTypeDef = TypedDict(
+    "BatchGetCodeSnippetResponseTypeDef",
+    {
+        "codeSnippetResults": List[CodeSnippetResultTypeDef],
+        "errors": List[CodeSnippetErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "ListCoverageRequestListCoveragePaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCoverageRequestRequestTypeDef = TypedDict(
     "ListCoverageRequestRequestTypeDef",
     {
@@ -1763,15 +2299,15 @@
 )
 
 ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
         "groupBy": GroupKeyType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
     "ListCoverageStatisticsRequestRequestTypeDef",
     {
@@ -1808,33 +2344,46 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchVulnerabilitiesResponseTypeDef = TypedDict(
+    "SearchVulnerabilitiesResponseTypeDef",
+    {
+        "nextToken": str,
+        "vulnerabilities": List[VulnerabilityTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
+        "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
+        "codeVulnerabilityDetectorTags": Sequence[StringFilterTypeDef],
+        "codeVulnerabilityFilePath": Sequence[StringFilterTypeDef],
         "componentId": Sequence[StringFilterTypeDef],
         "componentType": Sequence[StringFilterTypeDef],
         "ec2InstanceImageId": Sequence[StringFilterTypeDef],
         "ec2InstanceSubnetId": Sequence[StringFilterTypeDef],
         "ec2InstanceVpcId": Sequence[StringFilterTypeDef],
         "ecrImageArchitecture": Sequence[StringFilterTypeDef],
         "ecrImageHash": Sequence[StringFilterTypeDef],
         "ecrImagePushedAt": Sequence[DateFilterTypeDef],
         "ecrImageRegistry": Sequence[StringFilterTypeDef],
         "ecrImageRepositoryName": Sequence[StringFilterTypeDef],
         "ecrImageTags": Sequence[StringFilterTypeDef],
+        "epssScore": Sequence[NumberFilterTypeDef],
         "exploitAvailable": Sequence[StringFilterTypeDef],
         "findingArn": Sequence[StringFilterTypeDef],
         "findingStatus": Sequence[StringFilterTypeDef],
         "findingType": Sequence[StringFilterTypeDef],
         "firstObservedAt": Sequence[DateFilterTypeDef],
         "fixAvailable": Sequence[StringFilterTypeDef],
         "inspectorScore": Sequence[NumberFilterTypeDef],
@@ -1862,15 +2411,15 @@
 )
 
 BatchGetFreeTrialInfoResponseTypeDef = TypedDict(
     "BatchGetFreeTrialInfoResponseTypeDef",
     {
         "accounts": List[FreeTrialAccountInfoTypeDef],
         "failedAccounts": List[FreeTrialInfoErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCoveredResourceTypeDef = TypedDict(
     "_RequiredCoveredResourceTypeDef",
     {
         "accountId": str,
@@ -1878,14 +2427,15 @@
         "resourceType": CoverageResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 _OptionalCoveredResourceTypeDef = TypedDict(
     "_OptionalCoveredResourceTypeDef",
     {
+        "lastScannedAt": datetime,
         "resourceMetadata": ResourceScanMetadataTypeDef,
         "scanStatus": ScanStatusTypeDef,
     },
     total=False,
 )
 
 
@@ -1898,39 +2448,75 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
+_RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSbomExportRequestRequestTypeDef",
+    {
+        "reportFormat": SbomReportFormatType,
+        "s3Destination": DestinationTypeDef,
+    },
+)
+_OptionalCreateSbomExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSbomExportRequestRequestTypeDef",
+    {
+        "resourceFilterCriteria": ResourceFilterCriteriaTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateSbomExportRequestRequestTypeDef(
+    _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
+):
+    pass
+
+
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingAggregationsResponseTypeDef = TypedDict(
     "ListFindingAggregationsResponseTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "nextToken": str,
         "responses": List[AggregationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetAccountStatusResponseTypeDef = TypedDict(
     "BatchGetAccountStatusResponseTypeDef",
     {
         "accounts": List[AccountStateTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "id": str,
@@ -1960,15 +2546,15 @@
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "accountIds": Sequence[StringFilterTypeDef],
         "aggregationRequest": AggregationRequestTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(
     _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
@@ -2082,24 +2668,24 @@
     {
         "destination": DestinationTypeDef,
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
         "filterCriteria": FilterCriteriaTypeDef,
         "reportId": str,
         "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2137,15 +2723,15 @@
 
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "coveredResources": List[CoveredResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "awsAccountId": str,
@@ -2159,14 +2745,16 @@
         "status": FindingStatusType,
         "type": FindingTypeType,
     },
 )
 _OptionalFindingTypeDef = TypedDict(
     "_OptionalFindingTypeDef",
     {
+        "codeVulnerabilityDetails": CodeVulnerabilityDetailsTypeDef,
+        "epss": EpssDetailsTypeDef,
         "exploitAvailable": ExploitAvailableType,
         "exploitabilityDetails": ExploitabilityDetailsTypeDef,
         "fixAvailable": FixAvailableType,
         "inspectorScore": float,
         "inspectorScoreDetails": InspectorScoreDetailsTypeDef,
         "networkReachabilityDetails": NetworkReachabilityDetailsTypeDef,
         "packageVulnerabilityDetails": PackageVulnerabilityDetailsTypeDef,
@@ -2182,19 +2770,19 @@
 
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingsResponseTypeDef = TypedDict(
     "ListFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2/type_defs.pyi` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -19,17 +19,19 @@
     AccountSortByType,
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
+    CodeSnippetErrorCodeType,
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     DelegatedAdminStatusType,
+    Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
@@ -52,16 +54,18 @@
     PackageSortByType,
     PackageTypeType,
     RelationshipStatusType,
     ReportFormatType,
     ReportingErrorCodeType,
     RepositorySortByType,
     ResourceScanTypeType,
+    ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
+    SbomReportFormatType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
@@ -84,68 +88,115 @@
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateMemberResponseTypeDef",
+    "AtigDataTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
+    "BatchGetCodeSnippetRequestRequestTypeDef",
+    "CodeSnippetErrorTypeDef",
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
+    "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    "MemberAccountEc2DeepInspectionStatusStateTypeDef",
+    "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
+    "CancelFindingsReportResponseTypeDef",
+    "CancelSbomExportRequestRequestTypeDef",
+    "CancelSbomExportResponseTypeDef",
+    "CisaDataTypeDef",
+    "CodeFilePathTypeDef",
+    "CodeLineTypeDef",
+    "SuggestedFixTypeDef",
     "CountsTypeDef",
+    "CoverageDateFilterTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
+    "CreateFilterResponseTypeDef",
     "DestinationTypeDef",
+    "CreateFindingsReportResponseTypeDef",
+    "CreateSbomExportResponseTypeDef",
+    "Cvss2TypeDef",
+    "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DateFilterTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
+    "DeleteFilterResponseTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
+    "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
+    "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
+    "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
+    "EpssDetailsTypeDef",
+    "EpssTypeDef",
+    "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    "GetEncryptionKeyRequestRequestTypeDef",
+    "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
     "GetMemberRequestRequestTypeDef",
     "MemberTypeDef",
+    "GetSbomExportRequestRequestTypeDef",
     "LambdaFunctionMetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
     "ListAccountPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "SortCriteriaTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
+    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
+    "ResetEncryptionKeyRequestRequestTypeDef",
+    "ResourceMapFilterTypeDef",
+    "ResourceStringFilterTypeDef",
+    "ResponseMetadataTypeDef",
+    "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    "UpdateEncryptionKeyRequestRequestTypeDef",
+    "UpdateFilterResponseTypeDef",
+    "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     "UsageTypeDef",
     "AccountAggregationResponseTypeDef",
     "AmiAggregationResponseTypeDef",
     "AwsEcrContainerAggregationResponseTypeDef",
     "Ec2InstanceAggregationResponseTypeDef",
     "FindingTypeAggregationResponseTypeDef",
     "ImageLayerAggregationResponseTypeDef",
@@ -160,68 +211,66 @@
     "AmiAggregationTypeDef",
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
-    "AssociateMemberResponseTypeDef",
-    "CancelFindingsReportResponseTypeDef",
-    "CreateFilterResponseTypeDef",
-    "CreateFindingsReportResponseTypeDef",
-    "DeleteFilterResponseTypeDef",
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    "DisassociateMemberResponseTypeDef",
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateFilterResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateOrganizationConfigurationResponseTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
+    "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
+    "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
+    "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    "CodeVulnerabilityDetailsTypeDef",
+    "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
+    "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaTypeDef",
+    "SearchVulnerabilitiesRequestRequestTypeDef",
+    "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
+    "BatchGetCodeSnippetResponseTypeDef",
     "ListCoverageRequestListCoveragePaginateTypeDef",
     "ListCoverageRequestRequestTypeDef",
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     "ListCoverageStatisticsRequestRequestTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
+    "SearchVulnerabilitiesResponseTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
+    "GetSbomExportResponseTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
@@ -275,14 +324,15 @@
         "ecr": StatusType,
     },
 )
 _OptionalResourceStatusTypeDef = TypedDict(
     "_OptionalResourceStatusTypeDef",
     {
         "lambda": StatusType,
+        "lambdaCode": StatusType,
     },
     total=False,
 )
 
 class ResourceStatusTypeDef(_RequiredResourceStatusTypeDef, _OptionalResourceStatusTypeDef):
     pass
 
@@ -308,36 +358,45 @@
 AssociateMemberRequestRequestTypeDef = TypedDict(
     "AssociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateMemberResponseTypeDef = TypedDict(
+    "AssociateMemberResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AtigDataTypeDef = TypedDict(
+    "AtigDataTypeDef",
+    {
+        "firstSeen": datetime,
+        "lastSeen": datetime,
+        "targets": List[str],
+        "ttps": List[str],
     },
+    total=False,
 )
 
 _RequiredAutoEnableTypeDef = TypedDict(
     "_RequiredAutoEnableTypeDef",
     {
         "ec2": bool,
         "ecr": bool,
     },
 )
 _OptionalAutoEnableTypeDef = TypedDict(
     "_OptionalAutoEnableTypeDef",
     {
         "lambda": bool,
+        "lambdaCode": bool,
     },
     total=False,
 )
 
 class AutoEnableTypeDef(_RequiredAutoEnableTypeDef, _OptionalAutoEnableTypeDef):
     pass
 
@@ -397,14 +456,30 @@
     "BatchGetAccountStatusRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
+BatchGetCodeSnippetRequestRequestTypeDef = TypedDict(
+    "BatchGetCodeSnippetRequestRequestTypeDef",
+    {
+        "findingArns": Sequence[str],
+    },
+)
+
+CodeSnippetErrorTypeDef = TypedDict(
+    "CodeSnippetErrorTypeDef",
+    {
+        "errorCode": CodeSnippetErrorCodeType,
+        "errorMessage": str,
+        "findingArn": str,
+    },
+)
+
 BatchGetFreeTrialInfoRequestRequestTypeDef = TypedDict(
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 
@@ -413,30 +488,157 @@
     {
         "accountId": str,
         "code": FreeTrialInfoErrorCodeType,
         "message": str,
     },
 )
 
+BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
+    "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    {
+        "accountIds": Sequence[str],
+    },
+    total=False,
+)
+
+_RequiredFailedMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_RequiredFailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalFailedMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_OptionalFailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "ec2ScanStatus": StatusType,
+        "errorMessage": str,
+    },
+    total=False,
+)
+
+class FailedMemberAccountEc2DeepInspectionStatusStateTypeDef(
+    _RequiredFailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    _OptionalFailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+):
+    pass
+
+_RequiredMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_RequiredMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalMemberAccountEc2DeepInspectionStatusStateTypeDef = TypedDict(
+    "_OptionalMemberAccountEc2DeepInspectionStatusStateTypeDef",
+    {
+        "errorMessage": str,
+        "status": Ec2DeepInspectionStatusType,
+    },
+    total=False,
+)
+
+class MemberAccountEc2DeepInspectionStatusStateTypeDef(
+    _RequiredMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    _OptionalMemberAccountEc2DeepInspectionStatusStateTypeDef,
+):
+    pass
+
+MemberAccountEc2DeepInspectionStatusTypeDef = TypedDict(
+    "MemberAccountEc2DeepInspectionStatusTypeDef",
+    {
+        "accountId": str,
+        "activateDeepInspection": bool,
+    },
+)
+
 CancelFindingsReportRequestRequestTypeDef = TypedDict(
     "CancelFindingsReportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
+CancelFindingsReportResponseTypeDef = TypedDict(
+    "CancelFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CancelSbomExportRequestRequestTypeDef = TypedDict(
+    "CancelSbomExportRequestRequestTypeDef",
+    {
+        "reportId": str,
+    },
+)
+
+CancelSbomExportResponseTypeDef = TypedDict(
+    "CancelSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CisaDataTypeDef = TypedDict(
+    "CisaDataTypeDef",
+    {
+        "action": str,
+        "dateAdded": datetime,
+        "dateDue": datetime,
+    },
+    total=False,
+)
+
+CodeFilePathTypeDef = TypedDict(
+    "CodeFilePathTypeDef",
+    {
+        "endLine": int,
+        "fileName": str,
+        "filePath": str,
+        "startLine": int,
+    },
+)
+
+CodeLineTypeDef = TypedDict(
+    "CodeLineTypeDef",
+    {
+        "content": str,
+        "lineNumber": int,
+    },
+)
+
+SuggestedFixTypeDef = TypedDict(
+    "SuggestedFixTypeDef",
+    {
+        "code": str,
+        "description": str,
+    },
+    total=False,
+)
+
 CountsTypeDef = TypedDict(
     "CountsTypeDef",
     {
         "count": int,
         "groupKey": GroupKeyType,
     },
     total=False,
 )
 
+CoverageDateFilterTypeDef = TypedDict(
+    "CoverageDateFilterTypeDef",
+    {
+        "endInclusive": Union[datetime, str],
+        "startInclusive": Union[datetime, str],
+    },
+    total=False,
+)
+
 _RequiredCoverageMapFilterTypeDef = TypedDict(
     "_RequiredCoverageMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -465,14 +667,22 @@
     "ScanStatusTypeDef",
     {
         "reason": ScanStatusReasonType,
         "statusCode": ScanStatusCodeType,
     },
 )
 
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -483,14 +693,48 @@
     },
     total=False,
 )
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
+CreateFindingsReportResponseTypeDef = TypedDict(
+    "CreateFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSbomExportResponseTypeDef = TypedDict(
+    "CreateSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+Cvss2TypeDef = TypedDict(
+    "Cvss2TypeDef",
+    {
+        "baseScore": float,
+        "scoringVector": str,
+    },
+    total=False,
+)
+
+Cvss3TypeDef = TypedDict(
+    "Cvss3TypeDef",
+    {
+        "baseScore": float,
+        "scoringVector": str,
+    },
+    total=False,
+)
+
 CvssScoreAdjustmentTypeDef = TypedDict(
     "CvssScoreAdjustmentTypeDef",
     {
         "metric": str,
         "reason": str,
     },
 )
@@ -535,21 +779,37 @@
 DeleteFilterRequestRequestTypeDef = TypedDict(
     "DeleteFilterRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DeleteFilterResponseTypeDef = TypedDict(
+    "DeleteFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
+DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisableRequestRequestTypeDef = TypedDict(
     "DisableRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
     total=False,
@@ -558,14 +818,22 @@
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
+DisassociateMemberResponseTypeDef = TypedDict(
+    "DisassociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMapFilterTypeDef = TypedDict(
     "_RequiredMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -640,14 +908,22 @@
 
 class EnableDelegatedAdminAccountRequestRequestTypeDef(
     _RequiredEnableDelegatedAdminAccountRequestRequestTypeDef,
     _OptionalEnableDelegatedAdminAccountRequestRequestTypeDef,
 ):
     pass
 
+EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
 )
 _OptionalEnableRequestRequestTypeDef = TypedDict(
@@ -660,14 +936,39 @@
 )
 
 class EnableRequestRequestTypeDef(
     _RequiredEnableRequestRequestTypeDef, _OptionalEnableRequestRequestTypeDef
 ):
     pass
 
+EpssDetailsTypeDef = TypedDict(
+    "EpssDetailsTypeDef",
+    {
+        "score": float,
+    },
+    total=False,
+)
+
+EpssTypeDef = TypedDict(
+    "EpssTypeDef",
+    {
+        "score": float,
+    },
+    total=False,
+)
+
+ExploitObservedTypeDef = TypedDict(
+    "ExploitObservedTypeDef",
+    {
+        "firstSeen": datetime,
+        "lastSeen": datetime,
+    },
+    total=False,
+)
+
 ExploitabilityDetailsTypeDef = TypedDict(
     "ExploitabilityDetailsTypeDef",
     {
         "lastKnownExploitAt": datetime,
     },
     total=False,
 )
@@ -696,14 +997,41 @@
         "end": datetime,
         "start": datetime,
         "status": FreeTrialStatusType,
         "type": FreeTrialTypeType,
     },
 )
 
+GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetEncryptionKeyRequestRequestTypeDef = TypedDict(
+    "GetEncryptionKeyRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "scanType": ScanTypeType,
+    },
+)
+
+GetEncryptionKeyResponseTypeDef = TypedDict(
+    "GetEncryptionKeyResponseTypeDef",
+    {
+        "kmsKeyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFindingsReportStatusRequestRequestTypeDef = TypedDict(
     "GetFindingsReportStatusRequestRequestTypeDef",
     {
         "reportId": str,
     },
     total=False,
 )
@@ -722,31 +1050,37 @@
         "delegatedAdminAccountId": str,
         "relationshipStatus": RelationshipStatusType,
         "updatedAt": datetime,
     },
     total=False,
 )
 
+GetSbomExportRequestRequestTypeDef = TypedDict(
+    "GetSbomExportRequestRequestTypeDef",
+    {
+        "reportId": str,
+    },
+)
+
 LambdaFunctionMetadataTypeDef = TypedDict(
     "LambdaFunctionMetadataTypeDef",
     {
         "functionName": str,
         "functionTags": Dict[str, str],
         "layers": List[str],
         "runtime": RuntimeType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "service": ServiceType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccountPermissionsRequestRequestTypeDef = TypedDict(
     "ListAccountPermissionsRequestRequestTypeDef",
     {
@@ -761,23 +1095,41 @@
     "PermissionTypeDef",
     {
         "operation": OperationType,
         "service": ServiceType,
     },
 )
 
+ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDelegatedAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "action": FilterActionType,
+        "arns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "arns": Sequence[str],
         "maxResults": int,
         "nextToken": str,
@@ -789,14 +1141,23 @@
     "SortCriteriaTypeDef",
     {
         "field": SortFieldType,
         "sortOrder": SortOrderType,
     },
 )
 
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": bool,
     },
@@ -806,14 +1167,31 @@
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
+ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListUsageTotalsRequestRequestTypeDef = TypedDict(
     "ListUsageTotalsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -860,23 +1238,87 @@
 )
 
 class VulnerablePackageTypeDef(
     _RequiredVulnerablePackageTypeDef, _OptionalVulnerablePackageTypeDef
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Url": str,
         "text": str,
     },
     total=False,
 )
 
+ResetEncryptionKeyRequestRequestTypeDef = TypedDict(
+    "ResetEncryptionKeyRequestRequestTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "scanType": ScanTypeType,
+    },
+)
+
+_RequiredResourceMapFilterTypeDef = TypedDict(
+    "_RequiredResourceMapFilterTypeDef",
+    {
+        "comparison": Literal["EQUALS"],
+        "key": str,
+    },
+)
+_OptionalResourceMapFilterTypeDef = TypedDict(
+    "_OptionalResourceMapFilterTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class ResourceMapFilterTypeDef(
+    _RequiredResourceMapFilterTypeDef, _OptionalResourceMapFilterTypeDef
+):
+    pass
+
+ResourceStringFilterTypeDef = TypedDict(
+    "ResourceStringFilterTypeDef",
+    {
+        "comparison": ResourceStringComparisonType,
+        "value": str,
+    },
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
+SearchVulnerabilitiesFilterCriteriaTypeDef = TypedDict(
+    "SearchVulnerabilitiesFilterCriteriaTypeDef",
+    {
+        "vulnerabilityIds": Sequence[str],
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
@@ -885,14 +1327,58 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
+    {
+        "activateDeepInspection": bool,
+        "packagePaths": Sequence[str],
+    },
+    total=False,
+)
+
+UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateEncryptionKeyRequestRequestTypeDef = TypedDict(
+    "UpdateEncryptionKeyRequestRequestTypeDef",
+    {
+        "kmsKeyId": str,
+        "resourceType": ResourceTypeType,
+        "scanType": ScanTypeType,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
+    {
+        "orgPackagePaths": Sequence[str],
+    },
+)
+
 UsageTypeDef = TypedDict(
     "UsageTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedMonthlyCost": float,
         "total": float,
         "type": UsageTypeType,
@@ -1126,14 +1612,15 @@
         "ecr": StateTypeDef,
     },
 )
 _OptionalResourceStateTypeDef = TypedDict(
     "_OptionalResourceStateTypeDef",
     {
         "lambda": StateTypeDef,
+        "lambdaCode": StateTypeDef,
     },
     total=False,
 )
 
 class ResourceStateTypeDef(_RequiredResourceStateTypeDef, _OptionalResourceStateTypeDef):
     pass
 
@@ -1233,124 +1720,45 @@
     },
     total=False,
 )
 
 TitleAggregationTypeDef = TypedDict(
     "TitleAggregationTypeDef",
     {
+        "findingType": AggregationFindingTypeType,
         "resourceType": AggregationResourceTypeType,
         "sortBy": TitleSortByType,
         "sortOrder": SortOrderType,
         "titles": Sequence[StringFilterTypeDef],
         "vulnerabilityIds": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
-AssociateMemberResponseTypeDef = TypedDict(
-    "AssociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelFindingsReportResponseTypeDef = TypedDict(
-    "CancelFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFindingsReportResponseTypeDef = TypedDict(
-    "CreateFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFilterResponseTypeDef = TypedDict(
-    "DeleteFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateMemberResponseTypeDef = TypedDict(
-    "DisassociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
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
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
         "maxAccountLimitReached": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
     },
 )
 
 UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
     "UpdateOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1373,34 +1781,97 @@
 )
 
 class AwsLambdaFunctionDetailsTypeDef(
     _RequiredAwsLambdaFunctionDetailsTypeDef, _OptionalAwsLambdaFunctionDetailsTypeDef
 ):
     pass
 
+BatchGetMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
+    "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
+    {
+        "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
+    "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
+    {
+        "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
+    "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
+    {
+        "accountIds": Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],
+    },
+)
+
+_RequiredCodeVulnerabilityDetailsTypeDef = TypedDict(
+    "_RequiredCodeVulnerabilityDetailsTypeDef",
+    {
+        "cwes": List[str],
+        "detectorId": str,
+        "detectorName": str,
+        "filePath": CodeFilePathTypeDef,
+    },
+)
+_OptionalCodeVulnerabilityDetailsTypeDef = TypedDict(
+    "_OptionalCodeVulnerabilityDetailsTypeDef",
+    {
+        "detectorTags": List[str],
+        "referenceUrls": List[str],
+        "ruleId": str,
+        "sourceLambdaLayerArn": str,
+    },
+    total=False,
+)
+
+class CodeVulnerabilityDetailsTypeDef(
+    _RequiredCodeVulnerabilityDetailsTypeDef, _OptionalCodeVulnerabilityDetailsTypeDef
+):
+    pass
+
+CodeSnippetResultTypeDef = TypedDict(
+    "CodeSnippetResultTypeDef",
+    {
+        "codeSnippet": List[CodeLineTypeDef],
+        "endLine": int,
+        "findingArn": str,
+        "startLine": int,
+        "suggestedFixes": List[SuggestedFixTypeDef],
+    },
+    total=False,
+)
+
 ListCoverageStatisticsResponseTypeDef = TypedDict(
     "ListCoverageStatisticsResponseTypeDef",
     {
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CoverageFilterCriteriaTypeDef = TypedDict(
     "CoverageFilterCriteriaTypeDef",
     {
         "accountId": Sequence[CoverageStringFilterTypeDef],
         "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
         "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
         "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
         "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
         "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
         "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
+        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
         "resourceId": Sequence[CoverageStringFilterTypeDef],
         "resourceType": Sequence[CoverageStringFilterTypeDef],
         "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
         "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
         "scanType": Sequence[CoverageStringFilterTypeDef],
     },
     total=False,
@@ -1428,23 +1899,23 @@
     pass
 
 ListDelegatedAdminAccountsResponseTypeDef = TypedDict(
     "ListDelegatedAdminAccountsResponseTypeDef",
     {
         "delegatedAdminAccounts": List[DelegatedAdminAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": Sequence[StringFilterTypeDef],
@@ -1481,14 +1952,46 @@
 UpdateConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationRequestRequestTypeDef",
     {
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
 )
 
+_RequiredVulnerabilityTypeDef = TypedDict(
+    "_RequiredVulnerabilityTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalVulnerabilityTypeDef = TypedDict(
+    "_OptionalVulnerabilityTypeDef",
+    {
+        "atigData": AtigDataTypeDef,
+        "cisaData": CisaDataTypeDef,
+        "cvss2": Cvss2TypeDef,
+        "cvss3": Cvss3TypeDef,
+        "cwes": List[str],
+        "description": str,
+        "detectionPlatforms": List[str],
+        "epss": EpssTypeDef,
+        "exploitObserved": ExploitObservedTypeDef,
+        "referenceUrls": List[str],
+        "relatedVulnerabilities": List[str],
+        "source": Literal["NVD"],
+        "sourceUrl": str,
+        "vendorCreatedAt": datetime,
+        "vendorSeverity": str,
+        "vendorUpdatedAt": datetime,
+    },
+    total=False,
+)
+
+class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
+    pass
+
 PackageFilterTypeDef = TypedDict(
     "PackageFilterTypeDef",
     {
         "architecture": StringFilterTypeDef,
         "epoch": NumberFilterTypeDef,
         "name": StringFilterTypeDef,
         "release": StringFilterTypeDef,
@@ -1507,89 +2010,44 @@
     },
 )
 
 GetMemberResponseTypeDef = TypedDict(
     "GetMemberResponseTypeDef",
     {
         "member": MemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceScanMetadataTypeDef = TypedDict(
     "ResourceScanMetadataTypeDef",
     {
         "ec2": Ec2MetadataTypeDef,
         "ecrImage": EcrContainerImageMetadataTypeDef,
         "ecrRepository": EcrRepositoryMetadataTypeDef,
         "lambdaFunction": LambdaFunctionMetadataTypeDef,
     },
     total=False,
 )
 
-ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
-    {
-        "service": ServiceType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "action": FilterActionType,
-        "arns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListAccountPermissionsResponseTypeDef = TypedDict(
     "ListAccountPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkPathTypeDef = TypedDict(
     "NetworkPathTypeDef",
     {
         "steps": List[StepTypeDef],
@@ -1628,14 +2086,69 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+ResourceFilterCriteriaTypeDef = TypedDict(
+    "ResourceFilterCriteriaTypeDef",
+    {
+        "accountId": Sequence[ResourceStringFilterTypeDef],
+        "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
+        "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
+        "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
+        "lambdaFunctionName": Sequence[ResourceStringFilterTypeDef],
+        "lambdaFunctionTags": Sequence[ResourceMapFilterTypeDef],
+        "resourceId": Sequence[ResourceStringFilterTypeDef],
+        "resourceType": Sequence[ResourceStringFilterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredSearchVulnerabilitiesRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchVulnerabilitiesRequestRequestTypeDef",
+    {
+        "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
+    },
+)
+_OptionalSearchVulnerabilitiesRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchVulnerabilitiesRequestRequestTypeDef",
+    {
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class SearchVulnerabilitiesRequestRequestTypeDef(
+    _RequiredSearchVulnerabilitiesRequestRequestTypeDef,
+    _OptionalSearchVulnerabilitiesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
+    "_RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
+    {
+        "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
+    },
+)
+_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
+    "_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(
+    _RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
+    _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
+):
+    pass
+
 UsageTotalTypeDef = TypedDict(
     "UsageTotalTypeDef",
     {
         "accountId": str,
         "usage": List[UsageTypeDef],
     },
     total=False,
@@ -1669,42 +2182,51 @@
 )
 
 DisableResponseTypeDef = TypedDict(
     "DisableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableResponseTypeDef = TypedDict(
     "EnableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEc2Instance": AwsEc2InstanceDetailsTypeDef,
         "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
         "awsLambdaFunction": AwsLambdaFunctionDetailsTypeDef,
     },
     total=False,
 )
 
+BatchGetCodeSnippetResponseTypeDef = TypedDict(
+    "BatchGetCodeSnippetResponseTypeDef",
+    {
+        "codeSnippetResults": List[CodeSnippetResultTypeDef],
+        "errors": List[CodeSnippetErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "ListCoverageRequestListCoveragePaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCoverageRequestRequestTypeDef = TypedDict(
     "ListCoverageRequestRequestTypeDef",
     {
@@ -1716,15 +2238,15 @@
 )
 
 ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
     "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
     {
         "filterCriteria": CoverageFilterCriteriaTypeDef,
         "groupBy": GroupKeyType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
     "ListCoverageStatisticsRequestRequestTypeDef",
     {
@@ -1761,33 +2283,46 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SearchVulnerabilitiesResponseTypeDef = TypedDict(
+    "SearchVulnerabilitiesResponseTypeDef",
+    {
+        "nextToken": str,
+        "vulnerabilities": List[VulnerabilityTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
+        "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
+        "codeVulnerabilityDetectorTags": Sequence[StringFilterTypeDef],
+        "codeVulnerabilityFilePath": Sequence[StringFilterTypeDef],
         "componentId": Sequence[StringFilterTypeDef],
         "componentType": Sequence[StringFilterTypeDef],
         "ec2InstanceImageId": Sequence[StringFilterTypeDef],
         "ec2InstanceSubnetId": Sequence[StringFilterTypeDef],
         "ec2InstanceVpcId": Sequence[StringFilterTypeDef],
         "ecrImageArchitecture": Sequence[StringFilterTypeDef],
         "ecrImageHash": Sequence[StringFilterTypeDef],
         "ecrImagePushedAt": Sequence[DateFilterTypeDef],
         "ecrImageRegistry": Sequence[StringFilterTypeDef],
         "ecrImageRepositoryName": Sequence[StringFilterTypeDef],
         "ecrImageTags": Sequence[StringFilterTypeDef],
+        "epssScore": Sequence[NumberFilterTypeDef],
         "exploitAvailable": Sequence[StringFilterTypeDef],
         "findingArn": Sequence[StringFilterTypeDef],
         "findingStatus": Sequence[StringFilterTypeDef],
         "findingType": Sequence[StringFilterTypeDef],
         "firstObservedAt": Sequence[DateFilterTypeDef],
         "fixAvailable": Sequence[StringFilterTypeDef],
         "inspectorScore": Sequence[NumberFilterTypeDef],
@@ -1815,15 +2350,15 @@
 )
 
 BatchGetFreeTrialInfoResponseTypeDef = TypedDict(
     "BatchGetFreeTrialInfoResponseTypeDef",
     {
         "accounts": List[FreeTrialAccountInfoTypeDef],
         "failedAccounts": List[FreeTrialInfoErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCoveredResourceTypeDef = TypedDict(
     "_RequiredCoveredResourceTypeDef",
     {
         "accountId": str,
@@ -1831,14 +2366,15 @@
         "resourceType": CoverageResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 _OptionalCoveredResourceTypeDef = TypedDict(
     "_OptionalCoveredResourceTypeDef",
     {
+        "lastScannedAt": datetime,
         "resourceMetadata": ResourceScanMetadataTypeDef,
         "scanStatus": ScanStatusTypeDef,
     },
     total=False,
 )
 
 class CoveredResourceTypeDef(_RequiredCoveredResourceTypeDef, _OptionalCoveredResourceTypeDef):
@@ -1849,39 +2385,73 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
+_RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSbomExportRequestRequestTypeDef",
+    {
+        "reportFormat": SbomReportFormatType,
+        "s3Destination": DestinationTypeDef,
+    },
+)
+_OptionalCreateSbomExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSbomExportRequestRequestTypeDef",
+    {
+        "resourceFilterCriteria": ResourceFilterCriteriaTypeDef,
+    },
+    total=False,
+)
+
+class CreateSbomExportRequestRequestTypeDef(
+    _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
+):
+    pass
+
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingAggregationsResponseTypeDef = TypedDict(
     "ListFindingAggregationsResponseTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "nextToken": str,
         "responses": List[AggregationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetAccountStatusResponseTypeDef = TypedDict(
     "BatchGetAccountStatusResponseTypeDef",
     {
         "accounts": List[AccountStateTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "id": str,
@@ -1909,15 +2479,15 @@
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "accountIds": Sequence[StringFilterTypeDef],
         "aggregationRequest": AggregationRequestTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(
     _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
@@ -2021,24 +2591,24 @@
     {
         "destination": DestinationTypeDef,
         "errorCode": ReportingErrorCodeType,
         "errorMessage": str,
         "filterCriteria": FilterCriteriaTypeDef,
         "reportId": str,
         "status": ExternalReportStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2074,15 +2644,15 @@
     pass
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "coveredResources": List[CoveredResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "awsAccountId": str,
@@ -2096,14 +2666,16 @@
         "status": FindingStatusType,
         "type": FindingTypeType,
     },
 )
 _OptionalFindingTypeDef = TypedDict(
     "_OptionalFindingTypeDef",
     {
+        "codeVulnerabilityDetails": CodeVulnerabilityDetailsTypeDef,
+        "epss": EpssDetailsTypeDef,
         "exploitAvailable": ExploitAvailableType,
         "exploitabilityDetails": ExploitabilityDetailsTypeDef,
         "fixAvailable": FixAvailableType,
         "inspectorScore": float,
         "inspectorScoreDetails": InspectorScoreDetailsTypeDef,
         "networkReachabilityDetails": NetworkReachabilityDetailsTypeDef,
         "packageVulnerabilityDetails": PackageVulnerabilityDetailsTypeDef,
@@ -2117,19 +2689,19 @@
     pass
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFindingsResponseTypeDef = TypedDict(
     "ListFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/PKG-INFO` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector2
-Version: 1.26.37
-Summary: Type annotations for boto3.Inspector2 1.26.37 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Inspector2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-inspector2"></a>
 
 # mypy-boto3-inspector2
 
 [![PyPI - mypy-boto3-inspector2](https://img.shields.io/pypi/v/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector2.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector2?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector2 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
+[boto3.Inspector2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-inspector2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,14 +288,15 @@
     ListCoverageStatisticsPaginator,
     ListDelegatedAdminAccountsPaginator,
     ListFiltersPaginator,
     ListFindingAggregationsPaginator,
     ListFindingsPaginator,
     ListMembersPaginator,
     ListUsageTotalsPaginator,
+    SearchVulnerabilitiesPaginator,
 )
 
 client: Inspector2Client = Session().client("inspector2")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_account_permissions_paginator: ListAccountPermissionsPaginator = client.get_paginator(
@@ -311,14 +312,17 @@
 list_filters_paginator: ListFiltersPaginator = client.get_paginator("list_filters")
 list_finding_aggregations_paginator: ListFindingAggregationsPaginator = client.get_paginator(
     "list_finding_aggregations"
 )
 list_findings_paginator: ListFindingsPaginator = client.get_paginator("list_findings")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_usage_totals_paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
+search_vulnerabilities_paginator: SearchVulnerabilitiesPaginator = client.get_paginator(
+    "search_vulnerabilities"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_inspector2.literals` module contains literals extracted from shapes
@@ -329,19 +333,21 @@
     AccountSortByType,
     AggregationFindingTypeType,
     AggregationResourceTypeType,
     AggregationTypeType,
     AmiSortByType,
     ArchitectureType,
     AwsEcrContainerSortByType,
+    CodeSnippetErrorCodeType,
     CoverageMapComparisonType,
     CoverageResourceTypeType,
     CoverageStringComparisonType,
     CurrencyType,
     DelegatedAdminStatusType,
+    Ec2DeepInspectionStatusType,
     Ec2InstanceSortByType,
     Ec2PlatformType,
     EcrRescanDurationStatusType,
     EcrRescanDurationType,
     EcrScanFrequencyType,
     ErrorCodeType,
     ExploitAvailableType,
@@ -373,28 +379,33 @@
     PackageManagerType,
     PackageSortByType,
     PackageTypeType,
     RelationshipStatusType,
     ReportFormatType,
     ReportingErrorCodeType,
     RepositorySortByType,
+    ResourceMapComparisonType,
     ResourceScanTypeType,
+    ResourceStringComparisonType,
     ResourceTypeType,
     RuntimeType,
+    SbomReportFormatType,
     ScanStatusCodeType,
     ScanStatusReasonType,
     ScanTypeType,
+    SearchVulnerabilitiesPaginatorName,
     ServiceType,
     SeverityType,
     SortFieldType,
     SortOrderType,
     StatusType,
     StringComparisonType,
     TitleSortByType,
     UsageTypeType,
+    VulnerabilitySourceType,
     Inspector2ServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -415,68 +426,115 @@
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateMemberResponseTypeDef,
+    AtigDataTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
+    BatchGetCodeSnippetRequestRequestTypeDef,
+    CodeSnippetErrorTypeDef,
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
+    FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
+    MemberAccountEc2DeepInspectionStatusStateTypeDef,
+    MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportRequestRequestTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CisaDataTypeDef,
+    CodeFilePathTypeDef,
+    CodeLineTypeDef,
+    SuggestedFixTypeDef,
     CountsTypeDef,
+    CoverageDateFilterTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
+    CreateFilterResponseTypeDef,
     DestinationTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    Cvss2TypeDef,
+    Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DateFilterTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
+    DeleteFilterResponseTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
+    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
+    EpssDetailsTypeDef,
+    EpssTypeDef,
+    ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyRequestRequestTypeDef,
+    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
+    GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
+    ResetEncryptionKeyRequestRequestTypeDef,
+    ResourceMapFilterTypeDef,
+    ResourceStringFilterTypeDef,
+    ResponseMetadataTypeDef,
+    SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateEncryptionKeyRequestRequestTypeDef,
+    UpdateFilterResponseTypeDef,
+    UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
     ImageLayerAggregationResponseTypeDef,
@@ -491,68 +549,66 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
-    AssociateMemberResponseTypeDef,
-    CancelFindingsReportResponseTypeDef,
-    CreateFilterResponseTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    DeleteFilterResponseTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
-    DisassociateMemberResponseTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
+    BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
+    BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
+    CodeVulnerabilityDetailsTypeDef,
+    CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     CoverageFilterCriteriaTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
+    VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaTypeDef,
+    SearchVulnerabilitiesRequestRequestTypeDef,
+    SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
+    BatchGetCodeSnippetResponseTypeDef,
     ListCoverageRequestListCoveragePaginateTypeDef,
     ListCoverageRequestRequestTypeDef,
     ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
     ListCoverageStatisticsRequestRequestTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
+    SearchVulnerabilitiesResponseTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
+    GetSbomExportResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
     CreateFilterRequestRequestTypeDef,
@@ -576,42 +632,42 @@
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

### Comparing `mypy-boto3-inspector2-1.26.37/mypy_boto3_inspector2.egg-info/SOURCES.txt` & `mypy-boto3-inspector2-1.27.0/mypy_boto3_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector2-1.26.37/setup.py` & `mypy-boto3-inspector2-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-inspector2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector2",
-    version="1.26.37",
+    version="1.27.0",
     packages=["mypy_boto3_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector2 1.26.37 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.Inspector2 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector2/",
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


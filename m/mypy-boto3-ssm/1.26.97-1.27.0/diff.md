# Comparing `tmp/mypy-boto3-ssm-1.26.97.tar.gz` & `tmp/mypy-boto3-ssm-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-1.27.0.tar", last modified: Mon Jul  3 19:51:30 2023, max compression
```

## Comparing `mypy-boto3-ssm-1.26.97.tar` & `mypy-boto3-ssm-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.357775 mypy-boto3-ssm-1.26.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46048 2023-03-22 19:32:31.349775 mypy-boto3-ssm-1.26.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44577 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.345775 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131290 2023-03-22 19:32:16.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   131097 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-03-22 19:32:16.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   204155 2023-03-22 19:32:22.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   203927 2023-03-22 19:32:19.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-22 19:32:17.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.349775 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46048 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-22 19:32:31.000000 mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.357775 mypy-boto3-ssm-1.26.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-22 19:32:15.000000 mypy-boto3-ssm-1.26.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.888055 mypy-boto3-ssm-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46020 2023-07-03 19:51:30.888055 mypy-boto3-ssm-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44551 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.888055 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131264 2023-07-03 19:48:31.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131071 2023-07-03 19:48:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28094 2023-07-03 19:48:32.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28092 2023-07-03 19:48:32.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59280 2023-07-03 19:48:31.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59231 2023-07-03 19:48:31.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   204479 2023-07-03 19:48:36.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204251 2023-07-03 19:48:34.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 19:48:31.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-03 19:48:31.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.888055 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46020 2023-07-03 19:51:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:51:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:30.000000 mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:30.888055 mypy-boto3-ssm-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:48:27.000000 mypy-boto3-ssm-1.27.0/setup.py
```

### Comparing `mypy-boto3-ssm-1.26.97/LICENSE` & `mypy-boto3-ssm-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ssm-1.26.97/PKG-INFO` & `mypy-boto3-ssm-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.26.97
-Summary: Type annotations for boto3.SSM 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SSM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ssm"></a>
 
 # mypy-boto3-ssm
 
 [![PyPI - mypy-boto3-ssm](https://img.shields.io/pypi/v/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -647,15 +647,15 @@
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationOverviewTypeDef,
     AssociationStatusTypeDef,
     TargetTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
@@ -664,267 +664,267 @@
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
+    CreateActivationResultTypeDef,
     DocumentRequiresTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
+    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
+    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
+    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
+    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
+    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
+    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
+    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
     LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
+    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
+    PaginatorConfigTypeDef,
     ParameterInlinePolicyTypeDef,
     PatchFilterTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
+    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
+    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
+    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
+    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
+    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
     AlarmConfigurationTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
-    CreateActivationResultTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
-    CreateOpsItemResponseTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
-    DeleteParametersResultTypeDef,
-    DeletePatchBaselineResultTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesResultTypeDef,
-    GetCalendarStateResponseTypeDef,
-    GetConnectionStatusResponseTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
-    GetMaintenanceWindowResultTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListInventoryEntriesResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
-    ResumeSessionResponseTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
-    StartSessionResponseTypeDef,
-    TerminateSessionResponseTypeDef,
-    UnlabelParameterVersionResultTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateAssociationStatusRequestRequestTypeDef,
     AssociationTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
     DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
     RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
     UpdateDocumentRequestRequestTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
     GetCommandInvocationResultTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
     ComplianceItemTypeDef,
     PutComplianceItemsRequestRequestTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
     GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestRequestTypeDef,
     DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
+    DescribeActivationsRequestRequestTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
     DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
@@ -1113,42 +1113,42 @@
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

### Comparing `mypy-boto3-ssm-1.26.97/README.md` & `mypy-boto3-ssm-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ssm"></a>
 
 # mypy-boto3-ssm
 
 [![PyPI - mypy-boto3-ssm](https://img.shields.io/pypi/v/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -615,15 +615,15 @@
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationOverviewTypeDef,
     AssociationStatusTypeDef,
     TargetTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
@@ -632,267 +632,267 @@
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
+    CreateActivationResultTypeDef,
     DocumentRequiresTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
+    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
+    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
+    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
+    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
+    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
+    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
+    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
     LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
+    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
+    PaginatorConfigTypeDef,
     ParameterInlinePolicyTypeDef,
     PatchFilterTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
+    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
+    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
+    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
+    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
+    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
     AlarmConfigurationTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
-    CreateActivationResultTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
-    CreateOpsItemResponseTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
-    DeleteParametersResultTypeDef,
-    DeletePatchBaselineResultTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesResultTypeDef,
-    GetCalendarStateResponseTypeDef,
-    GetConnectionStatusResponseTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
-    GetMaintenanceWindowResultTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListInventoryEntriesResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
-    ResumeSessionResponseTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
-    StartSessionResponseTypeDef,
-    TerminateSessionResponseTypeDef,
-    UnlabelParameterVersionResultTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateAssociationStatusRequestRequestTypeDef,
     AssociationTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
     DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
     RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
     UpdateDocumentRequestRequestTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
     GetCommandInvocationResultTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
     ComplianceItemTypeDef,
     PutComplianceItemsRequestRequestTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
     GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestRequestTypeDef,
     DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
+    DescribeActivationsRequestRequestTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
     DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
@@ -1081,42 +1081,42 @@
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

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__init__.pyi` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/__main__.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.26.97\nVersion:         1.26.97\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.SSM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.97")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -998,17 +998,17 @@
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeInstanceInformationResultTypeDef:
         """
-        Describes one or more of your managed nodes, including information about the
-        operating system platform, the version of SSM Agent installed on the managed
-        node, node status, and so on.
+        Provides information about one or more of your managed nodes, including the
+        operating system platform, SSM Agent version, association status, and IP
+        address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_instance_information)
         """
 
     def describe_instance_patch_states(
         self, *, InstanceIds: Sequence[str], NextToken: str = ..., MaxResults: int = ...
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/client.pyi` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -951,17 +951,17 @@
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeInstanceInformationResultTypeDef:
         """
-        Describes one or more of your managed nodes, including information about the
-        operating system platform, the version of SSM Agent installed on the managed
-        node, node status, and so on.
+        Provides information about one or more of your managed nodes, including the
+        operating system platform, SSM Agent version, association status, and IP
+        address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_instance_information)
         """
     def describe_instance_patch_states(
         self, *, InstanceIds: Sequence[str], NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInstancePatchStatesResultTypeDef:
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,14 +530,15 @@
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
@@ -577,14 +578,15 @@
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
@@ -682,14 +684,15 @@
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
@@ -725,14 +728,15 @@
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
@@ -751,16 +755,19 @@
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
@@ -844,15 +851,17 @@
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

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/literals.pyi` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,15 @@
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
@@ -575,14 +576,15 @@
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
@@ -680,14 +682,15 @@
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
@@ -723,14 +726,15 @@
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
@@ -749,16 +753,19 @@
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
@@ -842,15 +849,17 @@
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

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
         """
 
 
@@ -289,15 +289,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 
@@ -308,15 +308,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAssociationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 
@@ -326,15 +326,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAutomationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 
@@ -346,15 +346,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAutomationStepExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 
@@ -364,60 +364,60 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 
 class DescribeEffectiveInstanceAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEffectiveInstanceAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
         """
 
 
 class DescribeEffectivePatchesForPatchBaselinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
     """
 
     def paginate(
-        self, *, BaselineId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BaselineId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEffectivePatchesForPatchBaselineResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
         """
 
 
 class DescribeInstanceAssociationsStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstanceAssociationsStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
         """
 
 
@@ -428,30 +428,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 
 class DescribeInstancePatchStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstancePatchStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
         """
 
 
@@ -462,15 +462,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 
@@ -481,30 +481,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 
 class DescribeInventoryDeletionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
-        self, *, DeletionId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DeletionId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInventoryDeletionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
         """
 
 
@@ -516,15 +516,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 
@@ -535,15 +535,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 
@@ -554,15 +554,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 
@@ -575,15 +575,15 @@
     def paginate(
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 
@@ -594,15 +594,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 
@@ -613,15 +613,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 
@@ -631,15 +631,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 
@@ -650,15 +650,15 @@
     """
 
     def paginate(
         self,
         *,
         Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 
@@ -668,15 +668,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
         """
 
 
@@ -687,15 +687,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeparameterspaginator)
         """
 
 
@@ -705,15 +705,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 
@@ -723,15 +723,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
         """
 
 
@@ -743,15 +743,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 
@@ -762,15 +762,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describesessionspaginator)
         """
 
 
@@ -782,15 +782,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventorypaginator)
         """
 
 
@@ -802,15 +802,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventoryschemapaginator)
         """
 
 
@@ -823,15 +823,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getopssummarypaginator)
         """
 
 
@@ -842,15 +842,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparameterhistorypaginator)
         """
 
 
@@ -863,45 +863,45 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparametersbypathpaginator)
         """
 
 
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
         """
 
 
 class ListAssociationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
     """
 
     def paginate(
-        self, *, AssociationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AssociationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
         """
 
 
@@ -911,15 +911,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
         """
 
 
@@ -932,15 +932,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 
@@ -952,15 +952,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCommandsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandspaginator)
         """
 
 
@@ -972,15 +972,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 
@@ -990,30 +990,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 
 class ListDocumentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
         """
 
 
@@ -1024,15 +1024,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentspaginator)
         """
 
 
@@ -1042,15 +1042,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
         """
 
 
@@ -1061,15 +1061,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 
@@ -1079,15 +1079,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
         """
 
 
@@ -1097,28 +1097,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 
 class ListResourceDataSyncPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
     """
 
     def paginate(
-        self, *, SyncType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SyncType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceDataSyncResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/paginator.pyi` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeactivationspaginator)
         """
 
 class DescribeAssociationExecutionTargetsPaginator(Paginator):
@@ -285,15 +285,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 class DescribeAssociationExecutionsPaginator(Paginator):
@@ -303,15 +303,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAssociationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 class DescribeAutomationExecutionsPaginator(Paginator):
@@ -320,15 +320,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAutomationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 class DescribeAutomationStepExecutionsPaginator(Paginator):
@@ -339,15 +339,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAutomationStepExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 class DescribeAvailablePatchesPaginator(Paginator):
@@ -356,57 +356,57 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 class DescribeEffectiveInstanceAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEffectiveInstanceAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
         """
 
 class DescribeEffectivePatchesForPatchBaselinePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
     """
 
     def paginate(
-        self, *, BaselineId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BaselineId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEffectivePatchesForPatchBaselineResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
         """
 
 class DescribeInstanceAssociationsStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstanceAssociationsStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceassociationsstatuspaginator)
         """
 
 class DescribeInstanceInformationPaginator(Paginator):
@@ -416,29 +416,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 class DescribeInstancePatchStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstancePatchStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatespaginator)
         """
 
 class DescribeInstancePatchStatesForPatchGroupPaginator(Paginator):
@@ -448,15 +448,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 class DescribeInstancePatchesPaginator(Paginator):
@@ -466,29 +466,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 class DescribeInventoryDeletionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
-        self, *, DeletionId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DeletionId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeInventoryDeletionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTaskInvocationsPaginator(Paginator):
@@ -499,15 +499,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTasksPaginator(Paginator):
@@ -517,15 +517,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionsPaginator(Paginator):
@@ -535,15 +535,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 class DescribeMaintenanceWindowSchedulePaginator(Paginator):
@@ -555,15 +555,15 @@
     def paginate(
         self,
         *,
         WindowId: str = ...,
         Targets: Sequence[TargetTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 class DescribeMaintenanceWindowTargetsPaginator(Paginator):
@@ -573,15 +573,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 class DescribeMaintenanceWindowTasksPaginator(Paginator):
@@ -591,15 +591,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 class DescribeMaintenanceWindowsPaginator(Paginator):
@@ -608,15 +608,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 class DescribeMaintenanceWindowsForTargetPaginator(Paginator):
@@ -626,15 +626,15 @@
     """
 
     def paginate(
         self,
         *,
         Targets: Sequence[TargetTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 class DescribeOpsItemsPaginator(Paginator):
@@ -643,15 +643,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeopsitemspaginator)
         """
 
 class DescribeParametersPaginator(Paginator):
@@ -661,15 +661,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeparameterspaginator)
         """
 
 class DescribePatchBaselinesPaginator(Paginator):
@@ -678,15 +678,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 class DescribePatchGroupsPaginator(Paginator):
@@ -695,15 +695,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchgroupspaginator)
         """
 
 class DescribePatchPropertiesPaginator(Paginator):
@@ -714,15 +714,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 class DescribeSessionsPaginator(Paginator):
@@ -732,15 +732,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describesessionspaginator)
         """
 
 class GetInventoryPaginator(Paginator):
@@ -751,15 +751,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventorypaginator)
         """
 
 class GetInventorySchemaPaginator(Paginator):
@@ -770,15 +770,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getinventoryschemapaginator)
         """
 
 class GetOpsSummaryPaginator(Paginator):
@@ -790,15 +790,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getopssummarypaginator)
         """
 
 class GetParameterHistoryPaginator(Paginator):
@@ -808,15 +808,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparameterhistorypaginator)
         """
 
 class GetParametersByPathPaginator(Paginator):
@@ -828,43 +828,43 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getparametersbypathpaginator)
         """
 
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#getresourcepoliciespaginator)
         """
 
 class ListAssociationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
     """
 
     def paginate(
-        self, *, AssociationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AssociationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationversionspaginator)
         """
 
 class ListAssociationsPaginator(Paginator):
@@ -873,15 +873,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listassociationspaginator)
         """
 
 class ListCommandInvocationsPaginator(Paginator):
@@ -893,15 +893,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 class ListCommandsPaginator(Paginator):
@@ -912,15 +912,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCommandsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcommandspaginator)
         """
 
 class ListComplianceItemsPaginator(Paginator):
@@ -931,15 +931,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 class ListComplianceSummariesPaginator(Paginator):
@@ -948,29 +948,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 class ListDocumentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentversionspaginator)
         """
 
 class ListDocumentsPaginator(Paginator):
@@ -980,15 +980,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listdocumentspaginator)
         """
 
 class ListOpsItemEventsPaginator(Paginator):
@@ -997,15 +997,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemeventspaginator)
         """
 
 class ListOpsItemRelatedItemsPaginator(Paginator):
@@ -1015,15 +1015,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 class ListOpsMetadataPaginator(Paginator):
@@ -1032,15 +1032,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listopsmetadatapaginator)
         """
 
 class ListResourceComplianceSummariesPaginator(Paginator):
@@ -1049,27 +1049,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 class ListResourceDataSyncPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
     """
 
     def paginate(
-        self, *, SyncType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SyncType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceDataSyncResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#listresourcedatasyncpaginator)
         """
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     "AssociationOverviewTypeDef",
     "AssociationStatusTypeDef",
     "TargetTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
@@ -123,267 +123,267 @@
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
+    "CancelMaintenanceWindowExecutionResultTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
     "NotificationConfigTypeDef",
     "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
+    "CreateActivationResultTypeDef",
     "DocumentRequiresTypeDef",
+    "CreateMaintenanceWindowResultTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
+    "CreateOpsItemResponseTypeDef",
     "MetadataValueTypeDef",
+    "CreateOpsMetadataResultTypeDef",
+    "CreatePatchBaselineResultTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
+    "DeleteMaintenanceWindowResultTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
     "DeleteParametersRequestRequestTypeDef",
+    "DeleteParametersResultTypeDef",
     "DeletePatchBaselineRequestRequestTypeDef",
+    "DeletePatchBaselineResultTypeDef",
     "DeleteResourceDataSyncRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeregisterManagedInstanceRequestRequestTypeDef",
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
     "DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     "DescribeActivationsFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "DescribeAssociationRequestRequestTypeDef",
     "StepExecutionFilterTypeDef",
     "PatchOrchestratorFilterTypeDef",
     "PatchTypeDef",
     "DescribeDocumentPermissionRequestRequestTypeDef",
     "DescribeDocumentRequestRequestTypeDef",
+    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     "InstanceAssociationTypeDef",
+    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
+    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
+    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
     "OpsItemFilterTypeDef",
     "ParameterStringFilterTypeDef",
     "ParametersFilterTypeDef",
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
+    "DescribePatchGroupStateResultTypeDef",
+    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
+    "DescribePatchPropertiesResultTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
+    "GetCalendarStateResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetCommandInvocationRequestRequestTypeDef",
     "GetConnectionStatusRequestRequestTypeDef",
+    "GetConnectionStatusResponseTypeDef",
     "GetDefaultPatchBaselineRequestRequestTypeDef",
+    "GetDefaultPatchBaselineResultTypeDef",
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
+    "GetMaintenanceWindowExecutionResultTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
+    "GetMaintenanceWindowResultTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
+    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
+    "GetPatchBaselineForPatchGroupResultTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
+    "LabelParameterVersionResultTypeDef",
+    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationVersionsRequestRequestTypeDef",
     "ListDocumentMetadataHistoryRequestRequestTypeDef",
+    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     "ListDocumentVersionsRequestRequestTypeDef",
+    "ListInventoryEntriesResultTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
     "MaintenanceWindowLambdaParametersTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterInlinePolicyTypeDef",
     "PatchFilterTypeDef",
+    "PutInventoryResultTypeDef",
+    "PutParameterResultTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
+    "RegisterDefaultPatchBaselineResultTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeSessionRequestRequestTypeDef",
+    "ResumeSessionResponseTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
+    "StartAutomationExecutionResultTypeDef",
+    "StartChangeRequestExecutionResultTypeDef",
     "StartSessionRequestRequestTypeDef",
+    "StartSessionResponseTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
+    "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionRequestRequestTypeDef",
+    "UnlabelParameterVersionResultTypeDef",
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     "UpdateMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowResultTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
+    "UpdateOpsMetadataResultTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
+    "DescribeDocumentPermissionResponseTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PutParameterRequestRequestTypeDef",
     "AlarmConfigurationTypeDef",
-    "AssociateOpsItemRelatedItemResponseTypeDef",
-    "CancelMaintenanceWindowExecutionResultTypeDef",
-    "CreateActivationResultTypeDef",
-    "CreateMaintenanceWindowResultTypeDef",
-    "CreateOpsItemResponseTypeDef",
-    "CreateOpsMetadataResultTypeDef",
-    "CreatePatchBaselineResultTypeDef",
-    "DeleteMaintenanceWindowResultTypeDef",
-    "DeleteParametersResultTypeDef",
-    "DeletePatchBaselineResultTypeDef",
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    "DescribeDocumentPermissionResponseTypeDef",
-    "DescribePatchGroupStateResultTypeDef",
-    "DescribePatchPropertiesResultTypeDef",
-    "GetCalendarStateResponseTypeDef",
-    "GetConnectionStatusResponseTypeDef",
-    "GetDefaultPatchBaselineResultTypeDef",
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    "GetMaintenanceWindowResultTypeDef",
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    "LabelParameterVersionResultTypeDef",
-    "ListInventoryEntriesResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PutInventoryResultTypeDef",
-    "PutParameterResultTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    "ResumeSessionResponseTypeDef",
-    "StartAutomationExecutionResultTypeDef",
-    "StartChangeRequestExecutionResultTypeDef",
-    "StartSessionResponseTypeDef",
-    "TerminateSessionResponseTypeDef",
-    "UnlabelParameterVersionResultTypeDef",
-    "UpdateMaintenanceWindowResultTypeDef",
-    "UpdateOpsMetadataResultTypeDef",
     "UpdateAssociationStatusRequestRequestTypeDef",
     "AssociationTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
     "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
+    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
+    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListAssociationsRequestRequestTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     "GetCommandInvocationResultTypeDef",
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
+    "ListCommandsRequestListCommandsPaginateTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
     "MaintenanceWindowRunCommandParametersTypeDef",
     "ComplianceItemTypeDef",
     "PutComplianceItemsRequestRequestTypeDef",
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
     "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
-    "DescribeActivationsRequestRequestTypeDef",
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
-    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    "DescribeActivationsRequestRequestTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
     "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
@@ -602,22 +602,19 @@
         "OpsItemId": str,
         "AssociationType": str,
         "ResourceType": str,
         "ResourceUri": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AssociationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociationOverviewTypeDef = TypedDict(
     "AssociationOverviewTypeDef",
     {
         "Status": str,
@@ -785,14 +782,22 @@
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
+CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "CancelMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
     },
     total=False,
@@ -908,14 +913,23 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateActivationResultTypeDef = TypedDict(
+    "CreateActivationResultTypeDef",
+    {
+        "ActivationId": str,
+        "ActivationCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDocumentRequiresTypeDef = TypedDict(
@@ -929,14 +943,22 @@
 )
 
 
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
 
+CreateMaintenanceWindowResultTypeDef = TypedDict(
+    "CreateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -953,22 +975,47 @@
 RelatedOpsItemTypeDef = TypedDict(
     "RelatedOpsItemTypeDef",
     {
         "OpsItemId": str,
     },
 )
 
+CreateOpsItemResponseTypeDef = TypedDict(
+    "CreateOpsItemResponseTypeDef",
+    {
+        "OpsItemId": str,
+        "OpsItemArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetadataValueTypeDef = TypedDict(
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+CreateOpsMetadataResultTypeDef = TypedDict(
+    "CreateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePatchBaselineResultTypeDef = TypedDict(
+    "CreatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1031,14 +1078,22 @@
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
+DeleteMaintenanceWindowResultTypeDef = TypedDict(
+    "DeleteMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteOpsMetadataRequestRequestTypeDef = TypedDict(
     "DeleteOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 
@@ -1052,21 +1107,38 @@
 DeleteParametersRequestRequestTypeDef = TypedDict(
     "DeleteParametersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
+DeleteParametersResultTypeDef = TypedDict(
+    "DeleteParametersResultTypeDef",
+    {
+        "DeletedParameters": List[str],
+        "InvalidParameters": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePatchBaselineRequestRequestTypeDef = TypedDict(
     "DeletePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+DeletePatchBaselineResultTypeDef = TypedDict(
+    "DeletePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
@@ -1105,14 +1177,23 @@
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
+DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
@@ -1128,37 +1209,45 @@
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
 
+DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-DescribeActivationsFilterTypeDef = TypedDict(
-    "DescribeActivationsFilterTypeDef",
+DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     {
-        "FilterKey": DescribeActivationsFilterKeysType,
-        "FilterValues": Sequence[str],
+        "WindowId": str,
+        "WindowTaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeActivationsFilterTypeDef = TypedDict(
+    "DescribeActivationsFilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FilterKey": DescribeActivationsFilterKeysType,
+        "FilterValues": Sequence[str],
     },
     total=False,
 )
 
 DescribeAssociationRequestRequestTypeDef = TypedDict(
     "DescribeAssociationRequestRequestTypeDef",
     {
@@ -1259,14 +1348,36 @@
 
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
+    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1293,14 +1404,36 @@
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
     },
     total=False,
 )
 
+_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "BaselineId": str,
+    },
+)
+_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
+    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
@@ -1316,14 +1449,36 @@
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
+    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1405,14 +1560,36 @@
 
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
 
+_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+    },
+)
+_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
+    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1454,14 +1631,23 @@
 
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
 
+DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    {
+        "DeletionId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1601,14 +1787,57 @@
 DescribePatchGroupStateRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupStateRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 
+DescribePatchGroupStateResultTypeDef = TypedDict(
+    "DescribePatchGroupStateResultTypeDef",
+    {
+        "Instances": int,
+        "InstancesWithInstalledPatches": int,
+        "InstancesWithInstalledOtherPatches": int,
+        "InstancesWithInstalledPendingRebootPatches": int,
+        "InstancesWithInstalledRejectedPatches": int,
+        "InstancesWithMissingPatches": int,
+        "InstancesWithFailedPatches": int,
+        "InstancesWithNotApplicablePatches": int,
+        "InstancesWithUnreportedNotApplicablePatches": int,
+        "InstancesWithCriticalNonCompliantPatches": int,
+        "InstancesWithSecurityNonCompliantPatches": int,
+        "InstancesWithOtherNonCompliantPatches": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "OperatingSystem": OperatingSystemType,
+        "Property": PatchPropertyType,
+    },
+)
+_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "PatchSet": PatchSetType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
+    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribePatchPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -1626,14 +1855,23 @@
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
 
+DescribePatchPropertiesResultTypeDef = TypedDict(
+    "DescribePatchPropertiesResultTypeDef",
+    {
+        "Properties": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1764,14 +2002,24 @@
 
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
 
+GetCalendarStateResponseTypeDef = TypedDict(
+    "GetCalendarStateResponseTypeDef",
+    {
+        "State": CalendarStateType,
+        "AtTime": str,
+        "NextTransitionTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1803,22 +2051,51 @@
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
+GetConnectionStatusResponseTypeDef = TypedDict(
+    "GetConnectionStatusResponseTypeDef",
+    {
+        "Target": str,
+        "Status": ConnectionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetDefaultPatchBaselineRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
+GetDefaultPatchBaselineResultTypeDef = TypedDict(
+    "GetDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": str,
+        "SnapshotDownloadUrl": str,
+        "Product": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -1861,14 +2138,25 @@
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
+GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    {
+        "TypeName": str,
+        "Aggregator": bool,
+        "SubType": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInventorySchemaRequestRequestTypeDef = TypedDict(
     "GetInventorySchemaRequestRequestTypeDef",
     {
         "TypeName": str,
         "NextToken": str,
         "MaxResults": int,
         "Aggregator": bool,
@@ -1880,23 +2168,55 @@
 GetMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
+GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskIds": List[str],
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "InvocationId": str,
     },
 )
 
+GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskExecutionId": str,
+        "InvocationId": str,
+        "ExecutionId": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "Parameters": str,
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "OwnerInformation": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMaintenanceWindowExecutionTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -1912,14 +2232,36 @@
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
+GetMaintenanceWindowResultTypeDef = TypedDict(
+    "GetMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "Name": str,
+        "Description": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "NextExecutionTime": str,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -2010,14 +2352,37 @@
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
+_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "WithDecryption": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
+    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetParameterHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterHistoryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterHistoryRequestRequestTypeDef = TypedDict(
@@ -2114,21 +2479,53 @@
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
 
+GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2289,14 +2686,45 @@
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
 
+LabelParameterVersionResultTypeDef = TypedDict(
+    "LabelParameterVersionResultTypeDef",
+    {
+        "InvalidLabels": List[str],
+        "ParameterVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
+    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2337,14 +2765,36 @@
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
+    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2360,14 +2810,27 @@
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListInventoryEntriesResultTypeDef = TypedDict(
+    "ListInventoryEntriesResultTypeDef",
+    {
+        "TypeName": str,
+        "InstanceId": str,
+        "SchemaVersion": str,
+        "CaptureTime": str,
+        "Entries": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2398,14 +2861,23 @@
         "LastModifiedDate": datetime,
         "LastModifiedUser": str,
         "CreationDate": datetime,
     },
     total=False,
 )
 
+ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    {
+        "SyncType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceDataSyncRequestRequestTypeDef = TypedDict(
     "ListResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2486,14 +2958,24 @@
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
     },
     total=False,
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
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
@@ -2504,14 +2986,31 @@
     "PatchFilterTypeDef",
     {
         "Key": PatchFilterKeyType,
         "Values": Sequence[str],
     },
 )
 
+PutInventoryResultTypeDef = TypedDict(
+    "PutInventoryResultTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutParameterResultTypeDef = TypedDict(
+    "PutParameterResultTypeDef",
+    {
+        "Version": int,
+        "Tier": ParameterTierType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
@@ -2527,29 +3026,71 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyHash": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
+RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    {
+        "WindowTargetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
+    {
+        "WindowTaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -2574,21 +3115,42 @@
     "ResourceDataSyncDestinationDataSharingTypeDef",
     {
         "DestinationDataSharingType": str,
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
 ResumeSessionRequestRequestTypeDef = TypedDict(
     "ResumeSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+ResumeSessionResponseTypeDef = TypedDict(
+    "ResumeSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendAutomationSignalRequestRequestTypeDef = TypedDict(
     "_RequiredSendAutomationSignalRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
         "SignalType": SignalTypeType,
     },
 )
@@ -2620,14 +3182,30 @@
 StartAssociationsOnceRequestRequestTypeDef = TypedDict(
     "StartAssociationsOnceRequestRequestTypeDef",
     {
         "AssociationIds": Sequence[str],
     },
 )
 
+StartAutomationExecutionResultTypeDef = TypedDict(
+    "StartAutomationExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartChangeRequestExecutionResultTypeDef = TypedDict(
+    "StartChangeRequestExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 _OptionalStartSessionRequestRequestTypeDef = TypedDict(
@@ -2643,14 +3221,24 @@
 
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
 
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
@@ -2672,23 +3260,40 @@
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnlabelParameterVersionRequestRequestTypeDef = TypedDict(
     "UnlabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "ParameterVersion": int,
         "Labels": Sequence[str],
     },
 )
 
+UnlabelParameterVersionResultTypeDef = TypedDict(
+    "UnlabelParameterVersionResultTypeDef",
+    {
+        "RemovedLabels": List[str],
+        "InvalidLabels": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateDocumentDefaultVersionRequestRequestTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
     },
 )
@@ -2722,30 +3327,67 @@
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateMaintenanceWindowResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "Name": str,
+        "Description": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
 
+UpdateOpsMetadataResultTypeDef = TypedDict(
+    "UpdateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateServiceSettingRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
         "SettingValue": str,
     },
 )
 
+DescribeDocumentPermissionResponseTypeDef = TypedDict(
+    "DescribeDocumentPermissionResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ActivationTypeDef = TypedDict(
     "ActivationTypeDef",
     {
         "ActivationId": str,
         "Description": str,
         "DefaultInstanceName": str,
         "IamRole": str,
@@ -2796,14 +3438,22 @@
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -2847,434 +3497,14 @@
 
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
 
-AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
-    "AssociateOpsItemRelatedItemResponseTypeDef",
-    {
-        "AssociationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "CancelMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateActivationResultTypeDef = TypedDict(
-    "CreateActivationResultTypeDef",
-    {
-        "ActivationId": str,
-        "ActivationCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMaintenanceWindowResultTypeDef = TypedDict(
-    "CreateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateOpsItemResponseTypeDef = TypedDict(
-    "CreateOpsItemResponseTypeDef",
-    {
-        "OpsItemId": str,
-        "OpsItemArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateOpsMetadataResultTypeDef = TypedDict(
-    "CreateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePatchBaselineResultTypeDef = TypedDict(
-    "CreatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMaintenanceWindowResultTypeDef = TypedDict(
-    "DeleteMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParametersResultTypeDef = TypedDict(
-    "DeleteParametersResultTypeDef",
-    {
-        "DeletedParameters": List[str],
-        "InvalidParameters": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePatchBaselineResultTypeDef = TypedDict(
-    "DeletePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDocumentPermissionResponseTypeDef = TypedDict(
-    "DescribeDocumentPermissionResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePatchGroupStateResultTypeDef = TypedDict(
-    "DescribePatchGroupStateResultTypeDef",
-    {
-        "Instances": int,
-        "InstancesWithInstalledPatches": int,
-        "InstancesWithInstalledOtherPatches": int,
-        "InstancesWithInstalledPendingRebootPatches": int,
-        "InstancesWithInstalledRejectedPatches": int,
-        "InstancesWithMissingPatches": int,
-        "InstancesWithFailedPatches": int,
-        "InstancesWithNotApplicablePatches": int,
-        "InstancesWithUnreportedNotApplicablePatches": int,
-        "InstancesWithCriticalNonCompliantPatches": int,
-        "InstancesWithSecurityNonCompliantPatches": int,
-        "InstancesWithOtherNonCompliantPatches": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePatchPropertiesResultTypeDef = TypedDict(
-    "DescribePatchPropertiesResultTypeDef",
-    {
-        "Properties": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCalendarStateResponseTypeDef = TypedDict(
-    "GetCalendarStateResponseTypeDef",
-    {
-        "State": CalendarStateType,
-        "AtTime": str,
-        "NextTransitionTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetConnectionStatusResponseTypeDef = TypedDict(
-    "GetConnectionStatusResponseTypeDef",
-    {
-        "Target": str,
-        "Status": ConnectionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDefaultPatchBaselineResultTypeDef = TypedDict(
-    "GetDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": str,
-        "SnapshotDownloadUrl": str,
-        "Product": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskIds": List[str],
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskExecutionId": str,
-        "InvocationId": str,
-        "ExecutionId": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "Parameters": str,
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "OwnerInformation": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMaintenanceWindowResultTypeDef = TypedDict(
-    "GetMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "NextExecutionTime": str,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LabelParameterVersionResultTypeDef = TypedDict(
-    "LabelParameterVersionResultTypeDef",
-    {
-        "InvalidLabels": List[str],
-        "ParameterVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListInventoryEntriesResultTypeDef = TypedDict(
-    "ListInventoryEntriesResultTypeDef",
-    {
-        "TypeName": str,
-        "InstanceId": str,
-        "SchemaVersion": str,
-        "CaptureTime": str,
-        "Entries": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutInventoryResultTypeDef = TypedDict(
-    "PutInventoryResultTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutParameterResultTypeDef = TypedDict(
-    "PutParameterResultTypeDef",
-    {
-        "Version": int,
-        "Tier": ParameterTierType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyHash": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTargetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResumeSessionResponseTypeDef = TypedDict(
-    "ResumeSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAutomationExecutionResultTypeDef = TypedDict(
-    "StartAutomationExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartChangeRequestExecutionResultTypeDef = TypedDict(
-    "StartChangeRequestExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UnlabelParameterVersionResultTypeDef = TypedDict(
-    "UnlabelParameterVersionResultTypeDef",
-    {
-        "RemovedLabels": List[str],
-        "InvalidLabels": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMaintenanceWindowResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateOpsMetadataResultTypeDef = TypedDict(
-    "UpdateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
     "UpdateAssociationStatusRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationStatus": AssociationStatusTypeDef,
     },
@@ -3295,14 +3525,37 @@
         "AssociationName": str,
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
         "Targets": Sequence[TargetTypeDef],
         "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
@@ -3396,18 +3649,45 @@
     {
         "WindowId": str,
         "WindowTargetId": str,
         "Targets": List[TargetTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "AssociationId": str,
+        },
+    )
+)
+_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "Filters": Sequence[AssociationExecutionFilterTypeDef],
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+
+class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
@@ -3440,14 +3720,38 @@
         "DetailedStatus": str,
         "LastExecutionDate": datetime,
         "OutputSource": OutputSourceTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "AssociationId": str,
+        "ExecutionId": str,
+    },
+)
+_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef",
     {
         "AssociationId": str,
         "ExecutionId": str,
     },
 )
@@ -3465,14 +3769,23 @@
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
 
+ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    {
+        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -3502,14 +3815,23 @@
 
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
 
+DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    {
+        "Filters": Sequence[AutomationExecutionFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -3532,31 +3854,54 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "Details": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[CommandFilterTypeDef],
         "Details": bool,
     },
     total=False,
 )
 
+ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCommandsRequestRequestTypeDef = TypedDict(
     "ListCommandsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -3645,36 +3990,65 @@
 class PutComplianceItemsRequestRequestTypeDef(
     _RequiredPutComplianceItemsRequestRequestTypeDef,
     _OptionalPutComplianceItemsRequestRequestTypeDef,
 ):
     pass
 
 
+ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "ResourceIds": Sequence[str],
+        "ResourceTypes": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -3788,15 +4162,15 @@
         "StatusInformation": str,
         "Content": str,
         "DocumentType": DocumentTypeType,
         "DocumentFormat": DocumentFormatType,
         "Requires": List[DocumentRequiresTypeDef],
         "AttachmentsContent": List[AttachmentContentTypeDef],
         "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpsItemSummaryTypeDef = TypedDict(
     "OpsItemSummaryTypeDef",
     {
         "CreatedBy": str,
@@ -3943,15 +4317,15 @@
 
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
@@ -3969,403 +4343,29 @@
 
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
 
-DescribeActivationsRequestRequestTypeDef = TypedDict(
-    "DescribeActivationsRequestRequestTypeDef",
-    {
-        "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribeActivationsRequestDescribeActivationsPaginateTypeDef = TypedDict(
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "AssociationId": str,
-        "ExecutionId": str,
-    },
-)
-_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "AssociationId": str,
-        },
-    )
-)
-_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "Filters": Sequence[AssociationExecutionFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-
-class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-):
-    pass
-
-
-DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    {
-        "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
-    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "BaselineId": str,
-    },
-)
-_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
-    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
-    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-    },
-)
-_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
-    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-):
-    pass
-
-
-DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    {
-        "DeletionId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "OperatingSystem": OperatingSystemType,
-        "Property": PatchPropertyType,
-    },
-)
-_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "PatchSet": PatchSetType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
-    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-):
-    pass
-
-
-GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    {
-        "TypeName": str,
-        "Aggregator": bool,
-        "SubType": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "WithDecryption": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
-    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
-    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    {
-        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "Details": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "ResourceIds": Sequence[str],
-        "ResourceTypes": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
-    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+DescribeActivationsRequestRequestTypeDef = TypedDict(
+    "DescribeActivationsRequestRequestTypeDef",
     {
-        "SyncType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": Sequence[DescribeActivationsFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
@@ -4373,15 +4373,15 @@
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
@@ -4415,15 +4415,15 @@
     pass
 
 
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAvailablePatchesRequestRequestTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestRequestTypeDef",
     {
@@ -4440,15 +4440,15 @@
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
@@ -4485,15 +4485,15 @@
     TypedDict(
         "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
         {
             "WindowId": str,
             "Targets": Sequence[TargetTypeDef],
             "ResourceType": MaintenanceWindowResourceTypeType,
             "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
 DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
@@ -4508,15 +4508,15 @@
     total=False,
 )
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePatchBaselinesRequestRequestTypeDef = TypedDict(
     "DescribePatchBaselinesRequestRequestTypeDef",
     {
@@ -4527,15 +4527,15 @@
     total=False,
 )
 
 DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef = TypedDict(
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePatchGroupsRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupsRequestRequestTypeDef",
     {
@@ -4547,33 +4547,33 @@
 )
 
 DescribeAvailablePatchesResultTypeDef = TypedDict(
     "DescribeAvailablePatchesResultTypeDef",
     {
         "Patches": List[PatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEffectiveInstanceAssociationsResultTypeDef = TypedDict(
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     {
         "Associations": List[InstanceAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef = TypedDict(
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     {
         "InstanceInformationFilterList": Sequence[InstanceInformationFilterTypeDef],
         "Filters": Sequence[InstanceInformationStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeInstanceInformationRequestRequestTypeDef = TypedDict(
     "DescribeInstanceInformationRequestRequestTypeDef",
     {
@@ -4591,15 +4591,15 @@
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
@@ -4633,48 +4633,48 @@
 
 
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstancePatchStatesResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstancePatchesResultTypeDef = TypedDict(
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
@@ -4714,15 +4714,15 @@
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
@@ -4761,15 +4761,15 @@
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
@@ -4808,15 +4808,15 @@
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
@@ -4855,15 +4855,15 @@
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
@@ -4896,15 +4896,15 @@
     pass
 
 
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeMaintenanceWindowsRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestRequestTypeDef",
     {
@@ -4918,59 +4918,59 @@
 DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef",
     {
         "WindowExecutionTaskInvocationIdentities": List[
             MaintenanceWindowExecutionTaskInvocationIdentityTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowExecutionsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionsResultTypeDef",
     {
         "WindowExecutions": List[MaintenanceWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowScheduleResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleResultTypeDef",
     {
         "ScheduledWindowExecutions": List[ScheduledWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowsForTargetResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsForTargetResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityForTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef = TypedDict(
     "DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef",
     {
         "OpsItemFilters": Sequence[OpsItemFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeOpsItemsRequestRequestTypeDef = TypedDict(
     "DescribeOpsItemsRequestRequestTypeDef",
     {
@@ -4989,15 +4989,15 @@
 )
 _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef = TypedDict(
     "_OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef",
     {
         "Recursive": bool,
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
@@ -5033,15 +5033,15 @@
 
 
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeParametersRequestRequestTypeDef = TypedDict(
     "DescribeParametersRequestRequestTypeDef",
     {
@@ -5054,15 +5054,15 @@
 )
 
 DescribePatchBaselinesResultTypeDef = TypedDict(
     "DescribePatchBaselinesResultTypeDef",
     {
         "BaselineIdentities": List[PatchBaselineIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PatchGroupPatchBaselineMappingTypeDef = TypedDict(
     "PatchGroupPatchBaselineMappingTypeDef",
     {
         "PatchGroup": str,
@@ -5077,15 +5077,15 @@
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
         "Filters": Sequence[SessionFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
@@ -5117,15 +5117,15 @@
     pass
 
 
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
@@ -5163,15 +5163,15 @@
 )
 
 ListDocumentsRequestListDocumentsPaginateTypeDef = TypedDict(
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     {
         "DocumentFilterList": Sequence[DocumentFilterTypeDef],
         "Filters": Sequence[DocumentKeyValuesFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
@@ -5215,15 +5215,15 @@
 
 
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EffectivePatchTypeDef = TypedDict(
     "EffectivePatchTypeDef",
     {
         "Patch": PatchTypeDef,
@@ -5291,15 +5291,15 @@
 
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetInventoryRequestRequestTypeDef = TypedDict(
     "GetInventoryRequestRequestTypeDef",
     {
@@ -5328,15 +5328,15 @@
 GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef = TypedDict(
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     {
         "SyncName": str,
         "Filters": Sequence[OpsFilterTypeDef],
         "Aggregators": Sequence["OpsAggregatorTypeDef"],
         "ResultAttributes": Sequence[OpsResultAttributeTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetOpsSummaryRequestRequestTypeDef = TypedDict(
     "GetOpsSummaryRequestRequestTypeDef",
     {
@@ -5350,58 +5350,58 @@
     total=False,
 )
 
 GetParameterResultTypeDef = TypedDict(
     "GetParameterResultTypeDef",
     {
         "Parameter": ParameterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParametersByPathResultTypeDef = TypedDict(
     "GetParametersByPathResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParametersResultTypeDef = TypedDict(
     "GetParametersResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceSettingResultTypeDef = TypedDict(
     "GetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetServiceSettingResultTypeDef = TypedDict(
     "ResetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceInformationTypeDef = TypedDict(
     "InstanceInformationTypeDef",
     {
         "InstanceId": str,
@@ -5495,15 +5495,15 @@
     total=False,
 )
 
 ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef = TypedDict(
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     {
         "Filters": Sequence[OpsItemEventFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOpsItemEventsRequestRequestTypeDef = TypedDict(
     "ListOpsItemEventsRequestRequestTypeDef",
     {
@@ -5515,15 +5515,15 @@
 )
 
 ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     {
         "OpsItemId": str,
         "Filters": Sequence[OpsItemRelatedItemsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOpsItemRelatedItemsRequestRequestTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     {
@@ -5535,15 +5535,15 @@
     total=False,
 )
 
 ListOpsMetadataRequestListOpsMetadataPaginateTypeDef = TypedDict(
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     {
         "Filters": Sequence[OpsMetadataFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOpsMetadataRequestRequestTypeDef = TypedDict(
     "ListOpsMetadataRequestRequestTypeDef",
     {
@@ -5555,15 +5555,15 @@
 )
 
 ListOpsMetadataResultTypeDef = TypedDict(
     "ListOpsMetadataResultTypeDef",
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
@@ -5713,15 +5713,15 @@
 )
 
 DescribeActivationsResultTypeDef = TypedDict(
     "DescribeActivationsResultTypeDef",
     {
         "ActivationList": List[ActivationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociationExecutionTypeDef = TypedDict(
     "AssociationExecutionTypeDef",
     {
         "AssociationId": str,
@@ -5785,15 +5785,15 @@
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     {
         "WindowExecutionId": str,
@@ -5883,42 +5883,42 @@
 )
 
 ListAssociationsResultTypeDef = TypedDict(
     "ListAssociationsResultTypeDef",
     {
         "Associations": List[AssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowTargetsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     {
         "Targets": List[MaintenanceWindowTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssociationExecutionTargetsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionTargetsResultTypeDef",
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
     "MaintenanceWindowTaskInvocationParametersTypeDef",
     {
         "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
@@ -5930,15 +5930,15 @@
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
         "ComplianceItems": List[ComplianceItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComplianceSummaryItemTypeDef = TypedDict(
     "ComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
@@ -5964,65 +5964,65 @@
 )
 
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOpsItemsResponseTypeDef = TypedDict(
     "DescribeOpsItemsResponseTypeDef",
     {
         "NextToken": str,
         "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOpsItemResponseTypeDef = TypedDict(
     "GetOpsItemResponseTypeDef",
     {
         "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePatchGroupsResultTypeDef = TypedDict(
     "DescribePatchGroupsResultTypeDef",
     {
         "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDocumentResultTypeDef = TypedDict(
     "DescribeDocumentResultTypeDef",
     {
         "Document": DocumentDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDocumentResultTypeDef = TypedDict(
     "UpdateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentMetadataResponseInfoTypeDef = TypedDict(
     "DocumentMetadataResponseInfoTypeDef",
     {
         "ReviewerResponse": List[DocumentReviewerResponseSourceTypeDef],
@@ -6054,15 +6054,15 @@
 
 
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InventoryAggregatorTypeDef = TypedDict(
     "InventoryAggregatorTypeDef",
     {
         "Expression": str,
@@ -6073,15 +6073,15 @@
 )
 
 DescribeInstanceInformationResultTypeDef = TypedDict(
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": str,
@@ -6102,15 +6102,15 @@
 
 DeleteInventoryResultTypeDef = TypedDict(
     "DeleteInventoryResultTypeDef",
     {
         "DeletionId": str,
         "TypeName": str,
         "DeletionSummary": InventoryDeletionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InventoryDeletionStatusItemTypeDef = TypedDict(
     "InventoryDeletionStatusItemTypeDef",
     {
         "DeletionId": str,
@@ -6125,69 +6125,69 @@
 )
 
 GetInventorySchemaResultTypeDef = TypedDict(
     "GetInventorySchemaResultTypeDef",
     {
         "Schemas": List[InventoryItemSchemaTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInventoryResultTypeDef = TypedDict(
     "GetInventoryResultTypeDef",
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOpsItemRelatedItemsResponseTypeDef = TypedDict(
     "ListOpsItemRelatedItemsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParametersResultTypeDef = TypedDict(
     "DescribeParametersResultTypeDef",
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
@@ -6247,59 +6247,59 @@
 )
 
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssociationExecutionsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionsResultTypeDef",
     {
         "AssociationExecutions": List[AssociationExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCommandsResultTypeDef = TypedDict(
     "ListCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "Command": CommandTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowExecutionTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     {
         "WindowExecutionTaskIdentities": List[MaintenanceWindowExecutionTaskIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTasksResultTypeDef",
     {
         "Tasks": List[MaintenanceWindowTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociationDescriptionTypeDef = TypedDict(
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
@@ -6581,15 +6581,15 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
@@ -6675,63 +6675,63 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListComplianceSummariesResultTypeDef = TypedDict(
     "ListComplianceSummariesResultTypeDef",
     {
         "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceComplianceSummariesResultTypeDef = TypedDict(
     "ListResourceComplianceSummariesResultTypeDef",
     {
         "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
     "ListDocumentMetadataHistoryResponseTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
         "Author": str,
         "Metadata": DocumentMetadataResponseInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
     "DescribeInstanceAssociationsStatusResultTypeDef",
     {
         "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInventoryDeletionsResultTypeDef = TypedDict(
     "DescribeInventoryDeletionsResultTypeDef",
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PatchRuleGroupTypeDef = TypedDict(
     "PatchRuleGroupTypeDef",
     {
         "PatchRules": Sequence[PatchRuleTypeDef],
@@ -6788,48 +6788,48 @@
     total=False,
 )
 
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssociationResultTypeDef = TypedDict(
     "DescribeAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssociationResultTypeDef = TypedDict(
     "UpdateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssociationStatusResultTypeDef = TypedDict(
     "UpdateAssociationStatusResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssociationVersionsResultTypeDef = TypedDict(
     "ListAssociationVersionsResultTypeDef",
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssociationBatchRequestRequestTypeDef = TypedDict(
     "CreateAssociationBatchRequestRequestTypeDef",
     {
         "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
@@ -6955,15 +6955,15 @@
 )
 
 DescribeAutomationStepExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationStepExecutionsResultTypeDef",
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
@@ -7026,15 +7026,15 @@
         "RejectedPatches": List[str],
         "RejectedPatchesAction": PatchActionType,
         "PatchGroups": List[str],
         "CreatedDate": datetime,
         "ModifiedDate": datetime,
         "Description": str,
         "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
@@ -7079,50 +7079,50 @@
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": List[str],
         "RejectedPatchesAction": PatchActionType,
         "CreatedDate": datetime,
         "ModifiedDate": datetime,
         "Description": str,
         "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssociationBatchResultTypeDef = TypedDict(
     "CreateAssociationBatchResultTypeDef",
     {
         "Successful": List[AssociationDescriptionTypeDef],
         "Failed": List[FailedCreateAssociationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAutomationExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationExecutionsResultTypeDef",
     {
         "AutomationExecutionMetadataList": List[AutomationExecutionMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAutomationExecutionResultTypeDef = TypedDict(
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/type_defs.pyi` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     "AssociationOverviewTypeDef",
     "AssociationStatusTypeDef",
     "TargetTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
@@ -122,267 +122,267 @@
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
+    "CancelMaintenanceWindowExecutionResultTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
     "NotificationConfigTypeDef",
     "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
+    "CreateActivationResultTypeDef",
     "DocumentRequiresTypeDef",
+    "CreateMaintenanceWindowResultTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
+    "CreateOpsItemResponseTypeDef",
     "MetadataValueTypeDef",
+    "CreateOpsMetadataResultTypeDef",
+    "CreatePatchBaselineResultTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
+    "DeleteMaintenanceWindowResultTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
     "DeleteParametersRequestRequestTypeDef",
+    "DeleteParametersResultTypeDef",
     "DeletePatchBaselineRequestRequestTypeDef",
+    "DeletePatchBaselineResultTypeDef",
     "DeleteResourceDataSyncRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeregisterManagedInstanceRequestRequestTypeDef",
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
     "DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     "DescribeActivationsFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "DescribeAssociationRequestRequestTypeDef",
     "StepExecutionFilterTypeDef",
     "PatchOrchestratorFilterTypeDef",
     "PatchTypeDef",
     "DescribeDocumentPermissionRequestRequestTypeDef",
     "DescribeDocumentRequestRequestTypeDef",
+    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     "InstanceAssociationTypeDef",
+    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
+    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
+    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
     "OpsItemFilterTypeDef",
     "ParameterStringFilterTypeDef",
     "ParametersFilterTypeDef",
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
+    "DescribePatchGroupStateResultTypeDef",
+    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
+    "DescribePatchPropertiesResultTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
+    "GetCalendarStateResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetCommandInvocationRequestRequestTypeDef",
     "GetConnectionStatusRequestRequestTypeDef",
+    "GetConnectionStatusResponseTypeDef",
     "GetDefaultPatchBaselineRequestRequestTypeDef",
+    "GetDefaultPatchBaselineResultTypeDef",
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
+    "GetMaintenanceWindowExecutionResultTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
+    "GetMaintenanceWindowResultTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
+    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
+    "GetPatchBaselineForPatchGroupResultTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
+    "LabelParameterVersionResultTypeDef",
+    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationVersionsRequestRequestTypeDef",
     "ListDocumentMetadataHistoryRequestRequestTypeDef",
+    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     "ListDocumentVersionsRequestRequestTypeDef",
+    "ListInventoryEntriesResultTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
     "MaintenanceWindowLambdaParametersTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterInlinePolicyTypeDef",
     "PatchFilterTypeDef",
+    "PutInventoryResultTypeDef",
+    "PutParameterResultTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
+    "RegisterDefaultPatchBaselineResultTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeSessionRequestRequestTypeDef",
+    "ResumeSessionResponseTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
+    "StartAutomationExecutionResultTypeDef",
+    "StartChangeRequestExecutionResultTypeDef",
     "StartSessionRequestRequestTypeDef",
+    "StartSessionResponseTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
+    "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionRequestRequestTypeDef",
+    "UnlabelParameterVersionResultTypeDef",
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     "UpdateMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowResultTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
+    "UpdateOpsMetadataResultTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
+    "DescribeDocumentPermissionResponseTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PutParameterRequestRequestTypeDef",
     "AlarmConfigurationTypeDef",
-    "AssociateOpsItemRelatedItemResponseTypeDef",
-    "CancelMaintenanceWindowExecutionResultTypeDef",
-    "CreateActivationResultTypeDef",
-    "CreateMaintenanceWindowResultTypeDef",
-    "CreateOpsItemResponseTypeDef",
-    "CreateOpsMetadataResultTypeDef",
-    "CreatePatchBaselineResultTypeDef",
-    "DeleteMaintenanceWindowResultTypeDef",
-    "DeleteParametersResultTypeDef",
-    "DeletePatchBaselineResultTypeDef",
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    "DescribeDocumentPermissionResponseTypeDef",
-    "DescribePatchGroupStateResultTypeDef",
-    "DescribePatchPropertiesResultTypeDef",
-    "GetCalendarStateResponseTypeDef",
-    "GetConnectionStatusResponseTypeDef",
-    "GetDefaultPatchBaselineResultTypeDef",
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    "GetMaintenanceWindowResultTypeDef",
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    "LabelParameterVersionResultTypeDef",
-    "ListInventoryEntriesResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PutInventoryResultTypeDef",
-    "PutParameterResultTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    "ResumeSessionResponseTypeDef",
-    "StartAutomationExecutionResultTypeDef",
-    "StartChangeRequestExecutionResultTypeDef",
-    "StartSessionResponseTypeDef",
-    "TerminateSessionResponseTypeDef",
-    "UnlabelParameterVersionResultTypeDef",
-    "UpdateMaintenanceWindowResultTypeDef",
-    "UpdateOpsMetadataResultTypeDef",
     "UpdateAssociationStatusRequestRequestTypeDef",
     "AssociationTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
     "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
     "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
+    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
+    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListAssociationsRequestRequestTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     "GetCommandInvocationResultTypeDef",
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
+    "ListCommandsRequestListCommandsPaginateTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
     "MaintenanceWindowRunCommandParametersTypeDef",
     "ComplianceItemTypeDef",
     "PutComplianceItemsRequestRequestTypeDef",
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
     "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
-    "DescribeActivationsRequestRequestTypeDef",
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
-    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    "DescribeActivationsRequestRequestTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
     "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
@@ -601,22 +601,19 @@
         "OpsItemId": str,
         "AssociationType": str,
         "ResourceType": str,
         "ResourceUri": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AssociationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociationOverviewTypeDef = TypedDict(
     "AssociationOverviewTypeDef",
     {
         "Status": str,
@@ -780,14 +777,22 @@
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
+CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "CancelMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
     },
     total=False,
@@ -899,14 +904,23 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateActivationResultTypeDef = TypedDict(
+    "CreateActivationResultTypeDef",
+    {
+        "ActivationId": str,
+        "ActivationCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDocumentRequiresTypeDef = TypedDict(
@@ -918,14 +932,22 @@
     },
     total=False,
 )
 
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
+CreateMaintenanceWindowResultTypeDef = TypedDict(
+    "CreateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -942,22 +964,47 @@
 RelatedOpsItemTypeDef = TypedDict(
     "RelatedOpsItemTypeDef",
     {
         "OpsItemId": str,
     },
 )
 
+CreateOpsItemResponseTypeDef = TypedDict(
+    "CreateOpsItemResponseTypeDef",
+    {
+        "OpsItemId": str,
+        "OpsItemArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetadataValueTypeDef = TypedDict(
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+CreateOpsMetadataResultTypeDef = TypedDict(
+    "CreateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePatchBaselineResultTypeDef = TypedDict(
+    "CreatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1016,14 +1063,22 @@
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
+DeleteMaintenanceWindowResultTypeDef = TypedDict(
+    "DeleteMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteOpsMetadataRequestRequestTypeDef = TypedDict(
     "DeleteOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 
@@ -1037,21 +1092,38 @@
 DeleteParametersRequestRequestTypeDef = TypedDict(
     "DeleteParametersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
+DeleteParametersResultTypeDef = TypedDict(
+    "DeleteParametersResultTypeDef",
+    {
+        "DeletedParameters": List[str],
+        "InvalidParameters": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePatchBaselineRequestRequestTypeDef = TypedDict(
     "DeletePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+DeletePatchBaselineResultTypeDef = TypedDict(
+    "DeletePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
@@ -1088,14 +1160,23 @@
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
+DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
@@ -1109,37 +1190,45 @@
 
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-DescribeActivationsFilterTypeDef = TypedDict(
-    "DescribeActivationsFilterTypeDef",
+DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     {
-        "FilterKey": DescribeActivationsFilterKeysType,
-        "FilterValues": Sequence[str],
+        "WindowId": str,
+        "WindowTaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeActivationsFilterTypeDef = TypedDict(
+    "DescribeActivationsFilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FilterKey": DescribeActivationsFilterKeysType,
+        "FilterValues": Sequence[str],
     },
     total=False,
 )
 
 DescribeAssociationRequestRequestTypeDef = TypedDict(
     "DescribeAssociationRequestRequestTypeDef",
     {
@@ -1236,14 +1325,34 @@
 )
 
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
+_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
+    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1268,14 +1377,34 @@
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
     },
     total=False,
 )
 
+_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "BaselineId": str,
+    },
+)
+_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
+    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
@@ -1289,14 +1418,34 @@
 
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
+    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1374,14 +1523,34 @@
 )
 
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
+_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+    },
+)
+_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
+    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1419,14 +1588,23 @@
 )
 
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
+DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    {
+        "DeletionId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1564,14 +1742,55 @@
 DescribePatchGroupStateRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupStateRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 
+DescribePatchGroupStateResultTypeDef = TypedDict(
+    "DescribePatchGroupStateResultTypeDef",
+    {
+        "Instances": int,
+        "InstancesWithInstalledPatches": int,
+        "InstancesWithInstalledOtherPatches": int,
+        "InstancesWithInstalledPendingRebootPatches": int,
+        "InstancesWithInstalledRejectedPatches": int,
+        "InstancesWithMissingPatches": int,
+        "InstancesWithFailedPatches": int,
+        "InstancesWithNotApplicablePatches": int,
+        "InstancesWithUnreportedNotApplicablePatches": int,
+        "InstancesWithCriticalNonCompliantPatches": int,
+        "InstancesWithSecurityNonCompliantPatches": int,
+        "InstancesWithOtherNonCompliantPatches": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "OperatingSystem": OperatingSystemType,
+        "Property": PatchPropertyType,
+    },
+)
+_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "PatchSet": PatchSetType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
+    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribePatchPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -1587,14 +1806,23 @@
 
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
+DescribePatchPropertiesResultTypeDef = TypedDict(
+    "DescribePatchPropertiesResultTypeDef",
+    {
+        "Properties": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1723,14 +1951,24 @@
 )
 
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
+GetCalendarStateResponseTypeDef = TypedDict(
+    "GetCalendarStateResponseTypeDef",
+    {
+        "State": CalendarStateType,
+        "AtTime": str,
+        "NextTransitionTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1760,22 +1998,51 @@
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
+GetConnectionStatusResponseTypeDef = TypedDict(
+    "GetConnectionStatusResponseTypeDef",
+    {
+        "Target": str,
+        "Status": ConnectionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetDefaultPatchBaselineRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
+GetDefaultPatchBaselineResultTypeDef = TypedDict(
+    "GetDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": str,
+        "SnapshotDownloadUrl": str,
+        "Product": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -1814,14 +2081,25 @@
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
+GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    {
+        "TypeName": str,
+        "Aggregator": bool,
+        "SubType": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetInventorySchemaRequestRequestTypeDef = TypedDict(
     "GetInventorySchemaRequestRequestTypeDef",
     {
         "TypeName": str,
         "NextToken": str,
         "MaxResults": int,
         "Aggregator": bool,
@@ -1833,23 +2111,55 @@
 GetMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
+GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskIds": List[str],
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "InvocationId": str,
     },
 )
 
+GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskExecutionId": str,
+        "InvocationId": str,
+        "ExecutionId": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "Parameters": str,
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "OwnerInformation": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMaintenanceWindowExecutionTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -1865,14 +2175,36 @@
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
+GetMaintenanceWindowResultTypeDef = TypedDict(
+    "GetMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "Name": str,
+        "Description": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "NextExecutionTime": str,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -1955,14 +2287,35 @@
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
+_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "WithDecryption": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
+    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetParameterHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterHistoryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterHistoryRequestRequestTypeDef = TypedDict(
@@ -2051,21 +2404,51 @@
 
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2218,14 +2601,43 @@
 
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
+LabelParameterVersionResultTypeDef = TypedDict(
+    "LabelParameterVersionResultTypeDef",
+    {
+        "InvalidLabels": List[str],
+        "ParameterVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
+    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2262,14 +2674,34 @@
 
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
+    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2283,14 +2715,27 @@
 
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListInventoryEntriesResultTypeDef = TypedDict(
+    "ListInventoryEntriesResultTypeDef",
+    {
+        "TypeName": str,
+        "InstanceId": str,
+        "SchemaVersion": str,
+        "CaptureTime": str,
+        "Entries": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2321,14 +2766,23 @@
         "LastModifiedDate": datetime,
         "LastModifiedUser": str,
         "CreationDate": datetime,
     },
     total=False,
 )
 
+ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    {
+        "SyncType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceDataSyncRequestRequestTypeDef = TypedDict(
     "ListResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2407,14 +2861,24 @@
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
     },
     total=False,
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
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
@@ -2425,14 +2889,31 @@
     "PatchFilterTypeDef",
     {
         "Key": PatchFilterKeyType,
         "Values": Sequence[str],
     },
 )
 
+PutInventoryResultTypeDef = TypedDict(
+    "PutInventoryResultTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutParameterResultTypeDef = TypedDict(
+    "PutParameterResultTypeDef",
+    {
+        "Version": int,
+        "Tier": ParameterTierType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
@@ -2446,29 +2927,71 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyHash": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
+RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
+RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    {
+        "WindowTargetId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
+    {
+        "WindowTaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -2493,21 +3016,42 @@
     "ResourceDataSyncDestinationDataSharingTypeDef",
     {
         "DestinationDataSharingType": str,
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
 ResumeSessionRequestRequestTypeDef = TypedDict(
     "ResumeSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+ResumeSessionResponseTypeDef = TypedDict(
+    "ResumeSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendAutomationSignalRequestRequestTypeDef = TypedDict(
     "_RequiredSendAutomationSignalRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
         "SignalType": SignalTypeType,
     },
 )
@@ -2537,14 +3081,30 @@
 StartAssociationsOnceRequestRequestTypeDef = TypedDict(
     "StartAssociationsOnceRequestRequestTypeDef",
     {
         "AssociationIds": Sequence[str],
     },
 )
 
+StartAutomationExecutionResultTypeDef = TypedDict(
+    "StartAutomationExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartChangeRequestExecutionResultTypeDef = TypedDict(
+    "StartChangeRequestExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 _OptionalStartSessionRequestRequestTypeDef = TypedDict(
@@ -2558,14 +3118,24 @@
 )
 
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
@@ -2585,23 +3155,40 @@
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UnlabelParameterVersionRequestRequestTypeDef = TypedDict(
     "UnlabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "ParameterVersion": int,
         "Labels": Sequence[str],
     },
 )
 
+UnlabelParameterVersionResultTypeDef = TypedDict(
+    "UnlabelParameterVersionResultTypeDef",
+    {
+        "RemovedLabels": List[str],
+        "InvalidLabels": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateDocumentDefaultVersionRequestRequestTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
     },
 )
@@ -2633,30 +3220,67 @@
 
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+UpdateMaintenanceWindowResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "Name": str,
+        "Description": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
 
+UpdateOpsMetadataResultTypeDef = TypedDict(
+    "UpdateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateServiceSettingRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
         "SettingValue": str,
     },
 )
 
+DescribeDocumentPermissionResponseTypeDef = TypedDict(
+    "DescribeDocumentPermissionResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ActivationTypeDef = TypedDict(
     "ActivationTypeDef",
     {
         "ActivationId": str,
         "Description": str,
         "DefaultInstanceName": str,
         "IamRole": str,
@@ -2705,14 +3329,22 @@
 
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -2752,434 +3384,14 @@
 )
 
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
-    "AssociateOpsItemRelatedItemResponseTypeDef",
-    {
-        "AssociationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "CancelMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateActivationResultTypeDef = TypedDict(
-    "CreateActivationResultTypeDef",
-    {
-        "ActivationId": str,
-        "ActivationCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMaintenanceWindowResultTypeDef = TypedDict(
-    "CreateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateOpsItemResponseTypeDef = TypedDict(
-    "CreateOpsItemResponseTypeDef",
-    {
-        "OpsItemId": str,
-        "OpsItemArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateOpsMetadataResultTypeDef = TypedDict(
-    "CreateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePatchBaselineResultTypeDef = TypedDict(
-    "CreatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMaintenanceWindowResultTypeDef = TypedDict(
-    "DeleteMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParametersResultTypeDef = TypedDict(
-    "DeleteParametersResultTypeDef",
-    {
-        "DeletedParameters": List[str],
-        "InvalidParameters": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePatchBaselineResultTypeDef = TypedDict(
-    "DeletePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDocumentPermissionResponseTypeDef = TypedDict(
-    "DescribeDocumentPermissionResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePatchGroupStateResultTypeDef = TypedDict(
-    "DescribePatchGroupStateResultTypeDef",
-    {
-        "Instances": int,
-        "InstancesWithInstalledPatches": int,
-        "InstancesWithInstalledOtherPatches": int,
-        "InstancesWithInstalledPendingRebootPatches": int,
-        "InstancesWithInstalledRejectedPatches": int,
-        "InstancesWithMissingPatches": int,
-        "InstancesWithFailedPatches": int,
-        "InstancesWithNotApplicablePatches": int,
-        "InstancesWithUnreportedNotApplicablePatches": int,
-        "InstancesWithCriticalNonCompliantPatches": int,
-        "InstancesWithSecurityNonCompliantPatches": int,
-        "InstancesWithOtherNonCompliantPatches": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePatchPropertiesResultTypeDef = TypedDict(
-    "DescribePatchPropertiesResultTypeDef",
-    {
-        "Properties": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCalendarStateResponseTypeDef = TypedDict(
-    "GetCalendarStateResponseTypeDef",
-    {
-        "State": CalendarStateType,
-        "AtTime": str,
-        "NextTransitionTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetConnectionStatusResponseTypeDef = TypedDict(
-    "GetConnectionStatusResponseTypeDef",
-    {
-        "Target": str,
-        "Status": ConnectionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDefaultPatchBaselineResultTypeDef = TypedDict(
-    "GetDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": str,
-        "SnapshotDownloadUrl": str,
-        "Product": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskIds": List[str],
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskExecutionId": str,
-        "InvocationId": str,
-        "ExecutionId": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "Parameters": str,
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "OwnerInformation": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMaintenanceWindowResultTypeDef = TypedDict(
-    "GetMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "NextExecutionTime": str,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LabelParameterVersionResultTypeDef = TypedDict(
-    "LabelParameterVersionResultTypeDef",
-    {
-        "InvalidLabels": List[str],
-        "ParameterVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListInventoryEntriesResultTypeDef = TypedDict(
-    "ListInventoryEntriesResultTypeDef",
-    {
-        "TypeName": str,
-        "InstanceId": str,
-        "SchemaVersion": str,
-        "CaptureTime": str,
-        "Entries": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutInventoryResultTypeDef = TypedDict(
-    "PutInventoryResultTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutParameterResultTypeDef = TypedDict(
-    "PutParameterResultTypeDef",
-    {
-        "Version": int,
-        "Tier": ParameterTierType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyHash": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTargetId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResumeSessionResponseTypeDef = TypedDict(
-    "ResumeSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAutomationExecutionResultTypeDef = TypedDict(
-    "StartAutomationExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartChangeRequestExecutionResultTypeDef = TypedDict(
-    "StartChangeRequestExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UnlabelParameterVersionResultTypeDef = TypedDict(
-    "UnlabelParameterVersionResultTypeDef",
-    {
-        "RemovedLabels": List[str],
-        "InvalidLabels": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMaintenanceWindowResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateOpsMetadataResultTypeDef = TypedDict(
-    "UpdateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
     "UpdateAssociationStatusRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationStatus": AssociationStatusTypeDef,
     },
@@ -3200,14 +3412,35 @@
         "AssociationName": str,
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     {
         "Targets": Sequence[TargetTypeDef],
         "ResourceType": MaintenanceWindowResourceTypeType,
     },
 )
@@ -3295,18 +3528,43 @@
     {
         "WindowId": str,
         "WindowTargetId": str,
         "Targets": List[TargetTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "AssociationId": str,
+        },
+    )
+)
+_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "Filters": Sequence[AssociationExecutionFilterTypeDef],
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
@@ -3337,14 +3595,36 @@
         "DetailedStatus": str,
         "LastExecutionDate": datetime,
         "OutputSource": OutputSourceTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "AssociationId": str,
+        "ExecutionId": str,
+    },
+)
+_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef",
     {
         "AssociationId": str,
         "ExecutionId": str,
     },
 )
@@ -3360,14 +3640,23 @@
 
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
+ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    {
+        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -3395,14 +3684,23 @@
 )
 
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
+DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    {
+        "Filters": Sequence[AutomationExecutionFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -3425,31 +3723,54 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "Details": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[CommandFilterTypeDef],
         "Details": bool,
     },
     total=False,
 )
 
+ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCommandsRequestRequestTypeDef = TypedDict(
     "ListCommandsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -3536,36 +3857,65 @@
 
 class PutComplianceItemsRequestRequestTypeDef(
     _RequiredPutComplianceItemsRequestRequestTypeDef,
     _OptionalPutComplianceItemsRequestRequestTypeDef,
 ):
     pass
 
+ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "ResourceIds": Sequence[str],
+        "ResourceTypes": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -3675,15 +4025,15 @@
         "StatusInformation": str,
         "Content": str,
         "DocumentType": DocumentTypeType,
         "DocumentFormat": DocumentFormatType,
         "Requires": List[DocumentRequiresTypeDef],
         "AttachmentsContent": List[AttachmentContentTypeDef],
         "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpsItemSummaryTypeDef = TypedDict(
     "OpsItemSummaryTypeDef",
     {
         "CreatedBy": str,
@@ -3824,15 +4174,15 @@
 
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
@@ -3848,379 +4198,29 @@
 )
 
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-DescribeActivationsRequestRequestTypeDef = TypedDict(
-    "DescribeActivationsRequestRequestTypeDef",
-    {
-        "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribeActivationsRequestDescribeActivationsPaginateTypeDef = TypedDict(
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "AssociationId": str,
-        "ExecutionId": str,
-    },
-)
-_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "AssociationId": str,
-        },
-    )
-)
-_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "Filters": Sequence[AssociationExecutionFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-):
-    pass
-
-DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    {
-        "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
-    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "BaselineId": str,
-    },
-)
-_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
-    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
-    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-    },
-)
-_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
-    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-):
-    pass
-
-DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    {
-        "DeletionId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-    },
-)
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "OperatingSystem": OperatingSystemType,
-        "Property": PatchPropertyType,
-    },
-)
-_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "PatchSet": PatchSetType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
-    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-):
-    pass
-
-GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    {
-        "TypeName": str,
-        "Aggregator": bool,
-        "SubType": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "WithDecryption": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
-    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
-    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-):
-    pass
-
-ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    {
-        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "Details": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "ResourceIds": Sequence[str],
-        "ResourceTypes": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
-    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+DescribeActivationsRequestRequestTypeDef = TypedDict(
+    "DescribeActivationsRequestRequestTypeDef",
     {
-        "SyncType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": Sequence[DescribeActivationsFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
@@ -4228,15 +4228,15 @@
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
@@ -4266,15 +4266,15 @@
 ):
     pass
 
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAvailablePatchesRequestRequestTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestRequestTypeDef",
     {
@@ -4291,15 +4291,15 @@
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
@@ -4332,15 +4332,15 @@
     TypedDict(
         "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
         {
             "WindowId": str,
             "Targets": Sequence[TargetTypeDef],
             "ResourceType": MaintenanceWindowResourceTypeType,
             "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
 DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
@@ -4355,15 +4355,15 @@
     total=False,
 )
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePatchBaselinesRequestRequestTypeDef = TypedDict(
     "DescribePatchBaselinesRequestRequestTypeDef",
     {
@@ -4374,15 +4374,15 @@
     total=False,
 )
 
 DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef = TypedDict(
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePatchGroupsRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupsRequestRequestTypeDef",
     {
@@ -4394,33 +4394,33 @@
 )
 
 DescribeAvailablePatchesResultTypeDef = TypedDict(
     "DescribeAvailablePatchesResultTypeDef",
     {
         "Patches": List[PatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEffectiveInstanceAssociationsResultTypeDef = TypedDict(
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     {
         "Associations": List[InstanceAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef = TypedDict(
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     {
         "InstanceInformationFilterList": Sequence[InstanceInformationFilterTypeDef],
         "Filters": Sequence[InstanceInformationStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeInstanceInformationRequestRequestTypeDef = TypedDict(
     "DescribeInstanceInformationRequestRequestTypeDef",
     {
@@ -4438,15 +4438,15 @@
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
@@ -4476,48 +4476,48 @@
     pass
 
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstancePatchStatesResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstancePatchesResultTypeDef = TypedDict(
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
@@ -4553,15 +4553,15 @@
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
@@ -4596,15 +4596,15 @@
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
@@ -4639,15 +4639,15 @@
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
@@ -4682,15 +4682,15 @@
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
@@ -4719,15 +4719,15 @@
 ):
     pass
 
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeMaintenanceWindowsRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestRequestTypeDef",
     {
@@ -4741,59 +4741,59 @@
 DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef",
     {
         "WindowExecutionTaskInvocationIdentities": List[
             MaintenanceWindowExecutionTaskInvocationIdentityTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowExecutionsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionsResultTypeDef",
     {
         "WindowExecutions": List[MaintenanceWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowScheduleResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleResultTypeDef",
     {
         "ScheduledWindowExecutions": List[ScheduledWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowsForTargetResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsForTargetResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityForTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef = TypedDict(
     "DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef",
     {
         "OpsItemFilters": Sequence[OpsItemFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeOpsItemsRequestRequestTypeDef = TypedDict(
     "DescribeOpsItemsRequestRequestTypeDef",
     {
@@ -4812,15 +4812,15 @@
 )
 _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef = TypedDict(
     "_OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef",
     {
         "Recursive": bool,
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
@@ -4852,15 +4852,15 @@
     pass
 
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeParametersRequestRequestTypeDef = TypedDict(
     "DescribeParametersRequestRequestTypeDef",
     {
@@ -4873,15 +4873,15 @@
 )
 
 DescribePatchBaselinesResultTypeDef = TypedDict(
     "DescribePatchBaselinesResultTypeDef",
     {
         "BaselineIdentities": List[PatchBaselineIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PatchGroupPatchBaselineMappingTypeDef = TypedDict(
     "PatchGroupPatchBaselineMappingTypeDef",
     {
         "PatchGroup": str,
@@ -4896,15 +4896,15 @@
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
         "Filters": Sequence[SessionFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
@@ -4932,15 +4932,15 @@
 ):
     pass
 
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
@@ -4978,15 +4978,15 @@
 )
 
 ListDocumentsRequestListDocumentsPaginateTypeDef = TypedDict(
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     {
         "DocumentFilterList": Sequence[DocumentFilterTypeDef],
         "Filters": Sequence[DocumentKeyValuesFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
@@ -5028,15 +5028,15 @@
     pass
 
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EffectivePatchTypeDef = TypedDict(
     "EffectivePatchTypeDef",
     {
         "Patch": PatchTypeDef,
@@ -5100,15 +5100,15 @@
 
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetInventoryRequestRequestTypeDef = TypedDict(
     "GetInventoryRequestRequestTypeDef",
     {
@@ -5137,15 +5137,15 @@
 GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef = TypedDict(
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     {
         "SyncName": str,
         "Filters": Sequence[OpsFilterTypeDef],
         "Aggregators": Sequence["OpsAggregatorTypeDef"],
         "ResultAttributes": Sequence[OpsResultAttributeTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetOpsSummaryRequestRequestTypeDef = TypedDict(
     "GetOpsSummaryRequestRequestTypeDef",
     {
@@ -5159,58 +5159,58 @@
     total=False,
 )
 
 GetParameterResultTypeDef = TypedDict(
     "GetParameterResultTypeDef",
     {
         "Parameter": ParameterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParametersByPathResultTypeDef = TypedDict(
     "GetParametersByPathResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParametersResultTypeDef = TypedDict(
     "GetParametersResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceSettingResultTypeDef = TypedDict(
     "GetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetServiceSettingResultTypeDef = TypedDict(
     "ResetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceInformationTypeDef = TypedDict(
     "InstanceInformationTypeDef",
     {
         "InstanceId": str,
@@ -5302,15 +5302,15 @@
     total=False,
 )
 
 ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef = TypedDict(
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     {
         "Filters": Sequence[OpsItemEventFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOpsItemEventsRequestRequestTypeDef = TypedDict(
     "ListOpsItemEventsRequestRequestTypeDef",
     {
@@ -5322,15 +5322,15 @@
 )
 
 ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     {
         "OpsItemId": str,
         "Filters": Sequence[OpsItemRelatedItemsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOpsItemRelatedItemsRequestRequestTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     {
@@ -5342,15 +5342,15 @@
     total=False,
 )
 
 ListOpsMetadataRequestListOpsMetadataPaginateTypeDef = TypedDict(
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     {
         "Filters": Sequence[OpsMetadataFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOpsMetadataRequestRequestTypeDef = TypedDict(
     "ListOpsMetadataRequestRequestTypeDef",
     {
@@ -5362,15 +5362,15 @@
 )
 
 ListOpsMetadataResultTypeDef = TypedDict(
     "ListOpsMetadataResultTypeDef",
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
@@ -5516,15 +5516,15 @@
 )
 
 DescribeActivationsResultTypeDef = TypedDict(
     "DescribeActivationsResultTypeDef",
     {
         "ActivationList": List[ActivationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociationExecutionTypeDef = TypedDict(
     "AssociationExecutionTypeDef",
     {
         "AssociationId": str,
@@ -5588,15 +5588,15 @@
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     {
         "WindowExecutionId": str,
@@ -5684,42 +5684,42 @@
 )
 
 ListAssociationsResultTypeDef = TypedDict(
     "ListAssociationsResultTypeDef",
     {
         "Associations": List[AssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowTargetsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     {
         "Targets": List[MaintenanceWindowTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssociationExecutionTargetsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionTargetsResultTypeDef",
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
     "MaintenanceWindowTaskInvocationParametersTypeDef",
     {
         "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
@@ -5731,15 +5731,15 @@
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
         "ComplianceItems": List[ComplianceItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComplianceSummaryItemTypeDef = TypedDict(
     "ComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
@@ -5765,65 +5765,65 @@
 )
 
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOpsItemsResponseTypeDef = TypedDict(
     "DescribeOpsItemsResponseTypeDef",
     {
         "NextToken": str,
         "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOpsItemResponseTypeDef = TypedDict(
     "GetOpsItemResponseTypeDef",
     {
         "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePatchGroupsResultTypeDef = TypedDict(
     "DescribePatchGroupsResultTypeDef",
     {
         "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDocumentResultTypeDef = TypedDict(
     "DescribeDocumentResultTypeDef",
     {
         "Document": DocumentDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDocumentResultTypeDef = TypedDict(
     "UpdateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentMetadataResponseInfoTypeDef = TypedDict(
     "DocumentMetadataResponseInfoTypeDef",
     {
         "ReviewerResponse": List[DocumentReviewerResponseSourceTypeDef],
@@ -5853,15 +5853,15 @@
     pass
 
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InventoryAggregatorTypeDef = TypedDict(
     "InventoryAggregatorTypeDef",
     {
         "Expression": str,
@@ -5872,15 +5872,15 @@
 )
 
 DescribeInstanceInformationResultTypeDef = TypedDict(
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": str,
@@ -5901,15 +5901,15 @@
 
 DeleteInventoryResultTypeDef = TypedDict(
     "DeleteInventoryResultTypeDef",
     {
         "DeletionId": str,
         "TypeName": str,
         "DeletionSummary": InventoryDeletionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InventoryDeletionStatusItemTypeDef = TypedDict(
     "InventoryDeletionStatusItemTypeDef",
     {
         "DeletionId": str,
@@ -5924,69 +5924,69 @@
 )
 
 GetInventorySchemaResultTypeDef = TypedDict(
     "GetInventorySchemaResultTypeDef",
     {
         "Schemas": List[InventoryItemSchemaTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInventoryResultTypeDef = TypedDict(
     "GetInventoryResultTypeDef",
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOpsItemRelatedItemsResponseTypeDef = TypedDict(
     "ListOpsItemRelatedItemsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParametersResultTypeDef = TypedDict(
     "DescribeParametersResultTypeDef",
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
@@ -6042,59 +6042,59 @@
 )
 
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssociationExecutionsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionsResultTypeDef",
     {
         "AssociationExecutions": List[AssociationExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCommandsResultTypeDef = TypedDict(
     "ListCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "Command": CommandTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowExecutionTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     {
         "WindowExecutionTaskIdentities": List[MaintenanceWindowExecutionTaskIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMaintenanceWindowTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTasksResultTypeDef",
     {
         "Tasks": List[MaintenanceWindowTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociationDescriptionTypeDef = TypedDict(
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
@@ -6366,15 +6366,15 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
@@ -6456,63 +6456,63 @@
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListComplianceSummariesResultTypeDef = TypedDict(
     "ListComplianceSummariesResultTypeDef",
     {
         "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceComplianceSummariesResultTypeDef = TypedDict(
     "ListResourceComplianceSummariesResultTypeDef",
     {
         "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
     "ListDocumentMetadataHistoryResponseTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
         "Author": str,
         "Metadata": DocumentMetadataResponseInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
     "DescribeInstanceAssociationsStatusResultTypeDef",
     {
         "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInventoryDeletionsResultTypeDef = TypedDict(
     "DescribeInventoryDeletionsResultTypeDef",
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PatchRuleGroupTypeDef = TypedDict(
     "PatchRuleGroupTypeDef",
     {
         "PatchRules": Sequence[PatchRuleTypeDef],
@@ -6567,48 +6567,48 @@
     total=False,
 )
 
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAssociationResultTypeDef = TypedDict(
     "DescribeAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssociationResultTypeDef = TypedDict(
     "UpdateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssociationStatusResultTypeDef = TypedDict(
     "UpdateAssociationStatusResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssociationVersionsResultTypeDef = TypedDict(
     "ListAssociationVersionsResultTypeDef",
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssociationBatchRequestRequestTypeDef = TypedDict(
     "CreateAssociationBatchRequestRequestTypeDef",
     {
         "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
@@ -6732,15 +6732,15 @@
 )
 
 DescribeAutomationStepExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationStepExecutionsResultTypeDef",
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
@@ -6801,15 +6801,15 @@
         "RejectedPatches": List[str],
         "RejectedPatchesAction": PatchActionType,
         "PatchGroups": List[str],
         "CreatedDate": datetime,
         "ModifiedDate": datetime,
         "Description": str,
         "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
@@ -6852,50 +6852,50 @@
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": List[str],
         "RejectedPatchesAction": PatchActionType,
         "CreatedDate": datetime,
         "ModifiedDate": datetime,
         "Description": str,
         "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssociationBatchResultTypeDef = TypedDict(
     "CreateAssociationBatchResultTypeDef",
     {
         "Successful": List[AssociationDescriptionTypeDef],
         "Failed": List[FailedCreateAssociationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAutomationExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationExecutionsResultTypeDef",
     {
         "AutomationExecutionMetadataList": List[AutomationExecutionMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAutomationExecutionResultTypeDef = TypedDict(
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
```

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.py` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm/waiter.pyi` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.26.97
-Summary: Type annotations for boto3.SSM 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SSM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ssm"></a>
 
 # mypy-boto3-ssm
 
 [![PyPI - mypy-boto3-ssm](https://img.shields.io/pypi/v/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -647,15 +647,15 @@
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationOverviewTypeDef,
     AssociationStatusTypeDef,
     TargetTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
@@ -664,267 +664,267 @@
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
+    CreateActivationResultTypeDef,
     DocumentRequiresTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
+    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
+    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
+    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
+    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
+    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
+    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
+    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
     LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
+    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
+    PaginatorConfigTypeDef,
     ParameterInlinePolicyTypeDef,
     PatchFilterTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
+    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
+    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
+    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
+    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
+    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
+    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
     AlarmConfigurationTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
-    CreateActivationResultTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
-    CreateOpsItemResponseTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
-    DeleteParametersResultTypeDef,
-    DeletePatchBaselineResultTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesResultTypeDef,
-    GetCalendarStateResponseTypeDef,
-    GetConnectionStatusResponseTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
-    GetMaintenanceWindowResultTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListInventoryEntriesResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
-    ResumeSessionResponseTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
-    StartSessionResponseTypeDef,
-    TerminateSessionResponseTypeDef,
-    UnlabelParameterVersionResultTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateAssociationStatusRequestRequestTypeDef,
     AssociationTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
     DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
     RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
     UpdateDocumentRequestRequestTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
     GetCommandInvocationResultTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
     ComplianceItemTypeDef,
     PutComplianceItemsRequestRequestTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
     GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestRequestTypeDef,
     DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
+    DescribeActivationsRequestRequestTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
     DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
@@ -1113,42 +1113,42 @@
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

### Comparing `mypy-boto3-ssm-1.26.97/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy-boto3-ssm-1.27.0/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.26.97/setup.py` & `mypy-boto3-ssm-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-ssm.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.26.97",
+    version="1.27.0",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSM 1.26.97 service generated with mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.SSM 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/",
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


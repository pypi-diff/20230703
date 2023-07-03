# Comparing `tmp/mypy-boto3-emr-1.26.73.tar.gz` & `tmp/mypy-boto3-emr-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.26.73.tar", last modified: Thu Feb 16 20:47:25 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
```

## Comparing `mypy-boto3-emr-1.26.73.tar` & `mypy-boto3-emr-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22052 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42800 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42727 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-02-16 20:47:03.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-02-16 20:47:03.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-02-16 20:47:05.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    76197 2023-02-16 20:47:04.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-16 20:47:25.000000 mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:47:25.471045 mypy-boto3-emr-1.26.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-16 20:47:02.000000 mypy-boto3-emr-1.26.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-03 19:37:27.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79659 2023-07-03 19:37:29.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79553 2023-07-03 19:37:29.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/setup.py
```

### Comparing `mypy-boto3-emr-1.26.73/LICENSE` & `mypy-boto3-emr-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-emr-1.26.73/PKG-INFO` & `mypy-boto3-emr-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.26.73
-Summary: Type annotations for boto3.EMR 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EMR 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,14 +389,15 @@
     ListStudioSessionMappingsPaginatorName,
     ListStudiosPaginatorName,
     MarketTypeType,
     NotebookExecutionStatusType,
     OnDemandCapacityReservationPreferenceType,
     OnDemandCapacityReservationUsageStrategyType,
     OnDemandProvisioningAllocationStrategyType,
+    OutputNotebookFormatType,
     PlacementGroupStrategyType,
     ReconfigurationTypeType,
     RepoUpgradeOnBootType,
     ScaleDownBehaviorType,
     SpotProvisioningAllocationStrategyType,
     SpotProvisioningTimeoutActionType,
     StatisticType,
@@ -424,52 +425,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
-    ResponseMetadataTypeDef,
+    AddInstanceFleetOutputTypeDef,
+    AddInstanceGroupsOutputTypeDef,
+    AddJobFlowStepsOutputTypeDef,
     TagTypeDef,
     ApplicationTypeDef,
     ScalingConstraintsTypeDef,
     AutoScalingPolicyStateChangeReasonTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
     PortRangeTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
+    ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
     KerberosAttributesTypeDef,
     PlacementGroupConfigTypeDef,
     CommandTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
+    CreateSecurityConfigurationOutputTypeDef,
+    CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
     DescribeJobFlowsInputRequestTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
+    DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
     EbsVolumeTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
@@ -484,58 +492,67 @@
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
-    PaginatorConfigTypeDef,
+    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
+    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
+    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
+    ListInstancesInputListInstancesPaginateTypeDef,
     ListInstancesInputRequestTypeDef,
+    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
     ListNotebookExecutionsInputRequestTypeDef,
-    NotebookExecutionSummaryTypeDef,
     ReleaseLabelFilterTypeDef,
+    ListReleaseLabelsOutputTypeDef,
+    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
+    ListStepsInputListStepsPaginateTypeDef,
     ListStepsInputRequestTypeDef,
+    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
+    ListStudiosInputListStudiosPaginateTypeDef,
     ListStudiosInputRequestTypeDef,
     StudioSummaryTypeDef,
+    ListSupportedInstanceTypesInputRequestTypeDef,
+    SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
+    ModifyClusterOutputTypeDef,
+    NotebookS3LocationForOutputTypeDef,
+    OutputNotebookS3LocationForOutputTypeDef,
+    NotebookS3LocationFromInputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
+    OutputNotebookS3LocationFromInputTypeDef,
+    PaginatorConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
+    RunJobFlowOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
+    StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
-    AddInstanceFleetOutputTypeDef,
-    AddInstanceGroupsOutputTypeDef,
-    AddJobFlowStepsOutputTypeDef,
-    CreateSecurityConfigurationOutputTypeDef,
-    CreateStudioOutputTypeDef,
-    DescribeSecurityConfigurationOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListReleaseLabelsOutputTypeDef,
-    ModifyClusterOutputTypeDef,
-    RunJobFlowOutputTypeDef,
-    StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
     StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationTypeDef,
@@ -548,59 +565,51 @@
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
-    NotebookExecutionTypeDef,
-    StartNotebookExecutionInputRequestTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
-    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
-    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    ListInstancesInputListInstancesPaginateTypeDef,
-    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
-    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
-    ListStepsInputListStepsPaginateTypeDef,
-    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
-    ListStudiosInputListStudiosPaginateTypeDef,
-    ListNotebookExecutionsOutputTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
+    ListSupportedInstanceTypesOutputTypeDef,
+    NotebookExecutionSummaryTypeDef,
+    NotebookExecutionTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
+    StartNotebookExecutionInputRequestTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
     DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
-    DescribeNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
+    ListNotebookExecutionsOutputTypeDef,
+    DescribeNotebookExecutionOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
@@ -626,53 +635,53 @@
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> AddInstanceFleetOutputTypeDef:
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

### Comparing `mypy-boto3-emr-1.26.73/README.md` & `mypy-boto3-emr-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,14 +357,15 @@
     ListStudioSessionMappingsPaginatorName,
     ListStudiosPaginatorName,
     MarketTypeType,
     NotebookExecutionStatusType,
     OnDemandCapacityReservationPreferenceType,
     OnDemandCapacityReservationUsageStrategyType,
     OnDemandProvisioningAllocationStrategyType,
+    OutputNotebookFormatType,
     PlacementGroupStrategyType,
     ReconfigurationTypeType,
     RepoUpgradeOnBootType,
     ScaleDownBehaviorType,
     SpotProvisioningAllocationStrategyType,
     SpotProvisioningTimeoutActionType,
     StatisticType,
@@ -392,52 +393,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
-    ResponseMetadataTypeDef,
+    AddInstanceFleetOutputTypeDef,
+    AddInstanceGroupsOutputTypeDef,
+    AddJobFlowStepsOutputTypeDef,
     TagTypeDef,
     ApplicationTypeDef,
     ScalingConstraintsTypeDef,
     AutoScalingPolicyStateChangeReasonTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
     PortRangeTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
+    ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
     KerberosAttributesTypeDef,
     PlacementGroupConfigTypeDef,
     CommandTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
+    CreateSecurityConfigurationOutputTypeDef,
+    CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
     DescribeJobFlowsInputRequestTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
+    DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
     EbsVolumeTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
@@ -452,58 +460,67 @@
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
-    PaginatorConfigTypeDef,
+    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
+    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
+    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
+    ListInstancesInputListInstancesPaginateTypeDef,
     ListInstancesInputRequestTypeDef,
+    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
     ListNotebookExecutionsInputRequestTypeDef,
-    NotebookExecutionSummaryTypeDef,
     ReleaseLabelFilterTypeDef,
+    ListReleaseLabelsOutputTypeDef,
+    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
+    ListStepsInputListStepsPaginateTypeDef,
     ListStepsInputRequestTypeDef,
+    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
+    ListStudiosInputListStudiosPaginateTypeDef,
     ListStudiosInputRequestTypeDef,
     StudioSummaryTypeDef,
+    ListSupportedInstanceTypesInputRequestTypeDef,
+    SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
+    ModifyClusterOutputTypeDef,
+    NotebookS3LocationForOutputTypeDef,
+    OutputNotebookS3LocationForOutputTypeDef,
+    NotebookS3LocationFromInputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
+    OutputNotebookS3LocationFromInputTypeDef,
+    PaginatorConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
+    RunJobFlowOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
+    StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
-    AddInstanceFleetOutputTypeDef,
-    AddInstanceGroupsOutputTypeDef,
-    AddJobFlowStepsOutputTypeDef,
-    CreateSecurityConfigurationOutputTypeDef,
-    CreateStudioOutputTypeDef,
-    DescribeSecurityConfigurationOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListReleaseLabelsOutputTypeDef,
-    ModifyClusterOutputTypeDef,
-    RunJobFlowOutputTypeDef,
-    StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
     StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationTypeDef,
@@ -516,59 +533,51 @@
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
-    NotebookExecutionTypeDef,
-    StartNotebookExecutionInputRequestTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
-    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
-    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    ListInstancesInputListInstancesPaginateTypeDef,
-    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
-    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
-    ListStepsInputListStepsPaginateTypeDef,
-    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
-    ListStudiosInputListStudiosPaginateTypeDef,
-    ListNotebookExecutionsOutputTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
+    ListSupportedInstanceTypesOutputTypeDef,
+    NotebookExecutionSummaryTypeDef,
+    NotebookExecutionTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
+    StartNotebookExecutionInputRequestTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
     DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
-    DescribeNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
+    ListNotebookExecutionsOutputTypeDef,
+    DescribeNotebookExecutionOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
@@ -594,53 +603,53 @@
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> AddInstanceFleetOutputTypeDef:
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

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.26.73\nVersion:         1.26.73\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.EMR 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.73")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,19 @@
     ListInstancesOutputTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     ListReleaseLabelsOutputTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStepsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
+    ListSupportedInstanceTypesOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     ModifyClusterOutputTypeDef,
+    NotebookS3LocationFromInputTypeDef,
+    OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
     SupportedProductConfigTypeDef,
@@ -252,15 +255,15 @@
         StudioId: str,
         IdentityType: IdentityTypeType,
         SessionPolicyArn: str,
         IdentityId: str = ...,
         IdentityName: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Maps a user or group to the Amazon EMR Studio specified by `StudioId` , and
+        Maps a user or group to the Amazon EMR Studio specified by `StudioId`, and
         applies a session policy to refine Studio permissions for that user or group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio_session_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#create_studio_session_mapping)
         """
 
     def delete_security_configuration(self, *, Name: str) -> Dict[str, Any]:
@@ -328,17 +331,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#describe_notebook_execution)
         """
 
     def describe_release_label(
         self, *, ReleaseLabel: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeReleaseLabelOutputTypeDef:
         """
-        Provides EMR release label details, such as releases available the region where
-        the API request is run, and the available applications for a specific EMR
-        release label.
+        Provides Amazon EMR release label details, such as the releases available the
+        Region where the API request is run, and the available applications for a
+        specific Amazon EMR release label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_release_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#describe_release_label)
         """
 
     def describe_security_configuration(
         self, *, Name: str
@@ -492,29 +495,30 @@
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
         Marker: str = ...
     ) -> ListInstancesOutputTypeDef:
         """
-        Provides information for all active EC2 instances and EC2 instances terminated
-        in the last 30 days, up to a maximum of 2,000.
+        Provides information for all active Amazon EC2 instances and Amazon EC2
+        instances terminated in the last 30 days, up to a maximum of 2,000.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_instances)
         """
 
     def list_notebook_executions(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: Union[datetime, str] = ...,
         To: Union[datetime, str] = ...,
-        Marker: str = ...
+        Marker: str = ...,
+        ExecutionEngineId: str = ...
     ) -> ListNotebookExecutionsOutputTypeDef:
         """
         Provides summaries of all notebook executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_notebook_executions)
         """
@@ -523,15 +527,16 @@
         self,
         *,
         Filters: ReleaseLabelFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReleaseLabelsOutputTypeDef:
         """
-        Retrieves release labels of EMR services in the region where the API is called.
+        Retrieves release labels of Amazon EMR services in the Region where the API is
+        called.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_release_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_release_labels)
         """
 
     def list_security_configurations(
         self, *, Marker: str = ...
@@ -561,29 +566,39 @@
         """
 
     def list_studio_session_mappings(
         self, *, StudioId: str = ..., IdentityType: IdentityTypeType = ..., Marker: str = ...
     ) -> ListStudioSessionMappingsOutputTypeDef:
         """
         Returns a list of all user or group session mappings for the Amazon EMR Studio
-        specified by `StudioId` .
+        specified by `StudioId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_studio_session_mappings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_studio_session_mappings)
         """
 
     def list_studios(self, *, Marker: str = ...) -> ListStudiosOutputTypeDef:
         """
         Returns a list of all Amazon EMR Studios associated with the Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_studios)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_studios)
         """
 
+    def list_supported_instance_types(
+        self, *, ReleaseLabel: str, Marker: str = ...
+    ) -> ListSupportedInstanceTypesOutputTypeDef:
+        """
+        A list of the instance types that Amazon EMR supports.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_supported_instance_types)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_supported_instance_types)
+        """
+
     def modify_cluster(
         self, *, ClusterId: str, StepConcurrencyLevel: int = ...
     ) -> ModifyClusterOutputTypeDef:
         """
         Modifies the number of steps that can be executed concurrently for the cluster
         specified using ClusterID.
 
@@ -657,15 +672,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_managed_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_managed_scaling_policy)
         """
 
     def remove_auto_scaling_policy(self, *, ClusterId: str, InstanceGroupId: str) -> Dict[str, Any]:
         """
         Removes an automatic scaling policy from a specified instance group within an
-        EMR cluster.
+        Amazon EMR cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_auto_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#remove_auto_scaling_policy)
         """
 
     def remove_auto_termination_policy(self, *, ClusterId: str) -> Dict[str, Any]:
         """
@@ -673,15 +688,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_auto_termination_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#remove_auto_termination_policy)
         """
 
     def remove_managed_scaling_policy(self, *, ClusterId: str) -> Dict[str, Any]:
         """
-        Removes a managed scaling policy from a specified EMR cluster.
+        Removes a managed scaling policy from a specified Amazon EMR cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_managed_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#remove_managed_scaling_policy)
         """
 
     def remove_tags(self, *, ResourceId: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
@@ -732,17 +747,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#run_job_flow)
         """
 
     def set_termination_protection(
         self, *, JobFlowIds: Sequence[str], TerminationProtected: bool
     ) -> EmptyResponseMetadataTypeDef:
         """
-        SetTerminationProtection locks a cluster (job flow) so the EC2 instances in the
-        cluster cannot be terminated by user intervention, an API call, or in the event
-        of a job-flow error.
+        SetTerminationProtection locks a cluster (job flow) so the Amazon EC2 instances
+        in the cluster cannot be terminated by user intervention, an API call, or in the
+        event of a job-flow error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_termination_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_termination_protection)
         """
 
     def set_visible_to_all_users(
         self, *, JobFlowIds: Sequence[str], VisibleToAllUsers: bool
@@ -753,22 +768,26 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_visible_to_all_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_visible_to_all_users)
         """
 
     def start_notebook_execution(
         self,
         *,
-        EditorId: str,
-        RelativePath: str,
         ExecutionEngine: ExecutionEngineConfigTypeDef,
         ServiceRole: str,
+        EditorId: str = ...,
+        RelativePath: str = ...,
         NotebookExecutionName: str = ...,
         NotebookParams: str = ...,
         NotebookInstanceSecurityGroupId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        NotebookS3Location: NotebookS3LocationFromInputTypeDef = ...,
+        OutputNotebookS3Location: OutputNotebookS3LocationFromInputTypeDef = ...,
+        OutputNotebookFormat: Literal["HTML"] = ...,
+        EnvironmentVariables: Mapping[str, str] = ...
     ) -> StartNotebookExecutionOutputTypeDef:
         """
         Starts a notebook execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.start_notebook_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#start_notebook_execution)
         """
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,19 @@
     ListInstancesOutputTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     ListReleaseLabelsOutputTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStepsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
+    ListSupportedInstanceTypesOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     ModifyClusterOutputTypeDef,
+    NotebookS3LocationFromInputTypeDef,
+    OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
     SupportedProductConfigTypeDef,
@@ -238,15 +241,15 @@
         StudioId: str,
         IdentityType: IdentityTypeType,
         SessionPolicyArn: str,
         IdentityId: str = ...,
         IdentityName: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Maps a user or group to the Amazon EMR Studio specified by `StudioId` , and
+        Maps a user or group to the Amazon EMR Studio specified by `StudioId`, and
         applies a session policy to refine Studio permissions for that user or group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.create_studio_session_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#create_studio_session_mapping)
         """
     def delete_security_configuration(self, *, Name: str) -> Dict[str, Any]:
         """
@@ -307,17 +310,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_notebook_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#describe_notebook_execution)
         """
     def describe_release_label(
         self, *, ReleaseLabel: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeReleaseLabelOutputTypeDef:
         """
-        Provides EMR release label details, such as releases available the region where
-        the API request is run, and the available applications for a specific EMR
-        release label.
+        Provides Amazon EMR release label details, such as the releases available the
+        Region where the API request is run, and the available applications for a
+        specific Amazon EMR release label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.describe_release_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#describe_release_label)
         """
     def describe_security_configuration(
         self, *, Name: str
     ) -> DescribeSecurityConfigurationOutputTypeDef:
@@ -457,28 +460,29 @@
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
         Marker: str = ...
     ) -> ListInstancesOutputTypeDef:
         """
-        Provides information for all active EC2 instances and EC2 instances terminated
-        in the last 30 days, up to a maximum of 2,000.
+        Provides information for all active Amazon EC2 instances and Amazon EC2
+        instances terminated in the last 30 days, up to a maximum of 2,000.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_instances)
         """
     def list_notebook_executions(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: Union[datetime, str] = ...,
         To: Union[datetime, str] = ...,
-        Marker: str = ...
+        Marker: str = ...,
+        ExecutionEngineId: str = ...
     ) -> ListNotebookExecutionsOutputTypeDef:
         """
         Provides summaries of all notebook executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_notebook_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_notebook_executions)
         """
@@ -486,15 +490,16 @@
         self,
         *,
         Filters: ReleaseLabelFilterTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReleaseLabelsOutputTypeDef:
         """
-        Retrieves release labels of EMR services in the region where the API is called.
+        Retrieves release labels of Amazon EMR services in the Region where the API is
+        called.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_release_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_release_labels)
         """
     def list_security_configurations(
         self, *, Marker: str = ...
     ) -> ListSecurityConfigurationsOutputTypeDef:
@@ -521,27 +526,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_steps)
         """
     def list_studio_session_mappings(
         self, *, StudioId: str = ..., IdentityType: IdentityTypeType = ..., Marker: str = ...
     ) -> ListStudioSessionMappingsOutputTypeDef:
         """
         Returns a list of all user or group session mappings for the Amazon EMR Studio
-        specified by `StudioId` .
+        specified by `StudioId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_studio_session_mappings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_studio_session_mappings)
         """
     def list_studios(self, *, Marker: str = ...) -> ListStudiosOutputTypeDef:
         """
         Returns a list of all Amazon EMR Studios associated with the Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_studios)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_studios)
         """
+    def list_supported_instance_types(
+        self, *, ReleaseLabel: str, Marker: str = ...
+    ) -> ListSupportedInstanceTypesOutputTypeDef:
+        """
+        A list of the instance types that Amazon EMR supports.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.list_supported_instance_types)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#list_supported_instance_types)
+        """
     def modify_cluster(
         self, *, ClusterId: str, StepConcurrencyLevel: int = ...
     ) -> ModifyClusterOutputTypeDef:
         """
         Modifies the number of steps that can be executed concurrently for the cluster
         specified using ClusterID.
 
@@ -608,29 +622,29 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_managed_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#put_managed_scaling_policy)
         """
     def remove_auto_scaling_policy(self, *, ClusterId: str, InstanceGroupId: str) -> Dict[str, Any]:
         """
         Removes an automatic scaling policy from a specified instance group within an
-        EMR cluster.
+        Amazon EMR cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_auto_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#remove_auto_scaling_policy)
         """
     def remove_auto_termination_policy(self, *, ClusterId: str) -> Dict[str, Any]:
         """
         Removes an auto-termination policy from an Amazon EMR cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_auto_termination_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#remove_auto_termination_policy)
         """
     def remove_managed_scaling_policy(self, *, ClusterId: str) -> Dict[str, Any]:
         """
-        Removes a managed scaling policy from a specified EMR cluster.
+        Removes a managed scaling policy from a specified Amazon EMR cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.remove_managed_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#remove_managed_scaling_policy)
         """
     def remove_tags(self, *, ResourceId: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an Amazon EMR resource, such as a cluster or Amazon EMR
@@ -678,17 +692,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.run_job_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#run_job_flow)
         """
     def set_termination_protection(
         self, *, JobFlowIds: Sequence[str], TerminationProtected: bool
     ) -> EmptyResponseMetadataTypeDef:
         """
-        SetTerminationProtection locks a cluster (job flow) so the EC2 instances in the
-        cluster cannot be terminated by user intervention, an API call, or in the event
-        of a job-flow error.
+        SetTerminationProtection locks a cluster (job flow) so the Amazon EC2 instances
+        in the cluster cannot be terminated by user intervention, an API call, or in the
+        event of a job-flow error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_termination_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_termination_protection)
         """
     def set_visible_to_all_users(
         self, *, JobFlowIds: Sequence[str], VisibleToAllUsers: bool
     ) -> EmptyResponseMetadataTypeDef:
@@ -697,22 +711,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_visible_to_all_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_visible_to_all_users)
         """
     def start_notebook_execution(
         self,
         *,
-        EditorId: str,
-        RelativePath: str,
         ExecutionEngine: ExecutionEngineConfigTypeDef,
         ServiceRole: str,
+        EditorId: str = ...,
+        RelativePath: str = ...,
         NotebookExecutionName: str = ...,
         NotebookParams: str = ...,
         NotebookInstanceSecurityGroupId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        NotebookS3Location: NotebookS3LocationFromInputTypeDef = ...,
+        OutputNotebookS3Location: OutputNotebookS3LocationFromInputTypeDef = ...,
+        OutputNotebookFormat: Literal["HTML"] = ...,
+        EnvironmentVariables: Mapping[str, str] = ...
     ) -> StartNotebookExecutionOutputTypeDef:
         """
         Starts a notebook execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.start_notebook_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#start_notebook_execution)
         """
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     "ListStudioSessionMappingsPaginatorName",
     "ListStudiosPaginatorName",
     "MarketTypeType",
     "NotebookExecutionStatusType",
     "OnDemandCapacityReservationPreferenceType",
     "OnDemandCapacityReservationUsageStrategyType",
     "OnDemandProvisioningAllocationStrategyType",
+    "OutputNotebookFormatType",
     "PlacementGroupStrategyType",
     "ReconfigurationTypeType",
     "RepoUpgradeOnBootType",
     "ScaleDownBehaviorType",
     "SpotProvisioningAllocationStrategyType",
     "SpotProvisioningTimeoutActionType",
     "StatisticType",
@@ -189,19 +190,22 @@
     "STOPPED",
     "STOPPING",
     "STOP_PENDING",
 ]
 OnDemandCapacityReservationPreferenceType = Literal["none", "open"]
 OnDemandCapacityReservationUsageStrategyType = Literal["use-capacity-reservations-first"]
 OnDemandProvisioningAllocationStrategyType = Literal["lowest-price"]
+OutputNotebookFormatType = Literal["HTML"]
 PlacementGroupStrategyType = Literal["CLUSTER", "NONE", "PARTITION", "SPREAD"]
 ReconfigurationTypeType = Literal["MERGE", "OVERWRITE"]
 RepoUpgradeOnBootType = Literal["NONE", "SECURITY"]
 ScaleDownBehaviorType = Literal["TERMINATE_AT_INSTANCE_HOUR", "TERMINATE_AT_TASK_COMPLETION"]
-SpotProvisioningAllocationStrategyType = Literal["capacity-optimized"]
+SpotProvisioningAllocationStrategyType = Literal[
+    "capacity-optimized", "diversified", "lowest-price", "price-capacity-optimized"
+]
 SpotProvisioningTimeoutActionType = Literal["SWITCH_TO_ON_DEMAND", "TERMINATE_CLUSTER"]
 StatisticType = Literal["AVERAGE", "MAXIMUM", "MINIMUM", "SAMPLE_COUNT", "SUM"]
 StepCancellationOptionType = Literal["SEND_INTERRUPT", "TERMINATE_PROCESS"]
 StepCompleteWaiterName = Literal["step_complete"]
 StepExecutionStateType = Literal[
     "CANCELLED", "COMPLETED", "CONTINUE", "FAILED", "INTERRUPTED", "PENDING", "RUNNING"
 ]
@@ -250,14 +254,15 @@
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
@@ -297,14 +302,15 @@
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
@@ -383,14 +389,15 @@
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
@@ -401,14 +408,15 @@
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
@@ -444,14 +452,15 @@
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
@@ -470,16 +479,19 @@
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
@@ -559,18 +571,21 @@
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

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "ListStudioSessionMappingsPaginatorName",
     "ListStudiosPaginatorName",
     "MarketTypeType",
     "NotebookExecutionStatusType",
     "OnDemandCapacityReservationPreferenceType",
     "OnDemandCapacityReservationUsageStrategyType",
     "OnDemandProvisioningAllocationStrategyType",
+    "OutputNotebookFormatType",
     "PlacementGroupStrategyType",
     "ReconfigurationTypeType",
     "RepoUpgradeOnBootType",
     "ScaleDownBehaviorType",
     "SpotProvisioningAllocationStrategyType",
     "SpotProvisioningTimeoutActionType",
     "StatisticType",
@@ -187,19 +188,22 @@
     "STOPPED",
     "STOPPING",
     "STOP_PENDING",
 ]
 OnDemandCapacityReservationPreferenceType = Literal["none", "open"]
 OnDemandCapacityReservationUsageStrategyType = Literal["use-capacity-reservations-first"]
 OnDemandProvisioningAllocationStrategyType = Literal["lowest-price"]
+OutputNotebookFormatType = Literal["HTML"]
 PlacementGroupStrategyType = Literal["CLUSTER", "NONE", "PARTITION", "SPREAD"]
 ReconfigurationTypeType = Literal["MERGE", "OVERWRITE"]
 RepoUpgradeOnBootType = Literal["NONE", "SECURITY"]
 ScaleDownBehaviorType = Literal["TERMINATE_AT_INSTANCE_HOUR", "TERMINATE_AT_TASK_COMPLETION"]
-SpotProvisioningAllocationStrategyType = Literal["capacity-optimized"]
+SpotProvisioningAllocationStrategyType = Literal[
+    "capacity-optimized", "diversified", "lowest-price", "price-capacity-optimized"
+]
 SpotProvisioningTimeoutActionType = Literal["SWITCH_TO_ON_DEMAND", "TERMINATE_CLUSTER"]
 StatisticType = Literal["AVERAGE", "MAXIMUM", "MINIMUM", "SAMPLE_COUNT", "SUM"]
 StepCancellationOptionType = Literal["SEND_INTERRUPT", "TERMINATE_PROCESS"]
 StepCompleteWaiterName = Literal["step_complete"]
 StepExecutionStateType = Literal[
     "CANCELLED", "COMPLETED", "CONTINUE", "FAILED", "INTERRUPTED", "PENDING", "RUNNING"
 ]
@@ -248,14 +252,15 @@
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
@@ -295,14 +300,15 @@
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
@@ -381,14 +387,15 @@
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
@@ -399,14 +406,15 @@
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
@@ -442,14 +450,15 @@
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
@@ -468,16 +477,19 @@
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
@@ -557,18 +569,21 @@
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

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 class ListBootstrapActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBootstrapActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
         """
 
 
@@ -112,45 +112,45 @@
 
     def paginate(
         self,
         *,
         CreatedAfter: Union[datetime, str] = ...,
         CreatedBefore: Union[datetime, str] = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
         """
 
 
 class ListInstanceFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstanceFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
         """
 
 
 class ListInstanceGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstanceGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
         """
 
 
@@ -165,15 +165,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancespaginator)
         """
 
 
@@ -186,30 +186,31 @@
     def paginate(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: Union[datetime, str] = ...,
         To: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        ExecutionEngineId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listnotebookexecutionspaginator)
         """
 
 
 class ListSecurityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSecurityConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
         """
 
 
@@ -221,15 +222,15 @@
 
     def paginate(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStepsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststepspaginator)
         """
 
 
@@ -240,28 +241,28 @@
     """
 
     def paginate(
         self,
         *,
         StudioId: str = ...,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudioSessionMappingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiosessionmappingspaginator)
         """
 
 
 class ListStudiosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudiosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
         """
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 class ListBootstrapActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBootstrapActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
         """
 
 class ListClustersPaginator(Paginator):
@@ -108,43 +108,43 @@
 
     def paginate(
         self,
         *,
         CreatedAfter: Union[datetime, str] = ...,
         CreatedBefore: Union[datetime, str] = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
         """
 
 class ListInstanceFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstanceFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
         """
 
 class ListInstanceGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstanceGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
         """
 
 class ListInstancesPaginator(Paginator):
@@ -158,15 +158,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancespaginator)
         """
 
 class ListNotebookExecutionsPaginator(Paginator):
@@ -178,29 +178,30 @@
     def paginate(
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: Union[datetime, str] = ...,
         To: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        ExecutionEngineId: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listnotebookexecutionspaginator)
         """
 
 class ListSecurityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSecurityConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
         """
 
 class ListStepsPaginator(Paginator):
@@ -211,15 +212,15 @@
 
     def paginate(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStepsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststepspaginator)
         """
 
 class ListStudioSessionMappingsPaginator(Paginator):
@@ -229,27 +230,27 @@
     """
 
     def paginate(
         self,
         *,
         StudioId: str = ...,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudioSessionMappingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiosessionmappingspaginator)
         """
 
 class ListStudiosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStudiosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
         """
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for emr service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_emr.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_emr.type_defs import AddInstanceFleetOutputTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: AddInstanceFleetOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -41,14 +41,15 @@
     MarketTypeType,
     NotebookExecutionStatusType,
     OnDemandCapacityReservationPreferenceType,
     PlacementGroupStrategyType,
     ReconfigurationTypeType,
     RepoUpgradeOnBootType,
     ScaleDownBehaviorType,
+    SpotProvisioningAllocationStrategyType,
     SpotProvisioningTimeoutActionType,
     StatisticType,
     StepCancellationOptionType,
     StepExecutionStateType,
     StepStateType,
     UnitType,
 )
@@ -60,52 +61,59 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "AddInstanceFleetOutputTypeDef",
+    "AddInstanceGroupsOutputTypeDef",
+    "AddJobFlowStepsOutputTypeDef",
     "TagTypeDef",
     "ApplicationTypeDef",
     "ScalingConstraintsTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
     "PortRangeTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
+    "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
     "KerberosAttributesTypeDef",
     "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
     "ComputeLimitsTypeDef",
     "ConfigurationTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
+    "CreateSecurityConfigurationOutputTypeDef",
+    "CreateStudioOutputTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterInputRequestTypeDef",
     "DescribeJobFlowsInputRequestTypeDef",
     "DescribeNotebookExecutionInputRequestTypeDef",
     "DescribeReleaseLabelInputRequestTypeDef",
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
+    "DescribeSecurityConfigurationOutputTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
     "VolumeSpecificationTypeDef",
     "EbsVolumeTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExecutionEngineConfigTypeDef",
     "FailureDetailsTypeDef",
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
@@ -120,58 +128,67 @@
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
+    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
+    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
+    "ListInstancesInputListInstancesPaginateTypeDef",
     "ListInstancesInputRequestTypeDef",
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     "ListNotebookExecutionsInputRequestTypeDef",
-    "NotebookExecutionSummaryTypeDef",
     "ReleaseLabelFilterTypeDef",
+    "ListReleaseLabelsOutputTypeDef",
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
     "SecurityConfigurationSummaryTypeDef",
+    "ListStepsInputListStepsPaginateTypeDef",
     "ListStepsInputRequestTypeDef",
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
     "ListStudioSessionMappingsInputRequestTypeDef",
     "SessionMappingSummaryTypeDef",
+    "ListStudiosInputListStudiosPaginateTypeDef",
     "ListStudiosInputRequestTypeDef",
     "StudioSummaryTypeDef",
+    "ListSupportedInstanceTypesInputRequestTypeDef",
+    "SupportedInstanceTypeTypeDef",
     "ModifyClusterInputRequestTypeDef",
+    "ModifyClusterOutputTypeDef",
+    "NotebookS3LocationForOutputTypeDef",
+    "OutputNotebookS3LocationForOutputTypeDef",
+    "NotebookS3LocationFromInputTypeDef",
     "OnDemandCapacityReservationOptionsTypeDef",
+    "OutputNotebookS3LocationFromInputTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SupportedProductConfigTypeDef",
+    "RunJobFlowOutputTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
+    "StartNotebookExecutionOutputTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
     "UpdateStudioSessionMappingInputRequestTypeDef",
-    "AddInstanceFleetOutputTypeDef",
-    "AddInstanceGroupsOutputTypeDef",
-    "AddJobFlowStepsOutputTypeDef",
-    "CreateSecurityConfigurationOutputTypeDef",
-    "CreateStudioOutputTypeDef",
-    "DescribeSecurityConfigurationOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListReleaseLabelsOutputTypeDef",
-    "ModifyClusterOutputTypeDef",
-    "RunJobFlowOutputTypeDef",
-    "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
     "StudioTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
@@ -184,59 +201,51 @@
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
-    "NotebookExecutionTypeDef",
-    "StartNotebookExecutionInputRequestTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
-    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
-    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    "ListInstancesInputListInstancesPaginateTypeDef",
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
-    "ListStepsInputListStepsPaginateTypeDef",
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
-    "ListStudiosInputListStudiosPaginateTypeDef",
-    "ListNotebookExecutionsOutputTypeDef",
     "ListReleaseLabelsInputRequestTypeDef",
     "ListSecurityConfigurationsOutputTypeDef",
     "ListStudioSessionMappingsOutputTypeDef",
     "ListStudiosOutputTypeDef",
+    "ListSupportedInstanceTypesOutputTypeDef",
+    "NotebookExecutionSummaryTypeDef",
+    "NotebookExecutionTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
+    "StartNotebookExecutionInputRequestTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
     "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
-    "DescribeNotebookExecutionOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
+    "ListNotebookExecutionsOutputTypeDef",
+    "DescribeNotebookExecutionOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
@@ -261,22 +270,39 @@
     "DescribeJobFlowsOutputTypeDef",
     "ListInstanceGroupsOutputTypeDef",
     "AddInstanceGroupsInputRequestTypeDef",
     "JobFlowInstancesConfigTypeDef",
     "RunJobFlowInputRequestTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddInstanceFleetOutputTypeDef = TypedDict(
+    "AddInstanceFleetOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ClusterId": str,
+        "InstanceFleetId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AddInstanceGroupsOutputTypeDef = TypedDict(
+    "AddInstanceGroupsOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "InstanceGroupIds": List[str],
+        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AddJobFlowStepsOutputTypeDef = TypedDict(
+    "AddJobFlowStepsOutputTypeDef",
+    {
+        "StepIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -425,14 +451,24 @@
         "CreationDateTime": datetime,
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
+ErrorDetailTypeDef = TypedDict(
+    "ErrorDetailTypeDef",
+    {
+        "ErrorCode": str,
+        "ErrorData": List[Dict[str, str]],
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 Ec2InstanceAttributesTypeDef = TypedDict(
     "Ec2InstanceAttributesTypeDef",
     {
         "Ec2KeyName": str,
         "Ec2SubnetId": str,
         "RequestedEc2SubnetIds": List[str],
         "Ec2AvailabilityZone": str,
@@ -538,14 +574,32 @@
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
 
+CreateSecurityConfigurationOutputTypeDef = TypedDict(
+    "CreateSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "CreationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStudioOutputTypeDef = TypedDict(
+    "CreateStudioOutputTypeDef",
+    {
+        "StudioId": str,
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateStudioSessionMappingInputRequestTypeDef = TypedDict(
     "_RequiredCreateStudioSessionMappingInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
     },
@@ -678,14 +732,24 @@
 DescribeSecurityConfigurationInputRequestTypeDef = TypedDict(
     "DescribeSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeSecurityConfigurationOutputTypeDef = TypedDict(
+    "DescribeSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "SecurityConfiguration": str,
+        "CreationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeStepInputRequestTypeDef = TypedDict(
     "DescribeStepInputRequestTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
     },
 )
@@ -725,25 +789,33 @@
     {
         "Device": str,
         "VolumeId": str,
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
 _RequiredExecutionEngineConfigTypeDef = TypedDict(
     "_RequiredExecutionEngineConfigTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalExecutionEngineConfigTypeDef = TypedDict(
     "_OptionalExecutionEngineConfigTypeDef",
     {
         "Type": Literal["EMR"],
         "MasterInstanceSecurityGroupId": str,
+        "ExecutionRoleArn": str,
     },
     total=False,
 )
 
 
 class ExecutionEngineConfigTypeDef(
     _RequiredExecutionEngineConfigTypeDef, _OptionalExecutionEngineConfigTypeDef
@@ -848,15 +920,15 @@
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
 _OptionalSpotProvisioningSpecificationTypeDef = TypedDict(
     "_OptionalSpotProvisioningSpecificationTypeDef",
     {
         "BlockDurationMinutes": int,
-        "AllocationStrategy": Literal["capacity-optimized"],
+        "AllocationStrategy": SpotProvisioningAllocationStrategyType,
     },
     total=False,
 )
 
 
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
@@ -1009,24 +1081,36 @@
     {
         "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterId": str,
+    },
+)
+_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
+    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputRequestTypeDef = TypedDict(
@@ -1041,25 +1125,58 @@
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
 
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "CreatedAfter": Union[datetime, str],
+        "CreatedBefore": Union[datetime, str],
+        "ClusterStates": Sequence[ClusterStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ClusterStates": Sequence[ClusterStateType],
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
+    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
@@ -1073,14 +1190,36 @@
 
 class ListInstanceFleetsInputRequestTypeDef(
     _RequiredListInstanceFleetsInputRequestTypeDef, _OptionalListInstanceFleetsInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
+    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputRequestTypeDef = TypedDict(
@@ -1094,14 +1233,41 @@
 
 class ListInstanceGroupsInputRequestTypeDef(
     _RequiredListInstanceGroupsInputRequestTypeDef, _OptionalListInstanceGroupsInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "InstanceGroupId": str,
+        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
+        "InstanceFleetId": str,
+        "InstanceFleetType": InstanceFleetTypeType,
+        "InstanceStates": Sequence[InstanceStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInstancesInputListInstancesPaginateTypeDef(
+    _RequiredListInstancesInputListInstancesPaginateTypeDef,
+    _OptionalListInstancesInputListInstancesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListInstancesInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputRequestTypeDef = TypedDict(
@@ -1120,48 +1286,66 @@
 
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
 
-ListNotebookExecutionsInputRequestTypeDef = TypedDict(
-    "ListNotebookExecutionsInputRequestTypeDef",
+ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
         "From": Union[datetime, str],
         "To": Union[datetime, str],
-        "Marker": str,
+        "ExecutionEngineId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-NotebookExecutionSummaryTypeDef = TypedDict(
-    "NotebookExecutionSummaryTypeDef",
+ListNotebookExecutionsInputRequestTypeDef = TypedDict(
+    "ListNotebookExecutionsInputRequestTypeDef",
     {
-        "NotebookExecutionId": str,
         "EditorId": str,
-        "NotebookExecutionName": str,
         "Status": NotebookExecutionStatusType,
-        "StartTime": datetime,
-        "EndTime": datetime,
+        "From": Union[datetime, str],
+        "To": Union[datetime, str],
+        "Marker": str,
+        "ExecutionEngineId": str,
     },
     total=False,
 )
 
 ReleaseLabelFilterTypeDef = TypedDict(
     "ReleaseLabelFilterTypeDef",
     {
         "Prefix": str,
         "Application": str,
     },
     total=False,
 )
 
+ListReleaseLabelsOutputTypeDef = TypedDict(
+    "ListReleaseLabelsOutputTypeDef",
+    {
+        "ReleaseLabels": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSecurityConfigurationsInputRequestTypeDef = TypedDict(
     "ListSecurityConfigurationsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1171,14 +1355,37 @@
     {
         "Name": str,
         "CreationDateTime": datetime,
     },
     total=False,
 )
 
+_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_RequiredListStepsInputListStepsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_OptionalListStepsInputListStepsPaginateTypeDef",
+    {
+        "StepStates": Sequence[StepStateType],
+        "StepIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListStepsInputListStepsPaginateTypeDef(
+    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
+):
+    pass
+
+
 _RequiredListStepsInputRequestTypeDef = TypedDict(
     "_RequiredListStepsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListStepsInputRequestTypeDef = TypedDict(
@@ -1194,14 +1401,24 @@
 
 class ListStepsInputRequestTypeDef(
     _RequiredListStepsInputRequestTypeDef, _OptionalListStepsInputRequestTypeDef
 ):
     pass
 
 
+ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
+    {
+        "StudioId": str,
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStudioSessionMappingsInputRequestTypeDef = TypedDict(
     "ListStudioSessionMappingsInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "Marker": str,
     },
@@ -1217,14 +1434,22 @@
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosInputListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStudiosInputRequestTypeDef = TypedDict(
     "ListStudiosInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1239,14 +1464,54 @@
         "Url": str,
         "AuthMode": AuthModeType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+_RequiredListSupportedInstanceTypesInputRequestTypeDef = TypedDict(
+    "_RequiredListSupportedInstanceTypesInputRequestTypeDef",
+    {
+        "ReleaseLabel": str,
+    },
+)
+_OptionalListSupportedInstanceTypesInputRequestTypeDef = TypedDict(
+    "_OptionalListSupportedInstanceTypesInputRequestTypeDef",
+    {
+        "Marker": str,
+    },
+    total=False,
+)
+
+
+class ListSupportedInstanceTypesInputRequestTypeDef(
+    _RequiredListSupportedInstanceTypesInputRequestTypeDef,
+    _OptionalListSupportedInstanceTypesInputRequestTypeDef,
+):
+    pass
+
+
+SupportedInstanceTypeTypeDef = TypedDict(
+    "SupportedInstanceTypeTypeDef",
+    {
+        "Type": str,
+        "MemoryGB": float,
+        "StorageGB": int,
+        "VCPU": int,
+        "Is64BitsOnly": bool,
+        "InstanceFamilyId": str,
+        "EbsOptimizedAvailable": bool,
+        "EbsOptimizedByDefault": bool,
+        "NumberOfDisks": int,
+        "EbsStorageOnly": bool,
+        "Architecture": str,
+    },
+    total=False,
+)
+
 _RequiredModifyClusterInputRequestTypeDef = TypedDict(
     "_RequiredModifyClusterInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalModifyClusterInputRequestTypeDef = TypedDict(
@@ -1260,24 +1525,78 @@
 
 class ModifyClusterInputRequestTypeDef(
     _RequiredModifyClusterInputRequestTypeDef, _OptionalModifyClusterInputRequestTypeDef
 ):
     pass
 
 
+ModifyClusterOutputTypeDef = TypedDict(
+    "ModifyClusterOutputTypeDef",
+    {
+        "StepConcurrencyLevel": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+NotebookS3LocationForOutputTypeDef = TypedDict(
+    "NotebookS3LocationForOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
+)
+
+OutputNotebookS3LocationForOutputTypeDef = TypedDict(
+    "OutputNotebookS3LocationForOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
+)
+
+NotebookS3LocationFromInputTypeDef = TypedDict(
+    "NotebookS3LocationFromInputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
+)
+
 OnDemandCapacityReservationOptionsTypeDef = TypedDict(
     "OnDemandCapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
         "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
         "CapacityReservationResourceGroupArn": str,
     },
     total=False,
 )
 
+OutputNotebookS3LocationFromInputTypeDef = TypedDict(
+    "OutputNotebookS3LocationFromInputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
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
 RemoveAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
     },
 )
@@ -1300,23 +1619,43 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
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
 SupportedProductConfigTypeDef = TypedDict(
     "SupportedProductConfigTypeDef",
     {
         "Name": str,
         "Args": Sequence[str],
     },
     total=False,
 )
 
+RunJobFlowOutputTypeDef = TypedDict(
+    "RunJobFlowOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSimpleScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredSimpleScalingPolicyConfigurationTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalSimpleScalingPolicyConfigurationTypeDef = TypedDict(
@@ -1348,14 +1687,22 @@
     "SetVisibleToAllUsersInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "VisibleToAllUsers": bool,
     },
 )
 
+StartNotebookExecutionOutputTypeDef = TypedDict(
+    "StartNotebookExecutionOutputTypeDef",
+    {
+        "NotebookExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStepExecutionStatusDetailTypeDef = TypedDict(
     "_RequiredStepExecutionStatusDetailTypeDef",
     {
         "State": StepExecutionStateType,
         "CreationDateTime": datetime,
     },
 )
@@ -1454,111 +1801,14 @@
 class UpdateStudioSessionMappingInputRequestTypeDef(
     _RequiredUpdateStudioSessionMappingInputRequestTypeDef,
     _OptionalUpdateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
 
-AddInstanceFleetOutputTypeDef = TypedDict(
-    "AddInstanceFleetOutputTypeDef",
-    {
-        "ClusterId": str,
-        "InstanceFleetId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddInstanceGroupsOutputTypeDef = TypedDict(
-    "AddInstanceGroupsOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "InstanceGroupIds": List[str],
-        "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddJobFlowStepsOutputTypeDef = TypedDict(
-    "AddJobFlowStepsOutputTypeDef",
-    {
-        "StepIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSecurityConfigurationOutputTypeDef = TypedDict(
-    "CreateSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "CreationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStudioOutputTypeDef = TypedDict(
-    "CreateStudioOutputTypeDef",
-    {
-        "StudioId": str,
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSecurityConfigurationOutputTypeDef = TypedDict(
-    "DescribeSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "SecurityConfiguration": str,
-        "CreationDateTime": datetime,
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
-ListReleaseLabelsOutputTypeDef = TypedDict(
-    "ListReleaseLabelsOutputTypeDef",
-    {
-        "ReleaseLabels": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyClusterOutputTypeDef = TypedDict(
-    "ModifyClusterOutputTypeDef",
-    {
-        "StepConcurrencyLevel": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunJobFlowOutputTypeDef = TypedDict(
-    "RunJobFlowOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartNotebookExecutionOutputTypeDef = TypedDict(
-    "StartNotebookExecutionOutputTypeDef",
-    {
-        "NotebookExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1628,15 +1878,15 @@
     total=False,
 )
 
 GetAutoTerminationPolicyOutputTypeDef = TypedDict(
     "GetAutoTerminationPolicyOutputTypeDef",
     {
         "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAutoTerminationPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutAutoTerminationPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -1687,15 +1937,15 @@
     },
 )
 
 CancelStepsOutputTypeDef = TypedDict(
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCloudWatchAlarmDefinitionTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
@@ -1725,24 +1975,25 @@
 
 ClusterStatusTypeDef = TypedDict(
     "ClusterStatusTypeDef",
     {
         "State": ClusterStateType,
         "StateChangeReason": ClusterStateChangeReasonTypeDef,
         "Timeline": ClusterTimelineTypeDef,
+        "ErrorDetails": List[ErrorDetailTypeDef],
     },
     total=False,
 )
 
 ListBootstrapActionsOutputTypeDef = TypedDict(
     "ListBootstrapActionsOutputTypeDef",
     {
         "BootstrapActions": List[CommandTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ManagedScalingPolicyTypeDef = TypedDict(
     "ManagedScalingPolicyTypeDef",
     {
         "ComputeLimits": ComputeLimitsTypeDef,
@@ -1828,15 +2079,15 @@
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEbsBlockDeviceConfigTypeDef = TypedDict(
     "_RequiredEbsBlockDeviceConfigTypeDef",
     {
         "VolumeSpecification": VolumeSpecificationTypeDef,
@@ -1862,67 +2113,19 @@
     {
         "VolumeSpecification": VolumeSpecificationTypeDef,
         "Device": str,
     },
     total=False,
 )
 
-NotebookExecutionTypeDef = TypedDict(
-    "NotebookExecutionTypeDef",
-    {
-        "NotebookExecutionId": str,
-        "EditorId": str,
-        "ExecutionEngine": ExecutionEngineConfigTypeDef,
-        "NotebookExecutionName": str,
-        "NotebookParams": str,
-        "Status": NotebookExecutionStatusType,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "Arn": str,
-        "OutputNotebookURI": str,
-        "LastStateChangeReason": str,
-        "NotebookInstanceSecurityGroupId": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-_RequiredStartNotebookExecutionInputRequestTypeDef = TypedDict(
-    "_RequiredStartNotebookExecutionInputRequestTypeDef",
-    {
-        "EditorId": str,
-        "RelativePath": str,
-        "ExecutionEngine": ExecutionEngineConfigTypeDef,
-        "ServiceRole": str,
-    },
-)
-_OptionalStartNotebookExecutionInputRequestTypeDef = TypedDict(
-    "_OptionalStartNotebookExecutionInputRequestTypeDef",
-    {
-        "NotebookExecutionName": str,
-        "NotebookParams": str,
-        "NotebookInstanceSecurityGroupId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class StartNotebookExecutionInputRequestTypeDef(
-    _RequiredStartNotebookExecutionInputRequestTypeDef,
-    _OptionalStartNotebookExecutionInputRequestTypeDef,
-):
-    pass
-
-
 GetStudioSessionMappingOutputTypeDef = TypedDict(
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHadoopJarStepConfigTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigTypeDef",
     {
         "Jar": str,
@@ -2021,243 +2224,149 @@
 
 class JobFlowInstancesDetailTypeDef(
     _RequiredJobFlowInstancesDetailTypeDef, _OptionalJobFlowInstancesDetailTypeDef
 ):
     pass
 
 
-_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+ListReleaseLabelsInputRequestTypeDef = TypedDict(
+    "ListReleaseLabelsInputRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": ReleaseLabelFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-
-class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
-    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-):
-    pass
-
-
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
+ListSecurityConfigurationsOutputTypeDef = TypedDict(
+    "ListSecurityConfigurationsOutputTypeDef",
     {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ClusterStates": Sequence[ClusterStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "SecurityConfigurations": List[SecurityConfigurationSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+ListStudioSessionMappingsOutputTypeDef = TypedDict(
+    "ListStudioSessionMappingsOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "SessionMappings": List[SessionMappingSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
-    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+ListStudiosOutputTypeDef = TypedDict(
+    "ListStudiosOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Studios": List[StudioSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
-    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
+ListSupportedInstanceTypesOutputTypeDef = TypedDict(
+    "ListSupportedInstanceTypesOutputTypeDef",
     {
-        "InstanceGroupId": str,
-        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
-        "InstanceFleetId": str,
-        "InstanceFleetType": InstanceFleetTypeType,
-        "InstanceStates": Sequence[InstanceStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "SupportedInstanceTypes": List[SupportedInstanceTypeTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListInstancesInputListInstancesPaginateTypeDef(
-    _RequiredListInstancesInputListInstancesPaginateTypeDef,
-    _OptionalListInstancesInputListInstancesPaginateTypeDef,
-):
-    pass
-
-
-ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
+NotebookExecutionSummaryTypeDef = TypedDict(
+    "NotebookExecutionSummaryTypeDef",
     {
+        "NotebookExecutionId": str,
         "EditorId": str,
+        "NotebookExecutionName": str,
         "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
+        "ExecutionEngineId": str,
     },
     total=False,
 )
 
-ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+NotebookExecutionTypeDef = TypedDict(
+    "NotebookExecutionTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NotebookExecutionId": str,
+        "EditorId": str,
+        "ExecutionEngine": ExecutionEngineConfigTypeDef,
+        "NotebookExecutionName": str,
+        "NotebookParams": str,
+        "Status": NotebookExecutionStatusType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "Arn": str,
+        "OutputNotebookURI": str,
+        "LastStateChangeReason": str,
+        "NotebookInstanceSecurityGroupId": str,
+        "Tags": List[TagTypeDef],
+        "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
+        "OutputNotebookS3Location": OutputNotebookS3LocationForOutputTypeDef,
+        "OutputNotebookFormat": Literal["HTML"],
+        "EnvironmentVariables": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_RequiredListStepsInputListStepsPaginateTypeDef",
+_RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
+    "_RequiredOnDemandProvisioningSpecificationTypeDef",
     {
-        "ClusterId": str,
+        "AllocationStrategy": Literal["lowest-price"],
     },
 )
-_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_OptionalListStepsInputListStepsPaginateTypeDef",
+_OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
+    "_OptionalOnDemandProvisioningSpecificationTypeDef",
     {
-        "StepStates": Sequence[StepStateType],
-        "StepIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "CapacityReservationOptions": OnDemandCapacityReservationOptionsTypeDef,
     },
     total=False,
 )
 
 
-class ListStepsInputListStepsPaginateTypeDef(
-    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
+class OnDemandProvisioningSpecificationTypeDef(
+    _RequiredOnDemandProvisioningSpecificationTypeDef,
+    _OptionalOnDemandProvisioningSpecificationTypeDef,
 ):
     pass
 
 
-ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
-    {
-        "StudioId": str,
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosInputListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListNotebookExecutionsOutputTypeDef = TypedDict(
-    "ListNotebookExecutionsOutputTypeDef",
-    {
-        "NotebookExecutions": List[NotebookExecutionSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReleaseLabelsInputRequestTypeDef = TypedDict(
-    "ListReleaseLabelsInputRequestTypeDef",
-    {
-        "Filters": ReleaseLabelFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSecurityConfigurationsOutputTypeDef = TypedDict(
-    "ListSecurityConfigurationsOutputTypeDef",
-    {
-        "SecurityConfigurations": List[SecurityConfigurationSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStudioSessionMappingsOutputTypeDef = TypedDict(
-    "ListStudioSessionMappingsOutputTypeDef",
-    {
-        "SessionMappings": List[SessionMappingSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStudiosOutputTypeDef = TypedDict(
-    "ListStudiosOutputTypeDef",
-    {
-        "Studios": List[StudioSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
-    "_RequiredOnDemandProvisioningSpecificationTypeDef",
+_RequiredStartNotebookExecutionInputRequestTypeDef = TypedDict(
+    "_RequiredStartNotebookExecutionInputRequestTypeDef",
     {
-        "AllocationStrategy": Literal["lowest-price"],
+        "ExecutionEngine": ExecutionEngineConfigTypeDef,
+        "ServiceRole": str,
     },
 )
-_OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
-    "_OptionalOnDemandProvisioningSpecificationTypeDef",
+_OptionalStartNotebookExecutionInputRequestTypeDef = TypedDict(
+    "_OptionalStartNotebookExecutionInputRequestTypeDef",
     {
-        "CapacityReservationOptions": OnDemandCapacityReservationOptionsTypeDef,
+        "EditorId": str,
+        "RelativePath": str,
+        "NotebookExecutionName": str,
+        "NotebookParams": str,
+        "NotebookInstanceSecurityGroupId": str,
+        "Tags": Sequence[TagTypeDef],
+        "NotebookS3Location": NotebookS3LocationFromInputTypeDef,
+        "OutputNotebookS3Location": OutputNotebookS3LocationFromInputTypeDef,
+        "OutputNotebookFormat": Literal["HTML"],
+        "EnvironmentVariables": Mapping[str, str],
     },
     total=False,
 )
 
 
-class OnDemandProvisioningSpecificationTypeDef(
-    _RequiredOnDemandProvisioningSpecificationTypeDef,
-    _OptionalOnDemandProvisioningSpecificationTypeDef,
+class StartNotebookExecutionInputRequestTypeDef(
+    _RequiredStartNotebookExecutionInputRequestTypeDef,
+    _OptionalStartNotebookExecutionInputRequestTypeDef,
 ):
     pass
 
 
 _RequiredScalingActionTypeDef = TypedDict(
     "_RequiredScalingActionTypeDef",
     {
@@ -2288,24 +2397,24 @@
     total=False,
 )
 
 DescribeStudioOutputTypeDef = TypedDict(
     "DescribeStudioOutputTypeDef",
     {
         "Studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
@@ -2378,15 +2487,15 @@
     total=False,
 )
 
 GetManagedScalingPolicyOutputTypeDef = TypedDict(
     "GetManagedScalingPolicyOutputTypeDef",
     {
         "ManagedScalingPolicy": ManagedScalingPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedScalingPolicyInputRequestTypeDef = TypedDict(
     "PutManagedScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -2395,15 +2504,15 @@
 )
 
 GetClusterSessionCredentialsOutputTypeDef = TypedDict(
     "GetClusterSessionCredentialsOutputTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "ExpiresAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EbsConfigurationTypeDef = TypedDict(
     "EbsConfigurationTypeDef",
     {
         "EbsBlockDeviceConfigs": Sequence[EbsBlockDeviceConfigTypeDef],
@@ -2423,22 +2532,14 @@
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
         "CustomAmiId": str,
     },
     total=False,
 )
 
-DescribeNotebookExecutionOutputTypeDef = TypedDict(
-    "DescribeNotebookExecutionOutputTypeDef",
-    {
-        "NotebookExecution": NotebookExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredStepConfigTypeDef = TypedDict(
     "_RequiredStepConfigTypeDef",
     {
         "Name": str,
         "HadoopJarStep": HadoopJarStepConfigTypeDef,
     },
 )
@@ -2518,14 +2619,31 @@
         "Market": MarketTypeType,
         "InstanceType": str,
         "EbsVolumes": List[EbsVolumeTypeDef],
     },
     total=False,
 )
 
+ListNotebookExecutionsOutputTypeDef = TypedDict(
+    "ListNotebookExecutionsOutputTypeDef",
+    {
+        "NotebookExecutions": List[NotebookExecutionSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeNotebookExecutionOutputTypeDef = TypedDict(
+    "DescribeNotebookExecutionOutputTypeDef",
+    {
+        "NotebookExecution": NotebookExecutionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InstanceFleetProvisioningSpecificationsTypeDef = TypedDict(
     "InstanceFleetProvisioningSpecificationsTypeDef",
     {
         "SpotSpecification": SpotProvisioningSpecificationTypeDef,
         "OnDemandSpecification": OnDemandProvisioningSpecificationTypeDef,
     },
     total=False,
@@ -2578,23 +2696,23 @@
 
 
 ListClustersOutputTypeDef = TypedDict(
     "ListClustersOutputTypeDef",
     {
         "Clusters": List[ClusterSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterOutputTypeDef = TypedDict(
     "DescribeClusterOutputTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInstanceTypeConfigTypeDef = TypedDict(
     "_RequiredInstanceTypeConfigTypeDef",
     {
         "InstanceType": str,
@@ -2668,15 +2786,15 @@
 )
 
 ListInstancesOutputTypeDef = TypedDict(
     "ListInstancesOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceFleetTypeDef = TypedDict(
     "InstanceFleetTypeDef",
     {
         "Id": str,
@@ -2695,23 +2813,23 @@
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
         "Steps": List[StepSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStepOutputTypeDef = TypedDict(
     "DescribeStepOutputTypeDef",
     {
         "Step": StepTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
@@ -2788,15 +2906,15 @@
 
 
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceGroupTypeDef = TypedDict(
     "InstanceGroupTypeDef",
     {
         "Id": str,
@@ -2824,15 +2942,15 @@
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
     "PutAutoScalingPolicyOutputTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInstanceGroupConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupConfigTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
@@ -2878,24 +2996,24 @@
     },
 )
 
 DescribeJobFlowsOutputTypeDef = TypedDict(
     "DescribeJobFlowsOutputTypeDef",
     {
         "JobFlows": List[JobFlowDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstanceGroupsOutputTypeDef = TypedDict(
     "ListInstanceGroupsOutputTypeDef",
     {
         "InstanceGroups": List[InstanceGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddInstanceGroupsInputRequestTypeDef = TypedDict(
     "AddInstanceGroupsInputRequestTypeDef",
     {
         "InstanceGroups": Sequence[InstanceGroupConfigTypeDef],
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for emr service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_emr.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_emr.type_defs import AddInstanceFleetOutputTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: AddInstanceFleetOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -41,14 +41,15 @@
     MarketTypeType,
     NotebookExecutionStatusType,
     OnDemandCapacityReservationPreferenceType,
     PlacementGroupStrategyType,
     ReconfigurationTypeType,
     RepoUpgradeOnBootType,
     ScaleDownBehaviorType,
+    SpotProvisioningAllocationStrategyType,
     SpotProvisioningTimeoutActionType,
     StatisticType,
     StepCancellationOptionType,
     StepExecutionStateType,
     StepStateType,
     UnitType,
 )
@@ -59,52 +60,59 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "AddInstanceFleetOutputTypeDef",
+    "AddInstanceGroupsOutputTypeDef",
+    "AddJobFlowStepsOutputTypeDef",
     "TagTypeDef",
     "ApplicationTypeDef",
     "ScalingConstraintsTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
     "PortRangeTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
+    "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
     "KerberosAttributesTypeDef",
     "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
     "ComputeLimitsTypeDef",
     "ConfigurationTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
+    "CreateSecurityConfigurationOutputTypeDef",
+    "CreateStudioOutputTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterInputRequestTypeDef",
     "DescribeJobFlowsInputRequestTypeDef",
     "DescribeNotebookExecutionInputRequestTypeDef",
     "DescribeReleaseLabelInputRequestTypeDef",
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
+    "DescribeSecurityConfigurationOutputTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
     "VolumeSpecificationTypeDef",
     "EbsVolumeTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExecutionEngineConfigTypeDef",
     "FailureDetailsTypeDef",
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
@@ -119,58 +127,67 @@
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
+    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
+    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
+    "ListInstancesInputListInstancesPaginateTypeDef",
     "ListInstancesInputRequestTypeDef",
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     "ListNotebookExecutionsInputRequestTypeDef",
-    "NotebookExecutionSummaryTypeDef",
     "ReleaseLabelFilterTypeDef",
+    "ListReleaseLabelsOutputTypeDef",
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
     "SecurityConfigurationSummaryTypeDef",
+    "ListStepsInputListStepsPaginateTypeDef",
     "ListStepsInputRequestTypeDef",
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
     "ListStudioSessionMappingsInputRequestTypeDef",
     "SessionMappingSummaryTypeDef",
+    "ListStudiosInputListStudiosPaginateTypeDef",
     "ListStudiosInputRequestTypeDef",
     "StudioSummaryTypeDef",
+    "ListSupportedInstanceTypesInputRequestTypeDef",
+    "SupportedInstanceTypeTypeDef",
     "ModifyClusterInputRequestTypeDef",
+    "ModifyClusterOutputTypeDef",
+    "NotebookS3LocationForOutputTypeDef",
+    "OutputNotebookS3LocationForOutputTypeDef",
+    "NotebookS3LocationFromInputTypeDef",
     "OnDemandCapacityReservationOptionsTypeDef",
+    "OutputNotebookS3LocationFromInputTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SupportedProductConfigTypeDef",
+    "RunJobFlowOutputTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
+    "StartNotebookExecutionOutputTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
     "UpdateStudioSessionMappingInputRequestTypeDef",
-    "AddInstanceFleetOutputTypeDef",
-    "AddInstanceGroupsOutputTypeDef",
-    "AddJobFlowStepsOutputTypeDef",
-    "CreateSecurityConfigurationOutputTypeDef",
-    "CreateStudioOutputTypeDef",
-    "DescribeSecurityConfigurationOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListReleaseLabelsOutputTypeDef",
-    "ModifyClusterOutputTypeDef",
-    "RunJobFlowOutputTypeDef",
-    "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
     "StudioTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
@@ -183,59 +200,51 @@
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
-    "NotebookExecutionTypeDef",
-    "StartNotebookExecutionInputRequestTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
-    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
-    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    "ListInstancesInputListInstancesPaginateTypeDef",
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
-    "ListStepsInputListStepsPaginateTypeDef",
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
-    "ListStudiosInputListStudiosPaginateTypeDef",
-    "ListNotebookExecutionsOutputTypeDef",
     "ListReleaseLabelsInputRequestTypeDef",
     "ListSecurityConfigurationsOutputTypeDef",
     "ListStudioSessionMappingsOutputTypeDef",
     "ListStudiosOutputTypeDef",
+    "ListSupportedInstanceTypesOutputTypeDef",
+    "NotebookExecutionSummaryTypeDef",
+    "NotebookExecutionTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
+    "StartNotebookExecutionInputRequestTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
     "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
-    "DescribeNotebookExecutionOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
+    "ListNotebookExecutionsOutputTypeDef",
+    "DescribeNotebookExecutionOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
@@ -260,22 +269,39 @@
     "DescribeJobFlowsOutputTypeDef",
     "ListInstanceGroupsOutputTypeDef",
     "AddInstanceGroupsInputRequestTypeDef",
     "JobFlowInstancesConfigTypeDef",
     "RunJobFlowInputRequestTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddInstanceFleetOutputTypeDef = TypedDict(
+    "AddInstanceFleetOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ClusterId": str,
+        "InstanceFleetId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AddInstanceGroupsOutputTypeDef = TypedDict(
+    "AddInstanceGroupsOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "InstanceGroupIds": List[str],
+        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AddJobFlowStepsOutputTypeDef = TypedDict(
+    "AddJobFlowStepsOutputTypeDef",
+    {
+        "StepIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -418,14 +444,24 @@
         "CreationDateTime": datetime,
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
+ErrorDetailTypeDef = TypedDict(
+    "ErrorDetailTypeDef",
+    {
+        "ErrorCode": str,
+        "ErrorData": List[Dict[str, str]],
+        "ErrorMessage": str,
+    },
+    total=False,
+)
+
 Ec2InstanceAttributesTypeDef = TypedDict(
     "Ec2InstanceAttributesTypeDef",
     {
         "Ec2KeyName": str,
         "Ec2SubnetId": str,
         "RequestedEc2SubnetIds": List[str],
         "Ec2AvailabilityZone": str,
@@ -525,14 +561,32 @@
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
 
+CreateSecurityConfigurationOutputTypeDef = TypedDict(
+    "CreateSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "CreationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStudioOutputTypeDef = TypedDict(
+    "CreateStudioOutputTypeDef",
+    {
+        "StudioId": str,
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateStudioSessionMappingInputRequestTypeDef = TypedDict(
     "_RequiredCreateStudioSessionMappingInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
     },
@@ -661,14 +715,24 @@
 DescribeSecurityConfigurationInputRequestTypeDef = TypedDict(
     "DescribeSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeSecurityConfigurationOutputTypeDef = TypedDict(
+    "DescribeSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "SecurityConfiguration": str,
+        "CreationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeStepInputRequestTypeDef = TypedDict(
     "DescribeStepInputRequestTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
     },
 )
@@ -706,25 +770,33 @@
     {
         "Device": str,
         "VolumeId": str,
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
 _RequiredExecutionEngineConfigTypeDef = TypedDict(
     "_RequiredExecutionEngineConfigTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalExecutionEngineConfigTypeDef = TypedDict(
     "_OptionalExecutionEngineConfigTypeDef",
     {
         "Type": Literal["EMR"],
         "MasterInstanceSecurityGroupId": str,
+        "ExecutionRoleArn": str,
     },
     total=False,
 )
 
 class ExecutionEngineConfigTypeDef(
     _RequiredExecutionEngineConfigTypeDef, _OptionalExecutionEngineConfigTypeDef
 ):
@@ -825,15 +897,15 @@
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
 _OptionalSpotProvisioningSpecificationTypeDef = TypedDict(
     "_OptionalSpotProvisioningSpecificationTypeDef",
     {
         "BlockDurationMinutes": int,
-        "AllocationStrategy": Literal["capacity-optimized"],
+        "AllocationStrategy": SpotProvisioningAllocationStrategyType,
     },
     total=False,
 )
 
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
@@ -980,24 +1052,34 @@
     {
         "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterId": str,
+    },
+)
+_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
+    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputRequestTypeDef = TypedDict(
@@ -1010,25 +1092,56 @@
 
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "CreatedAfter": Union[datetime, str],
+        "CreatedBefore": Union[datetime, str],
+        "ClusterStates": Sequence[ClusterStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ClusterStates": Sequence[ClusterStateType],
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
+    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
@@ -1040,14 +1153,34 @@
 )
 
 class ListInstanceFleetsInputRequestTypeDef(
     _RequiredListInstanceFleetsInputRequestTypeDef, _OptionalListInstanceFleetsInputRequestTypeDef
 ):
     pass
 
+_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
+    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputRequestTypeDef = TypedDict(
@@ -1059,14 +1192,39 @@
 )
 
 class ListInstanceGroupsInputRequestTypeDef(
     _RequiredListInstanceGroupsInputRequestTypeDef, _OptionalListInstanceGroupsInputRequestTypeDef
 ):
     pass
 
+_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "InstanceGroupId": str,
+        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
+        "InstanceFleetId": str,
+        "InstanceFleetType": InstanceFleetTypeType,
+        "InstanceStates": Sequence[InstanceStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInstancesInputListInstancesPaginateTypeDef(
+    _RequiredListInstancesInputListInstancesPaginateTypeDef,
+    _OptionalListInstancesInputListInstancesPaginateTypeDef,
+):
+    pass
+
 _RequiredListInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListInstancesInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputRequestTypeDef = TypedDict(
@@ -1083,48 +1241,66 @@
 )
 
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
-ListNotebookExecutionsInputRequestTypeDef = TypedDict(
-    "ListNotebookExecutionsInputRequestTypeDef",
+ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
         "From": Union[datetime, str],
         "To": Union[datetime, str],
-        "Marker": str,
+        "ExecutionEngineId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-NotebookExecutionSummaryTypeDef = TypedDict(
-    "NotebookExecutionSummaryTypeDef",
+ListNotebookExecutionsInputRequestTypeDef = TypedDict(
+    "ListNotebookExecutionsInputRequestTypeDef",
     {
-        "NotebookExecutionId": str,
         "EditorId": str,
-        "NotebookExecutionName": str,
         "Status": NotebookExecutionStatusType,
-        "StartTime": datetime,
-        "EndTime": datetime,
+        "From": Union[datetime, str],
+        "To": Union[datetime, str],
+        "Marker": str,
+        "ExecutionEngineId": str,
     },
     total=False,
 )
 
 ReleaseLabelFilterTypeDef = TypedDict(
     "ReleaseLabelFilterTypeDef",
     {
         "Prefix": str,
         "Application": str,
     },
     total=False,
 )
 
+ListReleaseLabelsOutputTypeDef = TypedDict(
+    "ListReleaseLabelsOutputTypeDef",
+    {
+        "ReleaseLabels": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSecurityConfigurationsInputRequestTypeDef = TypedDict(
     "ListSecurityConfigurationsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1134,14 +1310,35 @@
     {
         "Name": str,
         "CreationDateTime": datetime,
     },
     total=False,
 )
 
+_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_RequiredListStepsInputListStepsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_OptionalListStepsInputListStepsPaginateTypeDef",
+    {
+        "StepStates": Sequence[StepStateType],
+        "StepIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListStepsInputListStepsPaginateTypeDef(
+    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
+):
+    pass
+
 _RequiredListStepsInputRequestTypeDef = TypedDict(
     "_RequiredListStepsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListStepsInputRequestTypeDef = TypedDict(
@@ -1155,14 +1352,24 @@
 )
 
 class ListStepsInputRequestTypeDef(
     _RequiredListStepsInputRequestTypeDef, _OptionalListStepsInputRequestTypeDef
 ):
     pass
 
+ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
+    {
+        "StudioId": str,
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStudioSessionMappingsInputRequestTypeDef = TypedDict(
     "ListStudioSessionMappingsInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "Marker": str,
     },
@@ -1178,14 +1385,22 @@
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosInputListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStudiosInputRequestTypeDef = TypedDict(
     "ListStudiosInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1200,14 +1415,52 @@
         "Url": str,
         "AuthMode": AuthModeType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+_RequiredListSupportedInstanceTypesInputRequestTypeDef = TypedDict(
+    "_RequiredListSupportedInstanceTypesInputRequestTypeDef",
+    {
+        "ReleaseLabel": str,
+    },
+)
+_OptionalListSupportedInstanceTypesInputRequestTypeDef = TypedDict(
+    "_OptionalListSupportedInstanceTypesInputRequestTypeDef",
+    {
+        "Marker": str,
+    },
+    total=False,
+)
+
+class ListSupportedInstanceTypesInputRequestTypeDef(
+    _RequiredListSupportedInstanceTypesInputRequestTypeDef,
+    _OptionalListSupportedInstanceTypesInputRequestTypeDef,
+):
+    pass
+
+SupportedInstanceTypeTypeDef = TypedDict(
+    "SupportedInstanceTypeTypeDef",
+    {
+        "Type": str,
+        "MemoryGB": float,
+        "StorageGB": int,
+        "VCPU": int,
+        "Is64BitsOnly": bool,
+        "InstanceFamilyId": str,
+        "EbsOptimizedAvailable": bool,
+        "EbsOptimizedByDefault": bool,
+        "NumberOfDisks": int,
+        "EbsStorageOnly": bool,
+        "Architecture": str,
+    },
+    total=False,
+)
+
 _RequiredModifyClusterInputRequestTypeDef = TypedDict(
     "_RequiredModifyClusterInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalModifyClusterInputRequestTypeDef = TypedDict(
@@ -1219,24 +1472,78 @@
 )
 
 class ModifyClusterInputRequestTypeDef(
     _RequiredModifyClusterInputRequestTypeDef, _OptionalModifyClusterInputRequestTypeDef
 ):
     pass
 
+ModifyClusterOutputTypeDef = TypedDict(
+    "ModifyClusterOutputTypeDef",
+    {
+        "StepConcurrencyLevel": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+NotebookS3LocationForOutputTypeDef = TypedDict(
+    "NotebookS3LocationForOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
+)
+
+OutputNotebookS3LocationForOutputTypeDef = TypedDict(
+    "OutputNotebookS3LocationForOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
+)
+
+NotebookS3LocationFromInputTypeDef = TypedDict(
+    "NotebookS3LocationFromInputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
+)
+
 OnDemandCapacityReservationOptionsTypeDef = TypedDict(
     "OnDemandCapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
         "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
         "CapacityReservationResourceGroupArn": str,
     },
     total=False,
 )
 
+OutputNotebookS3LocationFromInputTypeDef = TypedDict(
+    "OutputNotebookS3LocationFromInputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+    total=False,
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
 RemoveAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
     },
 )
@@ -1259,23 +1566,43 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
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
 SupportedProductConfigTypeDef = TypedDict(
     "SupportedProductConfigTypeDef",
     {
         "Name": str,
         "Args": Sequence[str],
     },
     total=False,
 )
 
+RunJobFlowOutputTypeDef = TypedDict(
+    "RunJobFlowOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSimpleScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredSimpleScalingPolicyConfigurationTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalSimpleScalingPolicyConfigurationTypeDef = TypedDict(
@@ -1305,14 +1632,22 @@
     "SetVisibleToAllUsersInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "VisibleToAllUsers": bool,
     },
 )
 
+StartNotebookExecutionOutputTypeDef = TypedDict(
+    "StartNotebookExecutionOutputTypeDef",
+    {
+        "NotebookExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStepExecutionStatusDetailTypeDef = TypedDict(
     "_RequiredStepExecutionStatusDetailTypeDef",
     {
         "State": StepExecutionStateType,
         "CreationDateTime": datetime,
     },
 )
@@ -1405,111 +1740,14 @@
 
 class UpdateStudioSessionMappingInputRequestTypeDef(
     _RequiredUpdateStudioSessionMappingInputRequestTypeDef,
     _OptionalUpdateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
-AddInstanceFleetOutputTypeDef = TypedDict(
-    "AddInstanceFleetOutputTypeDef",
-    {
-        "ClusterId": str,
-        "InstanceFleetId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddInstanceGroupsOutputTypeDef = TypedDict(
-    "AddInstanceGroupsOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "InstanceGroupIds": List[str],
-        "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddJobFlowStepsOutputTypeDef = TypedDict(
-    "AddJobFlowStepsOutputTypeDef",
-    {
-        "StepIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSecurityConfigurationOutputTypeDef = TypedDict(
-    "CreateSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "CreationDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStudioOutputTypeDef = TypedDict(
-    "CreateStudioOutputTypeDef",
-    {
-        "StudioId": str,
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSecurityConfigurationOutputTypeDef = TypedDict(
-    "DescribeSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "SecurityConfiguration": str,
-        "CreationDateTime": datetime,
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
-ListReleaseLabelsOutputTypeDef = TypedDict(
-    "ListReleaseLabelsOutputTypeDef",
-    {
-        "ReleaseLabels": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyClusterOutputTypeDef = TypedDict(
-    "ModifyClusterOutputTypeDef",
-    {
-        "StepConcurrencyLevel": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunJobFlowOutputTypeDef = TypedDict(
-    "RunJobFlowOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartNotebookExecutionOutputTypeDef = TypedDict(
-    "StartNotebookExecutionOutputTypeDef",
-    {
-        "NotebookExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1577,15 +1815,15 @@
     total=False,
 )
 
 GetAutoTerminationPolicyOutputTypeDef = TypedDict(
     "GetAutoTerminationPolicyOutputTypeDef",
     {
         "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutAutoTerminationPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutAutoTerminationPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -1632,15 +1870,15 @@
     },
 )
 
 CancelStepsOutputTypeDef = TypedDict(
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCloudWatchAlarmDefinitionTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
@@ -1668,24 +1906,25 @@
 
 ClusterStatusTypeDef = TypedDict(
     "ClusterStatusTypeDef",
     {
         "State": ClusterStateType,
         "StateChangeReason": ClusterStateChangeReasonTypeDef,
         "Timeline": ClusterTimelineTypeDef,
+        "ErrorDetails": List[ErrorDetailTypeDef],
     },
     total=False,
 )
 
 ListBootstrapActionsOutputTypeDef = TypedDict(
     "ListBootstrapActionsOutputTypeDef",
     {
         "BootstrapActions": List[CommandTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ManagedScalingPolicyTypeDef = TypedDict(
     "ManagedScalingPolicyTypeDef",
     {
         "ComputeLimits": ComputeLimitsTypeDef,
@@ -1765,15 +2004,15 @@
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEbsBlockDeviceConfigTypeDef = TypedDict(
     "_RequiredEbsBlockDeviceConfigTypeDef",
     {
         "VolumeSpecification": VolumeSpecificationTypeDef,
@@ -1797,65 +2036,19 @@
     {
         "VolumeSpecification": VolumeSpecificationTypeDef,
         "Device": str,
     },
     total=False,
 )
 
-NotebookExecutionTypeDef = TypedDict(
-    "NotebookExecutionTypeDef",
-    {
-        "NotebookExecutionId": str,
-        "EditorId": str,
-        "ExecutionEngine": ExecutionEngineConfigTypeDef,
-        "NotebookExecutionName": str,
-        "NotebookParams": str,
-        "Status": NotebookExecutionStatusType,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "Arn": str,
-        "OutputNotebookURI": str,
-        "LastStateChangeReason": str,
-        "NotebookInstanceSecurityGroupId": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-_RequiredStartNotebookExecutionInputRequestTypeDef = TypedDict(
-    "_RequiredStartNotebookExecutionInputRequestTypeDef",
-    {
-        "EditorId": str,
-        "RelativePath": str,
-        "ExecutionEngine": ExecutionEngineConfigTypeDef,
-        "ServiceRole": str,
-    },
-)
-_OptionalStartNotebookExecutionInputRequestTypeDef = TypedDict(
-    "_OptionalStartNotebookExecutionInputRequestTypeDef",
-    {
-        "NotebookExecutionName": str,
-        "NotebookParams": str,
-        "NotebookInstanceSecurityGroupId": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class StartNotebookExecutionInputRequestTypeDef(
-    _RequiredStartNotebookExecutionInputRequestTypeDef,
-    _OptionalStartNotebookExecutionInputRequestTypeDef,
-):
-    pass
-
 GetStudioSessionMappingOutputTypeDef = TypedDict(
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHadoopJarStepConfigTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigTypeDef",
     {
         "Jar": str,
@@ -1950,232 +2143,146 @@
 )
 
 class JobFlowInstancesDetailTypeDef(
     _RequiredJobFlowInstancesDetailTypeDef, _OptionalJobFlowInstancesDetailTypeDef
 ):
     pass
 
-_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+ListReleaseLabelsInputRequestTypeDef = TypedDict(
+    "ListReleaseLabelsInputRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": ReleaseLabelFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
-class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
-    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-):
-    pass
-
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
+ListSecurityConfigurationsOutputTypeDef = TypedDict(
+    "ListSecurityConfigurationsOutputTypeDef",
     {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ClusterStates": Sequence[ClusterStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "SecurityConfigurations": List[SecurityConfigurationSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+ListStudioSessionMappingsOutputTypeDef = TypedDict(
+    "ListStudioSessionMappingsOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "SessionMappings": List[SessionMappingSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
-    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+ListStudiosOutputTypeDef = TypedDict(
+    "ListStudiosOutputTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Studios": List[StudioSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
-    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
+ListSupportedInstanceTypesOutputTypeDef = TypedDict(
+    "ListSupportedInstanceTypesOutputTypeDef",
     {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
-    {
-        "InstanceGroupId": str,
-        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
-        "InstanceFleetId": str,
-        "InstanceFleetType": InstanceFleetTypeType,
-        "InstanceStates": Sequence[InstanceStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "SupportedInstanceTypes": List[SupportedInstanceTypeTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListInstancesInputListInstancesPaginateTypeDef(
-    _RequiredListInstancesInputListInstancesPaginateTypeDef,
-    _OptionalListInstancesInputListInstancesPaginateTypeDef,
-):
-    pass
-
-ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
+NotebookExecutionSummaryTypeDef = TypedDict(
+    "NotebookExecutionSummaryTypeDef",
     {
+        "NotebookExecutionId": str,
         "EditorId": str,
+        "NotebookExecutionName": str,
         "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
+        "ExecutionEngineId": str,
     },
     total=False,
 )
 
-ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+NotebookExecutionTypeDef = TypedDict(
+    "NotebookExecutionTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NotebookExecutionId": str,
+        "EditorId": str,
+        "ExecutionEngine": ExecutionEngineConfigTypeDef,
+        "NotebookExecutionName": str,
+        "NotebookParams": str,
+        "Status": NotebookExecutionStatusType,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "Arn": str,
+        "OutputNotebookURI": str,
+        "LastStateChangeReason": str,
+        "NotebookInstanceSecurityGroupId": str,
+        "Tags": List[TagTypeDef],
+        "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
+        "OutputNotebookS3Location": OutputNotebookS3LocationForOutputTypeDef,
+        "OutputNotebookFormat": Literal["HTML"],
+        "EnvironmentVariables": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_RequiredListStepsInputListStepsPaginateTypeDef",
+_RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
+    "_RequiredOnDemandProvisioningSpecificationTypeDef",
     {
-        "ClusterId": str,
+        "AllocationStrategy": Literal["lowest-price"],
     },
 )
-_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_OptionalListStepsInputListStepsPaginateTypeDef",
+_OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
+    "_OptionalOnDemandProvisioningSpecificationTypeDef",
     {
-        "StepStates": Sequence[StepStateType],
-        "StepIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "CapacityReservationOptions": OnDemandCapacityReservationOptionsTypeDef,
     },
     total=False,
 )
 
-class ListStepsInputListStepsPaginateTypeDef(
-    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
+class OnDemandProvisioningSpecificationTypeDef(
+    _RequiredOnDemandProvisioningSpecificationTypeDef,
+    _OptionalOnDemandProvisioningSpecificationTypeDef,
 ):
     pass
 
-ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
-    {
-        "StudioId": str,
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosInputListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListNotebookExecutionsOutputTypeDef = TypedDict(
-    "ListNotebookExecutionsOutputTypeDef",
-    {
-        "NotebookExecutions": List[NotebookExecutionSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReleaseLabelsInputRequestTypeDef = TypedDict(
-    "ListReleaseLabelsInputRequestTypeDef",
-    {
-        "Filters": ReleaseLabelFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSecurityConfigurationsOutputTypeDef = TypedDict(
-    "ListSecurityConfigurationsOutputTypeDef",
-    {
-        "SecurityConfigurations": List[SecurityConfigurationSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStudioSessionMappingsOutputTypeDef = TypedDict(
-    "ListStudioSessionMappingsOutputTypeDef",
-    {
-        "SessionMappings": List[SessionMappingSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStudiosOutputTypeDef = TypedDict(
-    "ListStudiosOutputTypeDef",
-    {
-        "Studios": List[StudioSummaryTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
-    "_RequiredOnDemandProvisioningSpecificationTypeDef",
+_RequiredStartNotebookExecutionInputRequestTypeDef = TypedDict(
+    "_RequiredStartNotebookExecutionInputRequestTypeDef",
     {
-        "AllocationStrategy": Literal["lowest-price"],
+        "ExecutionEngine": ExecutionEngineConfigTypeDef,
+        "ServiceRole": str,
     },
 )
-_OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
-    "_OptionalOnDemandProvisioningSpecificationTypeDef",
+_OptionalStartNotebookExecutionInputRequestTypeDef = TypedDict(
+    "_OptionalStartNotebookExecutionInputRequestTypeDef",
     {
-        "CapacityReservationOptions": OnDemandCapacityReservationOptionsTypeDef,
+        "EditorId": str,
+        "RelativePath": str,
+        "NotebookExecutionName": str,
+        "NotebookParams": str,
+        "NotebookInstanceSecurityGroupId": str,
+        "Tags": Sequence[TagTypeDef],
+        "NotebookS3Location": NotebookS3LocationFromInputTypeDef,
+        "OutputNotebookS3Location": OutputNotebookS3LocationFromInputTypeDef,
+        "OutputNotebookFormat": Literal["HTML"],
+        "EnvironmentVariables": Mapping[str, str],
     },
     total=False,
 )
 
-class OnDemandProvisioningSpecificationTypeDef(
-    _RequiredOnDemandProvisioningSpecificationTypeDef,
-    _OptionalOnDemandProvisioningSpecificationTypeDef,
+class StartNotebookExecutionInputRequestTypeDef(
+    _RequiredStartNotebookExecutionInputRequestTypeDef,
+    _OptionalStartNotebookExecutionInputRequestTypeDef,
 ):
     pass
 
 _RequiredScalingActionTypeDef = TypedDict(
     "_RequiredScalingActionTypeDef",
     {
         "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationTypeDef,
@@ -2203,24 +2310,24 @@
     total=False,
 )
 
 DescribeStudioOutputTypeDef = TypedDict(
     "DescribeStudioOutputTypeDef",
     {
         "Studio": StudioTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
@@ -2293,15 +2400,15 @@
     total=False,
 )
 
 GetManagedScalingPolicyOutputTypeDef = TypedDict(
     "GetManagedScalingPolicyOutputTypeDef",
     {
         "ManagedScalingPolicy": ManagedScalingPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedScalingPolicyInputRequestTypeDef = TypedDict(
     "PutManagedScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -2310,15 +2417,15 @@
 )
 
 GetClusterSessionCredentialsOutputTypeDef = TypedDict(
     "GetClusterSessionCredentialsOutputTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "ExpiresAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EbsConfigurationTypeDef = TypedDict(
     "EbsConfigurationTypeDef",
     {
         "EbsBlockDeviceConfigs": Sequence[EbsBlockDeviceConfigTypeDef],
@@ -2338,22 +2445,14 @@
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
         "CustomAmiId": str,
     },
     total=False,
 )
 
-DescribeNotebookExecutionOutputTypeDef = TypedDict(
-    "DescribeNotebookExecutionOutputTypeDef",
-    {
-        "NotebookExecution": NotebookExecutionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredStepConfigTypeDef = TypedDict(
     "_RequiredStepConfigTypeDef",
     {
         "Name": str,
         "HadoopJarStep": HadoopJarStepConfigTypeDef,
     },
 )
@@ -2427,14 +2526,31 @@
         "Market": MarketTypeType,
         "InstanceType": str,
         "EbsVolumes": List[EbsVolumeTypeDef],
     },
     total=False,
 )
 
+ListNotebookExecutionsOutputTypeDef = TypedDict(
+    "ListNotebookExecutionsOutputTypeDef",
+    {
+        "NotebookExecutions": List[NotebookExecutionSummaryTypeDef],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeNotebookExecutionOutputTypeDef = TypedDict(
+    "DescribeNotebookExecutionOutputTypeDef",
+    {
+        "NotebookExecution": NotebookExecutionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InstanceFleetProvisioningSpecificationsTypeDef = TypedDict(
     "InstanceFleetProvisioningSpecificationsTypeDef",
     {
         "SpotSpecification": SpotProvisioningSpecificationTypeDef,
         "OnDemandSpecification": OnDemandProvisioningSpecificationTypeDef,
     },
     total=False,
@@ -2485,23 +2601,23 @@
     pass
 
 ListClustersOutputTypeDef = TypedDict(
     "ListClustersOutputTypeDef",
     {
         "Clusters": List[ClusterSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterOutputTypeDef = TypedDict(
     "DescribeClusterOutputTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInstanceTypeConfigTypeDef = TypedDict(
     "_RequiredInstanceTypeConfigTypeDef",
     {
         "InstanceType": str,
@@ -2571,15 +2687,15 @@
 )
 
 ListInstancesOutputTypeDef = TypedDict(
     "ListInstancesOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceFleetTypeDef = TypedDict(
     "InstanceFleetTypeDef",
     {
         "Id": str,
@@ -2598,23 +2714,23 @@
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
         "Steps": List[StepSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStepOutputTypeDef = TypedDict(
     "DescribeStepOutputTypeDef",
     {
         "Step": StepTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
@@ -2687,15 +2803,15 @@
     pass
 
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceGroupTypeDef = TypedDict(
     "InstanceGroupTypeDef",
     {
         "Id": str,
@@ -2723,15 +2839,15 @@
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
     "PutAutoScalingPolicyOutputTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "ClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInstanceGroupConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupConfigTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
@@ -2775,24 +2891,24 @@
     },
 )
 
 DescribeJobFlowsOutputTypeDef = TypedDict(
     "DescribeJobFlowsOutputTypeDef",
     {
         "JobFlows": List[JobFlowDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstanceGroupsOutputTypeDef = TypedDict(
     "ListInstanceGroupsOutputTypeDef",
     {
         "InstanceGroups": List[InstanceGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddInstanceGroupsInputRequestTypeDef = TypedDict(
     "AddInstanceGroupsInputRequestTypeDef",
     {
         "InstanceGroups": Sequence[InstanceGroupConfigTypeDef],
```

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.26.73
-Summary: Type annotations for boto3.EMR 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EMR 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,14 +389,15 @@
     ListStudioSessionMappingsPaginatorName,
     ListStudiosPaginatorName,
     MarketTypeType,
     NotebookExecutionStatusType,
     OnDemandCapacityReservationPreferenceType,
     OnDemandCapacityReservationUsageStrategyType,
     OnDemandProvisioningAllocationStrategyType,
+    OutputNotebookFormatType,
     PlacementGroupStrategyType,
     ReconfigurationTypeType,
     RepoUpgradeOnBootType,
     ScaleDownBehaviorType,
     SpotProvisioningAllocationStrategyType,
     SpotProvisioningTimeoutActionType,
     StatisticType,
@@ -424,52 +425,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
-    ResponseMetadataTypeDef,
+    AddInstanceFleetOutputTypeDef,
+    AddInstanceGroupsOutputTypeDef,
+    AddJobFlowStepsOutputTypeDef,
     TagTypeDef,
     ApplicationTypeDef,
     ScalingConstraintsTypeDef,
     AutoScalingPolicyStateChangeReasonTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
     PortRangeTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
+    ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
     KerberosAttributesTypeDef,
     PlacementGroupConfigTypeDef,
     CommandTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
+    CreateSecurityConfigurationOutputTypeDef,
+    CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
     DescribeJobFlowsInputRequestTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
+    DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
     EbsVolumeTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
@@ -484,58 +492,67 @@
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
-    PaginatorConfigTypeDef,
+    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
+    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
+    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
+    ListInstancesInputListInstancesPaginateTypeDef,
     ListInstancesInputRequestTypeDef,
+    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
     ListNotebookExecutionsInputRequestTypeDef,
-    NotebookExecutionSummaryTypeDef,
     ReleaseLabelFilterTypeDef,
+    ListReleaseLabelsOutputTypeDef,
+    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
+    ListStepsInputListStepsPaginateTypeDef,
     ListStepsInputRequestTypeDef,
+    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
+    ListStudiosInputListStudiosPaginateTypeDef,
     ListStudiosInputRequestTypeDef,
     StudioSummaryTypeDef,
+    ListSupportedInstanceTypesInputRequestTypeDef,
+    SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
+    ModifyClusterOutputTypeDef,
+    NotebookS3LocationForOutputTypeDef,
+    OutputNotebookS3LocationForOutputTypeDef,
+    NotebookS3LocationFromInputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
+    OutputNotebookS3LocationFromInputTypeDef,
+    PaginatorConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
+    RunJobFlowOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
+    StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
-    AddInstanceFleetOutputTypeDef,
-    AddInstanceGroupsOutputTypeDef,
-    AddJobFlowStepsOutputTypeDef,
-    CreateSecurityConfigurationOutputTypeDef,
-    CreateStudioOutputTypeDef,
-    DescribeSecurityConfigurationOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListReleaseLabelsOutputTypeDef,
-    ModifyClusterOutputTypeDef,
-    RunJobFlowOutputTypeDef,
-    StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
     StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationTypeDef,
@@ -548,59 +565,51 @@
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
-    NotebookExecutionTypeDef,
-    StartNotebookExecutionInputRequestTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
-    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
-    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    ListInstancesInputListInstancesPaginateTypeDef,
-    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
-    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
-    ListStepsInputListStepsPaginateTypeDef,
-    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
-    ListStudiosInputListStudiosPaginateTypeDef,
-    ListNotebookExecutionsOutputTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
+    ListSupportedInstanceTypesOutputTypeDef,
+    NotebookExecutionSummaryTypeDef,
+    NotebookExecutionTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
+    StartNotebookExecutionInputRequestTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
     DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
-    DescribeNotebookExecutionOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
+    ListNotebookExecutionsOutputTypeDef,
+    DescribeNotebookExecutionOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
     InstanceTypeConfigTypeDef,
@@ -626,53 +635,53 @@
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> AddInstanceFleetOutputTypeDef:
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

### Comparing `mypy-boto3-emr-1.26.73/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.26.73/setup.py` & `mypy-boto3-emr-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-emr.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.26.73",
+    version="1.27.0",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.26.73 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.EMR 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/",
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


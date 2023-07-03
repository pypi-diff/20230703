# Comparing `tmp/mypy-boto3-autoscaling-1.26.7.tar.gz` & `tmp/mypy-boto3-autoscaling-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-1.26.7.tar", last modified: Thu Nov 10 20:32:39 2022, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-1.26.7.tar` & `mypy-boto3-autoscaling-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.501201 mypy-boto3-autoscaling-1.26.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22181 2022-11-10 20:32:39.493201 mypy-boto3-autoscaling-1.26.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20730 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.489201 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    50191 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    50113 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12561 2022-11-10 20:31:33.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12559 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13271 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13259 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    71017 2022-11-10 20:31:34.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    70906 2022-11-10 20:31:34.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:32:39.493201 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22181 2022-11-10 20:32:39.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-10 20:32:39.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:32:39.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-10 20:32:39.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-10 20:32:39.000000 mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 20:32:39.501201 mypy-boto3-autoscaling-1.26.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-10 20:31:32.000000 mypy-boto3-autoscaling-1.26.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.798862 mypy-boto3-autoscaling-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-07-03 19:50:24.798862 mypy-boto3-autoscaling-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.798862 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52425 2023-07-03 19:32:56.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52343 2023-07-03 19:32:56.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-03 19:32:56.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-03 19:32:56.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-03 19:32:56.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-03 19:32:56.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75407 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75290 2023-07-03 19:32:57.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.798862 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.798862 mypy-boto3-autoscaling-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:32:55.000000 mypy-boto3-autoscaling-1.27.0/setup.py
```

### Comparing `mypy-boto3-autoscaling-1.26.7/LICENSE` & `mypy-boto3-autoscaling-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-autoscaling-1.26.7/PKG-INFO` & `mypy-boto3-autoscaling-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.26.7
-Summary: Type annotations for boto3.AutoScaling 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AutoScaling 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
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
 
 <a id="mypy-boto3-autoscaling"></a>
 
 # mypy-boto3-autoscaling
 
 [![PyPI - mypy-boto3-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,15 +363,17 @@
     MetricTypeType,
     PredefinedLoadMetricTypeType,
     PredefinedMetricPairTypeType,
     PredefinedScalingMetricTypeType,
     PredictiveScalingMaxCapacityBreachBehaviorType,
     PredictiveScalingModeType,
     RefreshStrategyType,
+    ScaleInProtectedInstancesType,
     ScalingActivityStatusCodeType,
+    StandbyInstancesType,
     WarmPoolStateType,
     WarmPoolStatusType,
     AutoScalingServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -389,65 +392,79 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
-    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
+    TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsTypeRequestTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
+    DescribeTrafficSourcesRequestRequestTypeDef,
+    TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
@@ -457,94 +474,91 @@
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
+    ResponseMetadataTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
-    AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeRequestTypeDef,
+    AttachTrafficSourcesTypeRequestTypeDef,
+    DetachTrafficSourcesTypeRequestTypeDef,
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    AutoScalingGroupNamesTypeRequestTypeDef,
     DescribeTagsTypeDescribeTagsPaginateTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
+    DescribeTagsTypeRequestTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
-    CustomizedMetricSpecificationTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
-    TargetTrackingConfigurationTypeDef,
     MetricStatTypeDef,
+    TargetTrackingMetricStatTypeDef,
+    RollbackDetailsTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
     MetricDataQueryTypeDef,
+    TargetTrackingMetricDataQueryTypeDef,
     LaunchTemplateTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
+    CustomizedMetricSpecificationTypeDef,
     MixedInstancesPolicyTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
+    TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
     PredictiveScalingConfigurationTypeDef,
     AutoScalingGroupsTypeTypeDef,
@@ -565,42 +579,42 @@
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

### Comparing `mypy-boto3-autoscaling-1.26.7/README.md` & `mypy-boto3-autoscaling-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-autoscaling"></a>
 
 # mypy-boto3-autoscaling
 
 [![PyPI - mypy-boto3-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,15 +331,17 @@
     MetricTypeType,
     PredefinedLoadMetricTypeType,
     PredefinedMetricPairTypeType,
     PredefinedScalingMetricTypeType,
     PredictiveScalingMaxCapacityBreachBehaviorType,
     PredictiveScalingModeType,
     RefreshStrategyType,
+    ScaleInProtectedInstancesType,
     ScalingActivityStatusCodeType,
+    StandbyInstancesType,
     WarmPoolStateType,
     WarmPoolStatusType,
     AutoScalingServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -358,65 +360,79 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
-    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
+    TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsTypeRequestTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
+    DescribeTrafficSourcesRequestRequestTypeDef,
+    TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
@@ -426,94 +442,91 @@
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
+    ResponseMetadataTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
-    AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeRequestTypeDef,
+    AttachTrafficSourcesTypeRequestTypeDef,
+    DetachTrafficSourcesTypeRequestTypeDef,
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    AutoScalingGroupNamesTypeRequestTypeDef,
     DescribeTagsTypeDescribeTagsPaginateTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
+    DescribeTagsTypeRequestTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
-    CustomizedMetricSpecificationTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
-    TargetTrackingConfigurationTypeDef,
     MetricStatTypeDef,
+    TargetTrackingMetricStatTypeDef,
+    RollbackDetailsTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
     MetricDataQueryTypeDef,
+    TargetTrackingMetricDataQueryTypeDef,
     LaunchTemplateTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
+    CustomizedMetricSpecificationTypeDef,
     MixedInstancesPolicyTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
+    TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
     PredictiveScalingConfigurationTypeDef,
     AutoScalingGroupsTypeTypeDef,
@@ -534,42 +547,42 @@
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

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/__init__.py` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/__init__.pyi` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/__main__.py` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScaling 1.26.7\nVersion:         1.26.7\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.AutoScaling 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.7")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/client.py` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLifecycleHookTypesAnswerTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
+    DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     DesiredConfigurationTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
@@ -68,21 +69,23 @@
     LifecycleHookSpecificationTypeDef,
     MixedInstancesPolicyTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
     PredictiveScalingConfigurationTypeDef,
     ProcessesTypeTypeDef,
     RefreshPreferencesTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
     TargetTrackingConfigurationTypeDef,
+    TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -100,14 +103,15 @@
 
 class Exceptions:
     ActiveInstanceRefreshNotFoundFault: Type[BotocoreClientError]
     AlreadyExistsFault: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InstanceRefreshInProgressFault: Type[BotocoreClientError]
     InvalidNextToken: Type[BotocoreClientError]
+    IrreversibleInstanceRefreshFault: Type[BotocoreClientError]
     LimitExceededFault: Type[BotocoreClientError]
     ResourceContentionFault: Type[BotocoreClientError]
     ResourceInUseFault: Type[BotocoreClientError]
     ScalingActivityInProgressFault: Type[BotocoreClientError]
     ServiceLinkedRoleFailure: Type[BotocoreClientError]
 
 
@@ -138,15 +142,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_instances)
         """
 
     def attach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
-        Attaches one or more target groups to the specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancer_target_groups)
         """
 
     def attach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
@@ -154,14 +158,24 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancers)
         """
 
+    def attach_traffic_sources(
+        self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Attaches one or more traffic sources to the specified Auto Scaling group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_traffic_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_traffic_sources)
+        """
+
     def batch_delete_scheduled_action(
         self, *, AutoScalingGroupName: str, ScheduledActionNames: Sequence[str]
     ) -> BatchDeleteScheduledActionAnswerTypeDef:
         """
         Deletes one or more scheduled actions for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_delete_scheduled_action)
@@ -190,15 +204,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#can_paginate)
         """
 
     def cancel_instance_refresh(
         self, *, AutoScalingGroupName: str
     ) -> CancelInstanceRefreshAnswerTypeDef:
         """
-        Cancels an instance refresh operation in progress.
+        Cancels an instance refresh or rollback that is in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.cancel_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#cancel_instance_refresh)
         """
 
     def close(self) -> None:
         """
@@ -249,15 +263,16 @@
         CapacityRebalance: bool = ...,
         LifecycleHookSpecificationList: Sequence[LifecycleHookSpecificationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ServiceLinkedRoleARN: str = ...,
         MaxInstanceLifetime: int = ...,
         Context: str = ...,
         DesiredCapacityType: str = ...,
-        DefaultInstanceWarmup: int = ...
+        DefaultInstanceWarmup: int = ...,
+        TrafficSources: Sequence[TrafficSourceIdentifierTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         **We strongly recommend using a launch template when calling this operation to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Creates
         an Auto Scaling group with the specified name and attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_auto_scaling_group)
@@ -480,26 +495,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_lifecycle_hooks)
         """
 
     def describe_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancerTargetGroupsResponseTypeDef:
         """
-        Gets information about the Elastic Load Balancing target groups for the
-        specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancer_target_groups)
         """
 
     def describe_load_balancers(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancersResponseTypeDef:
         """
-        Gets information about the load balancers for the specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancers)
         """
 
     def describe_metric_collection_types(self) -> DescribeMetricCollectionTypesAnswerTypeDef:
         """
@@ -597,14 +611,29 @@
         """
         Describes the termination policies supported by Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_termination_policy_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_termination_policy_types)
         """
 
+    def describe_traffic_sources(
+        self,
+        *,
+        AutoScalingGroupName: str,
+        TrafficSourceType: str = ...,
+        NextToken: str = ...,
+        MaxRecords: int = ...
+    ) -> DescribeTrafficSourcesResponseTypeDef:
+        """
+        Gets information about the traffic sources for the specified Auto Scaling group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_traffic_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_traffic_sources)
+        """
+
     def describe_warm_pool(
         self, *, AutoScalingGroupName: str, MaxRecords: int = ..., NextToken: str = ...
     ) -> DescribeWarmPoolAnswerTypeDef:
         """
         Gets information about a warm pool and its instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_warm_pool)
@@ -625,31 +654,40 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_instances)
         """
 
     def detach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
-        Detaches one or more target groups from the specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancer_target_groups)
         """
 
     def detach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
-        Detaches one or more Classic Load Balancers from the specified Auto Scaling
-        group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancers)
         """
 
+    def detach_traffic_sources(
+        self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Detaches one or more traffic sources from the specified Auto Scaling group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_traffic_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_traffic_sources)
+        """
+
     def disable_metrics_collection(
         self, *, AutoScalingGroupName: str, Metrics: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disables group metrics collection for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.disable_metrics_collection)
@@ -850,14 +888,25 @@
         Resumes the specified suspended auto scaling processes, or all suspended
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#resume_processes)
         """
 
+    def rollback_instance_refresh(
+        self, *, AutoScalingGroupName: str = ...
+    ) -> RollbackInstanceRefreshAnswerTypeDef:
+        """
+        Cancels an instance refresh that is in progress and rolls back any changes that
+        it made.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#rollback_instance_refresh)
+        """
+
     def set_desired_capacity(
         self, *, AutoScalingGroupName: str, DesiredCapacity: int, HonorCooldown: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the size of the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_desired_capacity)
@@ -889,15 +938,15 @@
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
         DesiredConfiguration: DesiredConfigurationTypeDef = ...,
         Preferences: RefreshPreferencesTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
-        Starts a new instance refresh operation.
+        Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#start_instance_refresh)
         """
 
     def suspend_processes(
         self, *, AutoScalingGroupName: str, ScalingProcesses: Sequence[str] = ...
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/client.pyi` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLifecycleHookTypesAnswerTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
+    DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     DesiredConfigurationTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
@@ -68,21 +69,23 @@
     LifecycleHookSpecificationTypeDef,
     MixedInstancesPolicyTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
     PredictiveScalingConfigurationTypeDef,
     ProcessesTypeTypeDef,
     RefreshPreferencesTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
     TargetTrackingConfigurationTypeDef,
+    TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -97,14 +100,15 @@
 
 class Exceptions:
     ActiveInstanceRefreshNotFoundFault: Type[BotocoreClientError]
     AlreadyExistsFault: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InstanceRefreshInProgressFault: Type[BotocoreClientError]
     InvalidNextToken: Type[BotocoreClientError]
+    IrreversibleInstanceRefreshFault: Type[BotocoreClientError]
     LimitExceededFault: Type[BotocoreClientError]
     ResourceContentionFault: Type[BotocoreClientError]
     ResourceInUseFault: Type[BotocoreClientError]
     ScalingActivityInProgressFault: Type[BotocoreClientError]
     ServiceLinkedRoleFailure: Type[BotocoreClientError]
 
 class AutoScalingClient(BaseClient):
@@ -132,28 +136,37 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_instances)
         """
     def attach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
-        Attaches one or more target groups to the specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancer_target_groups)
         """
     def attach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_load_balancers)
         """
+    def attach_traffic_sources(
+        self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Attaches one or more traffic sources to the specified Auto Scaling group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.attach_traffic_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#attach_traffic_sources)
+        """
     def batch_delete_scheduled_action(
         self, *, AutoScalingGroupName: str, ScheduledActionNames: Sequence[str]
     ) -> BatchDeleteScheduledActionAnswerTypeDef:
         """
         Deletes one or more scheduled actions for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.batch_delete_scheduled_action)
@@ -179,15 +192,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#can_paginate)
         """
     def cancel_instance_refresh(
         self, *, AutoScalingGroupName: str
     ) -> CancelInstanceRefreshAnswerTypeDef:
         """
-        Cancels an instance refresh operation in progress.
+        Cancels an instance refresh or rollback that is in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.cancel_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#cancel_instance_refresh)
         """
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
@@ -235,15 +248,16 @@
         CapacityRebalance: bool = ...,
         LifecycleHookSpecificationList: Sequence[LifecycleHookSpecificationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ServiceLinkedRoleARN: str = ...,
         MaxInstanceLifetime: int = ...,
         Context: str = ...,
         DesiredCapacityType: str = ...,
-        DefaultInstanceWarmup: int = ...
+        DefaultInstanceWarmup: int = ...,
+        TrafficSources: Sequence[TrafficSourceIdentifierTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         **We strongly recommend using a launch template when calling this operation to
         ensure full functionality for Amazon EC2 Auto Scaling and Amazon EC2.** Creates
         an Auto Scaling group with the specified name and attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.create_auto_scaling_group)
@@ -446,25 +460,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_lifecycle_hooks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_lifecycle_hooks)
         """
     def describe_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancerTargetGroupsResponseTypeDef:
         """
-        Gets information about the Elastic Load Balancing target groups for the
-        specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancer_target_groups)
         """
     def describe_load_balancers(
         self, *, AutoScalingGroupName: str, NextToken: str = ..., MaxRecords: int = ...
     ) -> DescribeLoadBalancersResponseTypeDef:
         """
-        Gets information about the load balancers for the specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_load_balancers)
         """
     def describe_metric_collection_types(self) -> DescribeMetricCollectionTypesAnswerTypeDef:
         """
         Describes the available CloudWatch metrics for Amazon EC2 Auto Scaling.
@@ -553,14 +566,28 @@
     def describe_termination_policy_types(self) -> DescribeTerminationPolicyTypesAnswerTypeDef:
         """
         Describes the termination policies supported by Amazon EC2 Auto Scaling.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_termination_policy_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_termination_policy_types)
         """
+    def describe_traffic_sources(
+        self,
+        *,
+        AutoScalingGroupName: str,
+        TrafficSourceType: str = ...,
+        NextToken: str = ...,
+        MaxRecords: int = ...
+    ) -> DescribeTrafficSourcesResponseTypeDef:
+        """
+        Gets information about the traffic sources for the specified Auto Scaling group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_traffic_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#describe_traffic_sources)
+        """
     def describe_warm_pool(
         self, *, AutoScalingGroupName: str, MaxRecords: int = ..., NextToken: str = ...
     ) -> DescribeWarmPoolAnswerTypeDef:
         """
         Gets information about a warm pool and its instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.describe_warm_pool)
@@ -579,29 +606,37 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_instances)
         """
     def detach_load_balancer_target_groups(
         self, *, AutoScalingGroupName: str, TargetGroupARNs: Sequence[str]
     ) -> Dict[str, Any]:
         """
-        Detaches one or more target groups from the specified Auto Scaling group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancer_target_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancer_target_groups)
         """
     def detach_load_balancers(
         self, *, AutoScalingGroupName: str, LoadBalancerNames: Sequence[str]
     ) -> Dict[str, Any]:
         """
-        Detaches one or more Classic Load Balancers from the specified Auto Scaling
-        group.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_load_balancers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_load_balancers)
         """
+    def detach_traffic_sources(
+        self, *, AutoScalingGroupName: str, TrafficSources: Sequence[TrafficSourceIdentifierTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Detaches one or more traffic sources from the specified Auto Scaling group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.detach_traffic_sources)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#detach_traffic_sources)
+        """
     def disable_metrics_collection(
         self, *, AutoScalingGroupName: str, Metrics: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disables group metrics collection for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.disable_metrics_collection)
@@ -788,14 +823,24 @@
         """
         Resumes the specified suspended auto scaling processes, or all suspended
         process, for the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.resume_processes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#resume_processes)
         """
+    def rollback_instance_refresh(
+        self, *, AutoScalingGroupName: str = ...
+    ) -> RollbackInstanceRefreshAnswerTypeDef:
+        """
+        Cancels an instance refresh that is in progress and rolls back any changes that
+        it made.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.rollback_instance_refresh)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#rollback_instance_refresh)
+        """
     def set_desired_capacity(
         self, *, AutoScalingGroupName: str, DesiredCapacity: int, HonorCooldown: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the size of the specified Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.set_desired_capacity)
@@ -824,15 +869,15 @@
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
         DesiredConfiguration: DesiredConfigurationTypeDef = ...,
         Preferences: RefreshPreferencesTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
-        Starts a new instance refresh operation.
+        Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/client/#start_instance_refresh)
         """
     def suspend_processes(
         self, *, AutoScalingGroupName: str, ScalingProcesses: Sequence[str] = ...
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/literals.py` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     "MetricTypeType",
     "PredefinedLoadMetricTypeType",
     "PredefinedMetricPairTypeType",
     "PredefinedScalingMetricTypeType",
     "PredictiveScalingMaxCapacityBreachBehaviorType",
     "PredictiveScalingModeType",
     "RefreshStrategyType",
+    "ScaleInProtectedInstancesType",
     "ScalingActivityStatusCodeType",
+    "StandbyInstancesType",
     "WarmPoolStateType",
     "WarmPoolStatusType",
     "AutoScalingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
@@ -78,15 +80,23 @@
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
 InstanceGenerationType = Literal["current", "previous"]
 InstanceMetadataEndpointStateType = Literal["disabled", "enabled"]
 InstanceMetadataHttpTokensStateType = Literal["optional", "required"]
 InstanceRefreshStatusType = Literal[
-    "Cancelled", "Cancelling", "Failed", "InProgress", "Pending", "Successful"
+    "Cancelled",
+    "Cancelling",
+    "Failed",
+    "InProgress",
+    "Pending",
+    "RollbackFailed",
+    "RollbackInProgress",
+    "RollbackSuccessful",
+    "Successful",
 ]
 LifecycleStateType = Literal[
     "Detached",
     "Detaching",
     "EnteringStandby",
     "InService",
     "Pending",
@@ -132,28 +142,31 @@
     "ASGAverageCPUUtilization",
     "ASGAverageNetworkIn",
     "ASGAverageNetworkOut",
 ]
 PredictiveScalingMaxCapacityBreachBehaviorType = Literal["HonorMaxCapacity", "IncreaseMaxCapacity"]
 PredictiveScalingModeType = Literal["ForecastAndScale", "ForecastOnly"]
 RefreshStrategyType = Literal["Rolling"]
+ScaleInProtectedInstancesType = Literal["Ignore", "Refresh", "Wait"]
 ScalingActivityStatusCodeType = Literal[
     "Cancelled",
     "Failed",
     "InProgress",
     "MidLifecycleAction",
     "PendingSpotBidPlacement",
     "PreInService",
     "Successful",
+    "WaitingForConnectionDraining",
     "WaitingForELBConnectionDraining",
     "WaitingForInstanceId",
     "WaitingForInstanceWarmup",
     "WaitingForSpotInstanceId",
     "WaitingForSpotInstanceRequestId",
 ]
+StandbyInstancesType = Literal["Ignore", "Terminate", "Wait"]
 WarmPoolStateType = Literal["Hibernated", "Running", "Stopped"]
 WarmPoolStatusType = Literal["PendingDelete"]
 AutoScalingServiceName = Literal["autoscaling"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -164,23 +177,25 @@
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
@@ -190,30 +205,35 @@
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
@@ -239,14 +259,15 @@
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
@@ -291,51 +312,57 @@
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
@@ -348,14 +375,15 @@
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
@@ -367,28 +395,35 @@
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
@@ -416,56 +451,64 @@
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
@@ -502,22 +545,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/literals.pyi` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/literals.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -46,15 +46,17 @@
     "MetricTypeType",
     "PredefinedLoadMetricTypeType",
     "PredefinedMetricPairTypeType",
     "PredefinedScalingMetricTypeType",
     "PredictiveScalingMaxCapacityBreachBehaviorType",
     "PredictiveScalingModeType",
     "RefreshStrategyType",
+    "ScaleInProtectedInstancesType",
     "ScalingActivityStatusCodeType",
+    "StandbyInstancesType",
     "WarmPoolStateType",
     "WarmPoolStatusType",
     "AutoScalingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
@@ -76,15 +78,23 @@
 DescribeScalingActivitiesPaginatorName = Literal["describe_scaling_activities"]
 DescribeScheduledActionsPaginatorName = Literal["describe_scheduled_actions"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
 InstanceGenerationType = Literal["current", "previous"]
 InstanceMetadataEndpointStateType = Literal["disabled", "enabled"]
 InstanceMetadataHttpTokensStateType = Literal["optional", "required"]
 InstanceRefreshStatusType = Literal[
-    "Cancelled", "Cancelling", "Failed", "InProgress", "Pending", "Successful"
+    "Cancelled",
+    "Cancelling",
+    "Failed",
+    "InProgress",
+    "Pending",
+    "RollbackFailed",
+    "RollbackInProgress",
+    "RollbackSuccessful",
+    "Successful",
 ]
 LifecycleStateType = Literal[
     "Detached",
     "Detaching",
     "EnteringStandby",
     "InService",
     "Pending",
@@ -130,28 +140,31 @@
     "ASGAverageCPUUtilization",
     "ASGAverageNetworkIn",
     "ASGAverageNetworkOut",
 ]
 PredictiveScalingMaxCapacityBreachBehaviorType = Literal["HonorMaxCapacity", "IncreaseMaxCapacity"]
 PredictiveScalingModeType = Literal["ForecastAndScale", "ForecastOnly"]
 RefreshStrategyType = Literal["Rolling"]
+ScaleInProtectedInstancesType = Literal["Ignore", "Refresh", "Wait"]
 ScalingActivityStatusCodeType = Literal[
     "Cancelled",
     "Failed",
     "InProgress",
     "MidLifecycleAction",
     "PendingSpotBidPlacement",
     "PreInService",
     "Successful",
+    "WaitingForConnectionDraining",
     "WaitingForELBConnectionDraining",
     "WaitingForInstanceId",
     "WaitingForInstanceWarmup",
     "WaitingForSpotInstanceId",
     "WaitingForSpotInstanceRequestId",
 ]
+StandbyInstancesType = Literal["Ignore", "Terminate", "Wait"]
 WarmPoolStateType = Literal["Hibernated", "Running", "Stopped"]
 WarmPoolStatusType = Literal["PendingDelete"]
 AutoScalingServiceName = Literal["autoscaling"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -162,23 +175,25 @@
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
@@ -188,30 +203,35 @@
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
@@ -237,14 +257,15 @@
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
@@ -289,51 +310,57 @@
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
@@ -346,14 +373,15 @@
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
@@ -365,28 +393,35 @@
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
@@ -414,56 +449,64 @@
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
@@ -500,22 +543,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/paginator.py` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,30 +88,30 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AutoScalingGroupsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
 
 class DescribeAutoScalingInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AutoScalingInstancesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
         """
 
 
@@ -121,45 +121,45 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
 
 class DescribeLoadBalancerTargetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
         """
 
 
 class DescribeLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLoadBalancersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
         """
 
 
@@ -169,15 +169,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
 
@@ -189,15 +189,15 @@
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describepoliciespaginator)
         """
 
 
@@ -209,15 +209,15 @@
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 
@@ -230,15 +230,15 @@
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -248,13 +248,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/paginator.pyi` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -85,29 +85,29 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AutoScalingGroupsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
 class DescribeAutoScalingInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AutoScalingInstancesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeautoscalinginstancespaginator)
         """
 
 class DescribeLaunchConfigurationsPaginator(Paginator):
@@ -116,43 +116,43 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
 class DescribeLoadBalancerTargetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
         """
 
 class DescribeLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLoadBalancersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describeloadbalancerspaginator)
         """
 
 class DescribeNotificationConfigurationsPaginator(Paginator):
@@ -161,15 +161,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
 class DescribePoliciesPaginator(Paginator):
@@ -180,15 +180,15 @@
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describepoliciespaginator)
         """
 
 class DescribeScalingActivitiesPaginator(Paginator):
@@ -199,15 +199,15 @@
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 class DescribeScheduledActionsPaginator(Paginator):
@@ -219,15 +219,15 @@
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
@@ -236,13 +236,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/paginators/#describetagspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/type_defs.py` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     MetricStatisticType,
     MetricTypeType,
     PredefinedLoadMetricTypeType,
     PredefinedMetricPairTypeType,
     PredefinedScalingMetricTypeType,
     PredictiveScalingMaxCapacityBreachBehaviorType,
     PredictiveScalingModeType,
+    ScaleInProtectedInstancesType,
     ScalingActivityStatusCodeType,
+    StandbyInstancesType,
     WarmPoolStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -50,65 +52,79 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
-    "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
+    "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsTypeDef",
+    "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
+    "DescribeAccountLimitsAnswerTypeDef",
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
     "DescribeInstanceRefreshesTypeRequestTypeDef",
+    "DescribeLifecycleHookTypesAnswerTypeDef",
     "LifecycleHookTypeDef",
     "DescribeLifecycleHooksTypeRequestTypeDef",
+    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     "LoadBalancerTargetGroupStateTypeDef",
+    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeLoadBalancersRequestRequestTypeDef",
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsTypeRequestTypeDef",
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    "DescribeTrafficSourcesRequestRequestTypeDef",
+    "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
@@ -118,94 +134,91 @@
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "RollbackInstanceRefreshAnswerTypeDef",
+    "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
+    "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
     "ActivityTypeTypeDef",
-    "CancelInstanceRefreshAnswerTypeDef",
-    "DescribeAccountLimitsAnswerTypeDef",
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DetachInstancesAnswerTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
-    "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
     "PolicyARNTypeTypeDef",
-    "AutoScalingGroupNamesTypeRequestTypeDef",
-    "DescribeTagsTypeRequestTypeDef",
+    "AttachTrafficSourcesTypeRequestTypeDef",
+    "DetachTrafficSourcesTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+    "DescribeTagsTypeRequestTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
-    "CustomizedMetricSpecificationTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
+    "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
-    "TargetTrackingConfigurationTypeDef",
     "MetricStatTypeDef",
+    "TargetTrackingMetricStatTypeDef",
+    "RollbackDetailsTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
     "MetricDataQueryTypeDef",
+    "TargetTrackingMetricDataQueryTypeDef",
     "LaunchTemplateTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
+    "CustomizedMetricSpecificationTypeDef",
     "MixedInstancesPolicyTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
+    "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
     "PredictiveScalingConfigurationTypeDef",
     "AutoScalingGroupsTypeTypeDef",
@@ -261,25 +274,14 @@
 )
 
 
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
 
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
 AdjustmentTypeTypeDef = TypedDict(
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
@@ -326,29 +328,40 @@
     "AttachLoadBalancersTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "LoadBalancerNames": Sequence[str],
     },
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+_RequiredTrafficSourceIdentifierTypeDef = TypedDict(
+    "_RequiredTrafficSourceIdentifierTypeDef",
     {
-        "Name": str,
-        "Values": Sequence[str],
+        "Identifier": str,
+    },
+)
+_OptionalTrafficSourceIdentifierTypeDef = TypedDict(
+    "_OptionalTrafficSourceIdentifierTypeDef",
+    {
+        "Type": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+class TrafficSourceIdentifierTypeDef(
+    _RequiredTrafficSourceIdentifierTypeDef, _OptionalTrafficSourceIdentifierTypeDef
+):
+    pass
+
+
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 EnabledMetricTypeDef = TypedDict(
     "EnabledMetricTypeDef",
     {
@@ -467,14 +480,22 @@
         "Iops": int,
         "Encrypted": bool,
         "Throughput": int,
     },
     total=False,
 )
 
+CancelInstanceRefreshAnswerTypeDef = TypedDict(
+    "CancelInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CancelInstanceRefreshTypeRequestTypeDef = TypedDict(
     "CancelInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -669,24 +690,52 @@
 
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
 
+DescribeAccountLimitsAnswerTypeDef = TypedDict(
+    "DescribeAccountLimitsAnswerTypeDef",
+    {
+        "MaxNumberOfAutoScalingGroups": int,
+        "MaxNumberOfLaunchConfigurations": int,
+        "NumberOfAutoScalingGroups": int,
+        "NumberOfLaunchConfigurations": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    {
+        "AutoScalingNotificationTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceRefreshesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
@@ -703,14 +752,22 @@
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
 
+DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    {
+        "LifecycleHookTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -741,14 +798,36 @@
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
+    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -773,14 +852,36 @@
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
 )
 
+_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
+    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
@@ -831,61 +932,147 @@
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationType": str,
     },
     total=False,
 )
 
+DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeNotificationConfigurationsTypeRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyNames": Sequence[str],
+        "PolicyTypes": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribePoliciesTypeRequestTypeDef = TypedDict(
     "DescribePoliciesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyNames": Sequence[str],
         "PolicyTypes": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ActivityIds": Sequence[str],
+        "AutoScalingGroupName": str,
+        "IncludeDeletedGroups": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeScalingActivitiesTypeRequestTypeDef = TypedDict(
     "DescribeScalingActivitiesTypeRequestTypeDef",
     {
         "ActivityIds": Sequence[str],
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
     "DescribeScheduledActionsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    {
+        "TerminationPolicyTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeTrafficSourcesRequestRequestTypeDef",
+    {
+        "TrafficSourceType": str,
+        "NextToken": str,
+        "MaxRecords": int,
+    },
+    total=False,
+)
+
+
+class DescribeTrafficSourcesRequestRequestTypeDef(
+    _RequiredDescribeTrafficSourcesRequestRequestTypeDef,
+    _OptionalDescribeTrafficSourcesRequestRequestTypeDef,
+):
+    pass
+
+
+TrafficSourceStateTypeDef = TypedDict(
+    "TrafficSourceStateTypeDef",
+    {
+        "TrafficSource": str,
+        "State": str,
+        "Identifier": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 _RequiredDescribeWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeWarmPoolTypeRequestTypeDef = TypedDict(
@@ -960,14 +1147,21 @@
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1086,14 +1280,17 @@
     "RefreshPreferencesTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
@@ -1192,24 +1389,43 @@
 LaunchConfigurationNameTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNameTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 
+LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+    {
+        "LaunchConfigurationNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 LaunchConfigurationNamesTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeRequestTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
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
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1406,14 +1622,41 @@
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
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
+RollbackInstanceRefreshAnswerTypeDef = TypedDict(
+    "RollbackInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
+    "RollbackInstanceRefreshTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+    total=False,
+)
+
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalScalingProcessQueryRequestTypeDef = TypedDict(
@@ -1498,279 +1741,140 @@
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
 )
 
+StartInstanceRefreshAnswerTypeDef = TypedDict(
+    "StartInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TerminateInstanceInAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     {
         "InstanceId": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
 
 ActivitiesTypeTypeDef = TypedDict(
     "ActivitiesTypeTypeDef",
     {
         "Activities": List[ActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivityTypeTypeDef = TypedDict(
     "ActivityTypeTypeDef",
     {
         "Activity": ActivityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelInstanceRefreshAnswerTypeDef = TypedDict(
-    "CancelInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountLimitsAnswerTypeDef = TypedDict(
-    "DescribeAccountLimitsAnswerTypeDef",
-    {
-        "MaxNumberOfAutoScalingGroups": int,
-        "MaxNumberOfLaunchConfigurations": int,
-        "NumberOfAutoScalingGroups": int,
-        "NumberOfLaunchConfigurations": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    {
-        "AutoScalingNotificationTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    {
-        "LifecycleHookTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
-    {
-        "TerminationPolicyTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachInstancesAnswerTypeDef = TypedDict(
     "DetachInstancesAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
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
 
 EnterStandbyAnswerTypeDef = TypedDict(
     "EnterStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExitStandbyAnswerTypeDef = TypedDict(
     "ExitStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartInstanceRefreshAnswerTypeDef = TypedDict(
-    "StartInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAdjustmentTypesAnswerTypeDef = TypedDict(
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeRequestTypeDef",
+AttachTrafficSourcesTypeRequestTypeDef = TypedDict(
+    "AttachTrafficSourcesTypeRequestTypeDef",
     {
-        "AutoScalingGroupNames": Sequence[str],
-        "NextToken": str,
-        "MaxRecords": int,
-        "Filters": Sequence[FilterTypeDef],
+        "AutoScalingGroupName": str,
+        "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
-    total=False,
 )
 
-DescribeTagsTypeRequestTypeDef = TypedDict(
-    "DescribeTagsTypeRequestTypeDef",
+DetachTrafficSourcesTypeRequestTypeDef = TypedDict(
+    "DetachTrafficSourcesTypeRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "NextToken": str,
-        "MaxRecords": int,
+        "AutoScalingGroupName": str,
+        "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
-    total=False,
 )
 
 AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
-    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
-    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-):
-    pass
-
-
-DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyNames": Sequence[str],
-        "PolicyTypes": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ActivityIds": Sequence[str],
-        "AutoScalingGroupName": str,
-        "IncludeDeletedGroups": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxRecords": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+DescribeTagsTypeRequestTypeDef = TypedDict(
+    "DescribeTagsTypeRequestTypeDef",
     {
-        "LaunchConfigurationNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": Sequence[FilterTypeDef],
+        "NextToken": str,
+        "MaxRecords": int,
     },
     total=False,
 )
 
 _RequiredAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_RequiredAutoScalingInstanceDetailsTypeDef",
     {
@@ -1827,31 +1931,31 @@
 
 
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteScheduledActionAnswerTypeDef = TypedDict(
     "BatchDeleteScheduledActionAnswerTypeDef",
     {
         "FailedScheduledActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutScheduledUpdateGroupActionAnswerTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -1892,38 +1996,14 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredCustomizedMetricSpecificationTypeDef = TypedDict(
-    "_RequiredCustomizedMetricSpecificationTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": MetricStatisticType,
-    },
-)
-_OptionalCustomizedMetricSpecificationTypeDef = TypedDict(
-    "_OptionalCustomizedMetricSpecificationTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Unit": str,
-    },
-    total=False,
-)
-
-
-class CustomizedMetricSpecificationTypeDef(
-    _RequiredCustomizedMetricSpecificationTypeDef, _OptionalCustomizedMetricSpecificationTypeDef
-):
-    pass
-
-
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -1940,51 +2020,60 @@
     pass
 
 
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerTargetGroupsResponseTypeDef = TypedDict(
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     {
         "LoadBalancerTargetGroups": List[LoadBalancerTargetGroupStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersResponseTypeDef = TypedDict(
     "DescribeLoadBalancersResponseTypeDef",
     {
         "LoadBalancers": List[LoadBalancerStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricCollectionTypesAnswerTypeDef = TypedDict(
     "DescribeMetricCollectionTypesAnswerTypeDef",
     {
         "Metrics": List[MetricCollectionTypeTypeDef],
         "Granularities": List[MetricGranularityTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNotificationConfigurationsAnswerTypeDef = TypedDict(
     "DescribeNotificationConfigurationsAnswerTypeDef",
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTrafficSourcesResponseTypeDef = TypedDict(
+    "DescribeTrafficSourcesResponseTypeDef",
+    {
+        "TrafficSources": List[TrafficSourceStateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceRefreshProgressDetailsTypeDef = TypedDict(
     "InstanceRefreshProgressDetailsTypeDef",
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
@@ -2071,33 +2160,33 @@
     total=False,
 )
 
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
@@ -2171,57 +2260,68 @@
 
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
 
-_RequiredTargetTrackingConfigurationTypeDef = TypedDict(
-    "_RequiredTargetTrackingConfigurationTypeDef",
+_RequiredMetricStatTypeDef = TypedDict(
+    "_RequiredMetricStatTypeDef",
     {
-        "TargetValue": float,
+        "Metric": MetricTypeDef,
+        "Stat": str,
     },
 )
-_OptionalTargetTrackingConfigurationTypeDef = TypedDict(
-    "_OptionalTargetTrackingConfigurationTypeDef",
+_OptionalMetricStatTypeDef = TypedDict(
+    "_OptionalMetricStatTypeDef",
     {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
-        "CustomizedMetricSpecification": CustomizedMetricSpecificationTypeDef,
-        "DisableScaleIn": bool,
+        "Unit": str,
     },
     total=False,
 )
 
 
-class TargetTrackingConfigurationTypeDef(
-    _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
-):
+class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
 
-_RequiredMetricStatTypeDef = TypedDict(
-    "_RequiredMetricStatTypeDef",
+_RequiredTargetTrackingMetricStatTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
-_OptionalMetricStatTypeDef = TypedDict(
-    "_OptionalMetricStatTypeDef",
+_OptionalTargetTrackingMetricStatTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
 
-class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
+class TargetTrackingMetricStatTypeDef(
+    _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
+):
     pass
 
 
+RollbackDetailsTypeDef = TypedDict(
+    "RollbackDetailsTypeDef",
+    {
+        "RollbackReason": str,
+        "RollbackStartTime": datetime,
+        "PercentageCompleteOnRollback": int,
+        "InstancesToUpdateOnRollback": int,
+        "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
+    },
+    total=False,
+)
+
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2231,24 +2331,24 @@
 
 DescribeWarmPoolAnswerTypeDef = TypedDict(
     "DescribeWarmPoolAnswerTypeDef",
     {
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LaunchConfigurationsTypeTypeDef = TypedDict(
     "LaunchConfigurationsTypeTypeDef",
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
@@ -2266,14 +2366,38 @@
 )
 
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
 
+_RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricDataQueryTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricDataQueryTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": TargetTrackingMetricStatTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+
+class TargetTrackingMetricDataQueryTypeDef(
+    _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
+):
+    pass
+
+
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
@@ -2296,14 +2420,27 @@
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
         "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
+CustomizedMetricSpecificationTypeDef = TypedDict(
+    "CustomizedMetricSpecificationTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Statistic": MetricStatisticType,
+        "Unit": str,
+        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
+    },
+    total=False,
+)
+
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
@@ -2332,14 +2469,37 @@
 class PredictiveScalingMetricSpecificationTypeDef(
     _RequiredPredictiveScalingMetricSpecificationTypeDef,
     _OptionalPredictiveScalingMetricSpecificationTypeDef,
 ):
     pass
 
 
+_RequiredTargetTrackingConfigurationTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationTypeDef,
+        "DisableScaleIn": bool,
+    },
+    total=False,
+)
+
+
+class TargetTrackingConfigurationTypeDef(
+    _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
+):
+    pass
+
+
 _RequiredAutoScalingGroupTypeDef = TypedDict(
     "_RequiredAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
         "DesiredCapacity": int,
@@ -2373,14 +2533,15 @@
         "MaxInstanceLifetime": int,
         "CapacityRebalance": bool,
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "WarmPoolSize": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
+        "TrafficSources": List[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
@@ -2416,14 +2577,15 @@
         "LifecycleHookSpecificationList": Sequence[LifecycleHookSpecificationTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ServiceLinkedRoleARN": str,
         "MaxInstanceLifetime": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
+        "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
 
 class CreateAutoScalingGroupTypeRequestTypeDef(
     _RequiredCreateAutoScalingGroupTypeRequestTypeDef,
@@ -2516,15 +2678,15 @@
 
 
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceRefreshTypeDef = TypedDict(
     "InstanceRefreshTypeDef",
     {
         "InstanceRefreshId": str,
@@ -2534,14 +2696,15 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
         "Preferences": RefreshPreferencesTypeDef,
         "DesiredConfiguration": DesiredConfigurationTypeDef,
+        "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
@@ -2567,15 +2730,15 @@
 
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -2632,19 +2795,19 @@
 )
 
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PoliciesTypeTypeDef = TypedDict(
     "PoliciesTypeTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling/type_defs.pyi` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     MetricStatisticType,
     MetricTypeType,
     PredefinedLoadMetricTypeType,
     PredefinedMetricPairTypeType,
     PredefinedScalingMetricTypeType,
     PredictiveScalingMaxCapacityBreachBehaviorType,
     PredictiveScalingModeType,
+    ScaleInProtectedInstancesType,
     ScalingActivityStatusCodeType,
+    StandbyInstancesType,
     WarmPoolStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -49,65 +51,79 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
-    "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
+    "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsTypeDef",
+    "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
+    "DescribeAccountLimitsAnswerTypeDef",
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
     "DescribeInstanceRefreshesTypeRequestTypeDef",
+    "DescribeLifecycleHookTypesAnswerTypeDef",
     "LifecycleHookTypeDef",
     "DescribeLifecycleHooksTypeRequestTypeDef",
+    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     "LoadBalancerTargetGroupStateTypeDef",
+    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeLoadBalancersRequestRequestTypeDef",
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsTypeRequestTypeDef",
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    "DescribeTrafficSourcesRequestRequestTypeDef",
+    "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
@@ -117,94 +133,91 @@
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "RollbackInstanceRefreshAnswerTypeDef",
+    "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
+    "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
     "ActivityTypeTypeDef",
-    "CancelInstanceRefreshAnswerTypeDef",
-    "DescribeAccountLimitsAnswerTypeDef",
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DetachInstancesAnswerTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
-    "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
     "PolicyARNTypeTypeDef",
-    "AutoScalingGroupNamesTypeRequestTypeDef",
-    "DescribeTagsTypeRequestTypeDef",
+    "AttachTrafficSourcesTypeRequestTypeDef",
+    "DetachTrafficSourcesTypeRequestTypeDef",
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+    "DescribeTagsTypeRequestTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
-    "CustomizedMetricSpecificationTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
+    "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
-    "TargetTrackingConfigurationTypeDef",
     "MetricStatTypeDef",
+    "TargetTrackingMetricStatTypeDef",
+    "RollbackDetailsTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
     "MetricDataQueryTypeDef",
+    "TargetTrackingMetricDataQueryTypeDef",
     "LaunchTemplateTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
+    "CustomizedMetricSpecificationTypeDef",
     "MixedInstancesPolicyTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
+    "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
     "PredictiveScalingConfigurationTypeDef",
     "AutoScalingGroupsTypeTypeDef",
@@ -258,25 +271,14 @@
     },
     total=False,
 )
 
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
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
 AdjustmentTypeTypeDef = TypedDict(
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
@@ -321,29 +323,38 @@
     "AttachLoadBalancersTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "LoadBalancerNames": Sequence[str],
     },
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+_RequiredTrafficSourceIdentifierTypeDef = TypedDict(
+    "_RequiredTrafficSourceIdentifierTypeDef",
     {
-        "Name": str,
-        "Values": Sequence[str],
+        "Identifier": str,
+    },
+)
+_OptionalTrafficSourceIdentifierTypeDef = TypedDict(
+    "_OptionalTrafficSourceIdentifierTypeDef",
+    {
+        "Type": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+class TrafficSourceIdentifierTypeDef(
+    _RequiredTrafficSourceIdentifierTypeDef, _OptionalTrafficSourceIdentifierTypeDef
+):
+    pass
+
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 EnabledMetricTypeDef = TypedDict(
     "EnabledMetricTypeDef",
     {
@@ -458,14 +469,22 @@
         "Iops": int,
         "Encrypted": bool,
         "Throughput": int,
     },
     total=False,
 )
 
+CancelInstanceRefreshAnswerTypeDef = TypedDict(
+    "CancelInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CancelInstanceRefreshTypeRequestTypeDef = TypedDict(
     "CancelInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -648,24 +667,52 @@
 )
 
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
+DescribeAccountLimitsAnswerTypeDef = TypedDict(
+    "DescribeAccountLimitsAnswerTypeDef",
+    {
+        "MaxNumberOfAutoScalingGroups": int,
+        "MaxNumberOfLaunchConfigurations": int,
+        "NumberOfAutoScalingGroups": int,
+        "NumberOfLaunchConfigurations": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    {
+        "AutoScalingNotificationTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceRefreshesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
@@ -680,14 +727,22 @@
 
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
+DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    {
+        "LifecycleHookTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -716,14 +771,34 @@
 
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
+    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -746,14 +821,34 @@
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
 )
 
+_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
+    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
@@ -802,61 +897,145 @@
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationType": str,
     },
     total=False,
 )
 
+DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeNotificationConfigurationsTypeRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyNames": Sequence[str],
+        "PolicyTypes": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribePoliciesTypeRequestTypeDef = TypedDict(
     "DescribePoliciesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyNames": Sequence[str],
         "PolicyTypes": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ActivityIds": Sequence[str],
+        "AutoScalingGroupName": str,
+        "IncludeDeletedGroups": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeScalingActivitiesTypeRequestTypeDef = TypedDict(
     "DescribeScalingActivitiesTypeRequestTypeDef",
     {
         "ActivityIds": Sequence[str],
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
     "DescribeScheduledActionsTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    {
+        "TerminationPolicyTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeTrafficSourcesRequestRequestTypeDef",
+    {
+        "TrafficSourceType": str,
+        "NextToken": str,
+        "MaxRecords": int,
+    },
+    total=False,
+)
+
+class DescribeTrafficSourcesRequestRequestTypeDef(
+    _RequiredDescribeTrafficSourcesRequestRequestTypeDef,
+    _OptionalDescribeTrafficSourcesRequestRequestTypeDef,
+):
+    pass
+
+TrafficSourceStateTypeDef = TypedDict(
+    "TrafficSourceStateTypeDef",
+    {
+        "TrafficSource": str,
+        "State": str,
+        "Identifier": str,
+        "Type": str,
+    },
+    total=False,
+)
+
 _RequiredDescribeWarmPoolTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeWarmPoolTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeWarmPoolTypeRequestTypeDef = TypedDict(
@@ -925,14 +1104,21 @@
 
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1043,14 +1229,17 @@
     "RefreshPreferencesTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
     },
     total=False,
 )
 
 MemoryGiBPerVCpuRequestTypeDef = TypedDict(
     "MemoryGiBPerVCpuRequestTypeDef",
     {
@@ -1145,24 +1334,43 @@
 LaunchConfigurationNameTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNameTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 
+LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+    {
+        "LaunchConfigurationNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 LaunchConfigurationNamesTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeRequestTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
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
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1343,14 +1551,41 @@
 
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
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
+RollbackInstanceRefreshAnswerTypeDef = TypedDict(
+    "RollbackInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
+    "RollbackInstanceRefreshTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+    total=False,
+)
+
 _RequiredScalingProcessQueryRequestTypeDef = TypedDict(
     "_RequiredScalingProcessQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalScalingProcessQueryRequestTypeDef = TypedDict(
@@ -1429,275 +1664,140 @@
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
 )
 
+StartInstanceRefreshAnswerTypeDef = TypedDict(
+    "StartInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TerminateInstanceInAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     {
         "InstanceId": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
 
 ActivitiesTypeTypeDef = TypedDict(
     "ActivitiesTypeTypeDef",
     {
         "Activities": List[ActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActivityTypeTypeDef = TypedDict(
     "ActivityTypeTypeDef",
     {
         "Activity": ActivityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelInstanceRefreshAnswerTypeDef = TypedDict(
-    "CancelInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountLimitsAnswerTypeDef = TypedDict(
-    "DescribeAccountLimitsAnswerTypeDef",
-    {
-        "MaxNumberOfAutoScalingGroups": int,
-        "MaxNumberOfLaunchConfigurations": int,
-        "NumberOfAutoScalingGroups": int,
-        "NumberOfLaunchConfigurations": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    {
-        "AutoScalingNotificationTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    {
-        "LifecycleHookTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
-    {
-        "TerminationPolicyTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetachInstancesAnswerTypeDef = TypedDict(
     "DetachInstancesAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
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
 
 EnterStandbyAnswerTypeDef = TypedDict(
     "EnterStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExitStandbyAnswerTypeDef = TypedDict(
     "ExitStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartInstanceRefreshAnswerTypeDef = TypedDict(
-    "StartInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAdjustmentTypesAnswerTypeDef = TypedDict(
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeRequestTypeDef",
+AttachTrafficSourcesTypeRequestTypeDef = TypedDict(
+    "AttachTrafficSourcesTypeRequestTypeDef",
     {
-        "AutoScalingGroupNames": Sequence[str],
-        "NextToken": str,
-        "MaxRecords": int,
-        "Filters": Sequence[FilterTypeDef],
+        "AutoScalingGroupName": str,
+        "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
-    total=False,
 )
 
-DescribeTagsTypeRequestTypeDef = TypedDict(
-    "DescribeTagsTypeRequestTypeDef",
+DetachTrafficSourcesTypeRequestTypeDef = TypedDict(
+    "DetachTrafficSourcesTypeRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "NextToken": str,
-        "MaxRecords": int,
+        "AutoScalingGroupName": str,
+        "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
-    total=False,
 )
 
 AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
     "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
-    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
-    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-):
-    pass
-
-DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyNames": Sequence[str],
-        "PolicyTypes": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ActivityIds": Sequence[str],
-        "AutoScalingGroupName": str,
-        "IncludeDeletedGroups": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxRecords": int,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
+DescribeTagsTypeRequestTypeDef = TypedDict(
+    "DescribeTagsTypeRequestTypeDef",
     {
-        "LaunchConfigurationNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": Sequence[FilterTypeDef],
+        "NextToken": str,
+        "MaxRecords": int,
     },
     total=False,
 )
 
 _RequiredAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_RequiredAutoScalingInstanceDetailsTypeDef",
     {
@@ -1750,31 +1850,31 @@
     pass
 
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteScheduledActionAnswerTypeDef = TypedDict(
     "BatchDeleteScheduledActionAnswerTypeDef",
     {
         "FailedScheduledActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutScheduledUpdateGroupActionAnswerTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -1813,36 +1913,14 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredCustomizedMetricSpecificationTypeDef = TypedDict(
-    "_RequiredCustomizedMetricSpecificationTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": MetricStatisticType,
-    },
-)
-_OptionalCustomizedMetricSpecificationTypeDef = TypedDict(
-    "_OptionalCustomizedMetricSpecificationTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Unit": str,
-    },
-    total=False,
-)
-
-class CustomizedMetricSpecificationTypeDef(
-    _RequiredCustomizedMetricSpecificationTypeDef, _OptionalCustomizedMetricSpecificationTypeDef
-):
-    pass
-
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
@@ -1857,51 +1935,60 @@
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerTargetGroupsResponseTypeDef = TypedDict(
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     {
         "LoadBalancerTargetGroups": List[LoadBalancerTargetGroupStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersResponseTypeDef = TypedDict(
     "DescribeLoadBalancersResponseTypeDef",
     {
         "LoadBalancers": List[LoadBalancerStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricCollectionTypesAnswerTypeDef = TypedDict(
     "DescribeMetricCollectionTypesAnswerTypeDef",
     {
         "Metrics": List[MetricCollectionTypeTypeDef],
         "Granularities": List[MetricGranularityTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNotificationConfigurationsAnswerTypeDef = TypedDict(
     "DescribeNotificationConfigurationsAnswerTypeDef",
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTrafficSourcesResponseTypeDef = TypedDict(
+    "DescribeTrafficSourcesResponseTypeDef",
+    {
+        "TrafficSources": List[TrafficSourceStateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceRefreshProgressDetailsTypeDef = TypedDict(
     "InstanceRefreshProgressDetailsTypeDef",
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
@@ -1984,33 +2071,33 @@
     total=False,
 )
 
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
@@ -2080,53 +2167,64 @@
 )
 
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
-_RequiredTargetTrackingConfigurationTypeDef = TypedDict(
-    "_RequiredTargetTrackingConfigurationTypeDef",
+_RequiredMetricStatTypeDef = TypedDict(
+    "_RequiredMetricStatTypeDef",
     {
-        "TargetValue": float,
+        "Metric": MetricTypeDef,
+        "Stat": str,
     },
 )
-_OptionalTargetTrackingConfigurationTypeDef = TypedDict(
-    "_OptionalTargetTrackingConfigurationTypeDef",
+_OptionalMetricStatTypeDef = TypedDict(
+    "_OptionalMetricStatTypeDef",
     {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
-        "CustomizedMetricSpecification": CustomizedMetricSpecificationTypeDef,
-        "DisableScaleIn": bool,
+        "Unit": str,
     },
     total=False,
 )
 
-class TargetTrackingConfigurationTypeDef(
-    _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
-):
+class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
-_RequiredMetricStatTypeDef = TypedDict(
-    "_RequiredMetricStatTypeDef",
+_RequiredTargetTrackingMetricStatTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
-_OptionalMetricStatTypeDef = TypedDict(
-    "_OptionalMetricStatTypeDef",
+_OptionalTargetTrackingMetricStatTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
+class TargetTrackingMetricStatTypeDef(
+    _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
+):
     pass
 
+RollbackDetailsTypeDef = TypedDict(
+    "RollbackDetailsTypeDef",
+    {
+        "RollbackReason": str,
+        "RollbackStartTime": datetime,
+        "PercentageCompleteOnRollback": int,
+        "InstancesToUpdateOnRollback": int,
+        "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
+    },
+    total=False,
+)
+
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2136,24 +2234,24 @@
 
 DescribeWarmPoolAnswerTypeDef = TypedDict(
     "DescribeWarmPoolAnswerTypeDef",
     {
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LaunchConfigurationsTypeTypeDef = TypedDict(
     "LaunchConfigurationsTypeTypeDef",
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
@@ -2169,14 +2267,36 @@
     },
     total=False,
 )
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
+_RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricDataQueryTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricDataQueryTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": TargetTrackingMetricStatTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+class TargetTrackingMetricDataQueryTypeDef(
+    _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
+):
+    pass
+
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
@@ -2199,14 +2319,27 @@
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
         "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
+CustomizedMetricSpecificationTypeDef = TypedDict(
+    "CustomizedMetricSpecificationTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Statistic": MetricStatisticType,
+        "Unit": str,
+        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
+    },
+    total=False,
+)
+
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
@@ -2233,14 +2366,35 @@
 
 class PredictiveScalingMetricSpecificationTypeDef(
     _RequiredPredictiveScalingMetricSpecificationTypeDef,
     _OptionalPredictiveScalingMetricSpecificationTypeDef,
 ):
     pass
 
+_RequiredTargetTrackingConfigurationTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationTypeDef,
+        "DisableScaleIn": bool,
+    },
+    total=False,
+)
+
+class TargetTrackingConfigurationTypeDef(
+    _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
+):
+    pass
+
 _RequiredAutoScalingGroupTypeDef = TypedDict(
     "_RequiredAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
         "DesiredCapacity": int,
@@ -2274,14 +2428,15 @@
         "MaxInstanceLifetime": int,
         "CapacityRebalance": bool,
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "WarmPoolSize": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
+        "TrafficSources": List[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
@@ -2315,14 +2470,15 @@
         "LifecycleHookSpecificationList": Sequence[LifecycleHookSpecificationTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ServiceLinkedRoleARN": str,
         "MaxInstanceLifetime": int,
         "Context": str,
         "DesiredCapacityType": str,
         "DefaultInstanceWarmup": int,
+        "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
     total=False,
 )
 
 class CreateAutoScalingGroupTypeRequestTypeDef(
     _RequiredCreateAutoScalingGroupTypeRequestTypeDef,
     _OptionalCreateAutoScalingGroupTypeRequestTypeDef,
@@ -2409,15 +2565,15 @@
     pass
 
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceRefreshTypeDef = TypedDict(
     "InstanceRefreshTypeDef",
     {
         "InstanceRefreshId": str,
@@ -2427,14 +2583,15 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
         "Preferences": RefreshPreferencesTypeDef,
         "DesiredConfiguration": DesiredConfigurationTypeDef,
+        "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
@@ -2458,15 +2615,15 @@
 
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -2521,19 +2678,19 @@
 )
 
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PoliciesTypeTypeDef = TypedDict(
     "PoliciesTypeTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling
-Version: 1.26.7
-Summary: Type annotations for boto3.AutoScaling 1.26.7 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AutoScaling 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/
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
 
 <a id="mypy-boto3-autoscaling"></a>
 
 # mypy-boto3-autoscaling
 
 [![PyPI - mypy-boto3-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScaling 1.26.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
+[boto3.AutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [mypy-boto3-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,15 +363,17 @@
     MetricTypeType,
     PredefinedLoadMetricTypeType,
     PredefinedMetricPairTypeType,
     PredefinedScalingMetricTypeType,
     PredictiveScalingMaxCapacityBreachBehaviorType,
     PredictiveScalingModeType,
     RefreshStrategyType,
+    ScaleInProtectedInstancesType,
     ScalingActivityStatusCodeType,
+    StandbyInstancesType,
     WarmPoolStateType,
     WarmPoolStatusType,
     AutoScalingServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -389,65 +392,79 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
-    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
+    TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsTypeRequestTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
+    DescribeTrafficSourcesRequestRequestTypeDef,
+    TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
     GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
@@ -457,94 +474,91 @@
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
     PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
+    ResponseMetadataTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
-    AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeRequestTypeDef,
+    AttachTrafficSourcesTypeRequestTypeDef,
+    DetachTrafficSourcesTypeRequestTypeDef,
     AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    AutoScalingGroupNamesTypeRequestTypeDef,
     DescribeTagsTypeDescribeTagsPaginateTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
+    DescribeTagsTypeRequestTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
-    CustomizedMetricSpecificationTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
-    TargetTrackingConfigurationTypeDef,
     MetricStatTypeDef,
+    TargetTrackingMetricStatTypeDef,
+    RollbackDetailsTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
     MetricDataQueryTypeDef,
+    TargetTrackingMetricDataQueryTypeDef,
     LaunchTemplateTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
+    CustomizedMetricSpecificationTypeDef,
     MixedInstancesPolicyTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
+    TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
     PredictiveScalingConfigurationTypeDef,
     AutoScalingGroupsTypeTypeDef,
@@ -565,42 +579,42 @@
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

### Comparing `mypy-boto3-autoscaling-1.26.7/mypy_boto3_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-1.27.0/mypy_boto3_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-1.26.7/setup.py` & `mypy-boto3-autoscaling-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-autoscaling.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling",
-    version="1.26.7",
+    version="1.27.0",
     packages=["mypy_boto3_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScaling 1.26.7 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.AutoScaling 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 autoscaling type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_autoscaling": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_autoscaling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling/",
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


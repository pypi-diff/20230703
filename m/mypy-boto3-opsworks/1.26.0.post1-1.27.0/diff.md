# Comparing `tmp/mypy-boto3-opsworks-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-opsworks-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworks-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:48 2022, max compression
+gzip compressed data, was "mypy-boto3-opsworks-1.27.0.tar", last modified: Mon Jul  3 19:51:12 2023, max compression
```

## Comparing `mypy-boto3-opsworks-1.26.0.post1.tar` & `mypy-boto3-opsworks-1.27.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:48.208839 mypy-boto3-opsworks-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22977 2022-11-01 21:43:48.208839 mypy-boto3-opsworks-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21532 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:48.208839 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51763 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    51675 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11730 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    19546 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)    19510 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    64735 2022-11-01 21:38:50.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    64668 2022-11-01 21:38:50.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6633 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6627 2022-11-01 21:38:49.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:48.208839 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22977 2022-11-01 21:43:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-11-01 21:43:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:43:48.000000 mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:48.208839 mypy-boto3-opsworks-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-01 21:38:48.000000 mypy-boto3-opsworks-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.691762 mypy-boto3-opsworks-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-03 19:51:12.691762 mypy-boto3-opsworks-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.691762 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51761 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51673 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-07-03 19:43:07.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    64297 2023-07-03 19:43:08.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64230 2023-07-03 19:43:07.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.691762 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-07-03 19:51:12.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 19:51:12.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:12.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:12.000000 mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:12.691762 mypy-boto3-opsworks-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:43:06.000000 mypy-boto3-opsworks-1.27.0/setup.py
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/LICENSE` & `mypy-boto3-opsworks-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-opsworks-1.26.0.post1/PKG-INFO` & `mypy-boto3-opsworks-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.OpsWorks 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.OpsWorks 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
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
 
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworks?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -448,37 +449,44 @@
     SslConfigurationTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
-    ResponseMetadataTypeDef,
+    ChefConfigurationResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
+    CloneStackResultTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
+    CreateAppResultTypeDef,
     DeploymentCommandTypeDef,
+    CreateDeploymentResultTypeDef,
+    CreateInstanceResultTypeDef,
     RecipesTypeDef,
     VolumeConfigurationTypeDef,
+    CreateLayerResultTypeDef,
+    CreateStackResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
+    CreateUserProfileResultTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
     DeregisterEcsClusterRequestRequestTypeDef,
     DeregisterElasticIpRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DeregisterRdsDbInstanceRequestRequestTypeDef,
     DeregisterVolumeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAppsRequestRequestTypeDef,
     DescribeCommandsRequestRequestTypeDef,
     DescribeDeploymentsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersRequestRequestTypeDef,
     EcsClusterTypeDef,
     DescribeElasticIpsRequestRequestTypeDef,
     ElasticIpTypeDef,
     DescribeElasticLoadBalancersRequestRequestTypeDef,
     ElasticLoadBalancerTypeDef,
     DescribeInstancesRequestRequestTypeDef,
@@ -490,42 +498,53 @@
     DescribeRaidArraysRequestRequestTypeDef,
     RaidArrayTypeDef,
     DescribeRdsDbInstancesRequestRequestTypeDef,
     RdsDbInstanceTypeDef,
     DescribeServiceErrorsRequestRequestTypeDef,
     ServiceErrorTypeDef,
     DescribeStackProvisioningParametersRequestRequestTypeDef,
+    DescribeStackProvisioningParametersResultTypeDef,
     DescribeStackSummaryRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeTimeBasedAutoScalingRequestRequestTypeDef,
     DescribeUserProfilesRequestRequestTypeDef,
     UserProfileTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     VolumeTypeDef,
     DetachElasticLoadBalancerRequestRequestTypeDef,
     DisassociateElasticIpRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionRequestRequestTypeDef,
+    GetHostnameSuggestionResultTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
+    InstancesCountResponseMetadataTypeDef,
     InstancesCountTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResultTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
+    PaginatorConfigTypeDef,
     RebootInstanceRequestRequestTypeDef,
+    RecipesResponseMetadataTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
+    RegisterEcsClusterResultTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
+    RegisterElasticIpResultTypeDef,
+    RegisterInstanceResultTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
     RegisterVolumeRequestRequestTypeDef,
-    ServiceResourceLayerRequestTypeDef,
-    ServiceResourceStackRequestTypeDef,
-    ServiceResourceStackSummaryRequestTypeDef,
+    RegisterVolumeResultTypeDef,
+    ResponseMetadataTypeDef,
     SetPermissionRequestRequestTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
+    SourceResponseMetadataTypeDef,
+    StackConfigurationManagerResponseMetadataTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartStackRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopStackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UnassignInstanceRequestRequestTypeDef,
     UnassignVolumeRequestRequestTypeDef,
@@ -540,34 +559,14 @@
     DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
     BlockDeviceMappingTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
-    CloneStackResultTypeDef,
-    CreateAppResultTypeDef,
-    CreateDeploymentResultTypeDef,
-    CreateInstanceResultTypeDef,
-    CreateLayerResultTypeDef,
-    CreateStackResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DescribeStackProvisioningParametersResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetHostnameSuggestionResultTypeDef,
-    InstancesCountResponseMetadataTypeDef,
-    ListTagsResultTypeDef,
-    RecipesResponseMetadataTypeDef,
-    RegisterEcsClusterResultTypeDef,
-    RegisterElasticIpResultTypeDef,
-    RegisterInstanceResultTypeDef,
-    RegisterVolumeResultTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
     StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
@@ -576,15 +575,14 @@
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
-    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
     DescribeMyUserProfileResultTypeDef,
     DescribePermissionsResultTypeDef,
     DescribeRaidArraysResultTypeDef,
     DescribeRdsDbInstancesResultTypeDef,
@@ -625,42 +623,42 @@
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

### Comparing `mypy-boto3-opsworks-1.26.0.post1/README.md` & `mypy-boto3-opsworks-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworks?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,37 +417,44 @@
     SslConfigurationTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
-    ResponseMetadataTypeDef,
+    ChefConfigurationResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
+    CloneStackResultTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
+    CreateAppResultTypeDef,
     DeploymentCommandTypeDef,
+    CreateDeploymentResultTypeDef,
+    CreateInstanceResultTypeDef,
     RecipesTypeDef,
     VolumeConfigurationTypeDef,
+    CreateLayerResultTypeDef,
+    CreateStackResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
+    CreateUserProfileResultTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
     DeregisterEcsClusterRequestRequestTypeDef,
     DeregisterElasticIpRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DeregisterRdsDbInstanceRequestRequestTypeDef,
     DeregisterVolumeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAppsRequestRequestTypeDef,
     DescribeCommandsRequestRequestTypeDef,
     DescribeDeploymentsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersRequestRequestTypeDef,
     EcsClusterTypeDef,
     DescribeElasticIpsRequestRequestTypeDef,
     ElasticIpTypeDef,
     DescribeElasticLoadBalancersRequestRequestTypeDef,
     ElasticLoadBalancerTypeDef,
     DescribeInstancesRequestRequestTypeDef,
@@ -459,42 +466,53 @@
     DescribeRaidArraysRequestRequestTypeDef,
     RaidArrayTypeDef,
     DescribeRdsDbInstancesRequestRequestTypeDef,
     RdsDbInstanceTypeDef,
     DescribeServiceErrorsRequestRequestTypeDef,
     ServiceErrorTypeDef,
     DescribeStackProvisioningParametersRequestRequestTypeDef,
+    DescribeStackProvisioningParametersResultTypeDef,
     DescribeStackSummaryRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeTimeBasedAutoScalingRequestRequestTypeDef,
     DescribeUserProfilesRequestRequestTypeDef,
     UserProfileTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     VolumeTypeDef,
     DetachElasticLoadBalancerRequestRequestTypeDef,
     DisassociateElasticIpRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionRequestRequestTypeDef,
+    GetHostnameSuggestionResultTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
+    InstancesCountResponseMetadataTypeDef,
     InstancesCountTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResultTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
+    PaginatorConfigTypeDef,
     RebootInstanceRequestRequestTypeDef,
+    RecipesResponseMetadataTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
+    RegisterEcsClusterResultTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
+    RegisterElasticIpResultTypeDef,
+    RegisterInstanceResultTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
     RegisterVolumeRequestRequestTypeDef,
-    ServiceResourceLayerRequestTypeDef,
-    ServiceResourceStackRequestTypeDef,
-    ServiceResourceStackSummaryRequestTypeDef,
+    RegisterVolumeResultTypeDef,
+    ResponseMetadataTypeDef,
     SetPermissionRequestRequestTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
+    SourceResponseMetadataTypeDef,
+    StackConfigurationManagerResponseMetadataTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartStackRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopStackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UnassignInstanceRequestRequestTypeDef,
     UnassignVolumeRequestRequestTypeDef,
@@ -509,34 +527,14 @@
     DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
     BlockDeviceMappingTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
-    CloneStackResultTypeDef,
-    CreateAppResultTypeDef,
-    CreateDeploymentResultTypeDef,
-    CreateInstanceResultTypeDef,
-    CreateLayerResultTypeDef,
-    CreateStackResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DescribeStackProvisioningParametersResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetHostnameSuggestionResultTypeDef,
-    InstancesCountResponseMetadataTypeDef,
-    ListTagsResultTypeDef,
-    RecipesResponseMetadataTypeDef,
-    RegisterEcsClusterResultTypeDef,
-    RegisterElasticIpResultTypeDef,
-    RegisterInstanceResultTypeDef,
-    RegisterVolumeResultTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
     StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
@@ -545,15 +543,14 @@
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
-    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
     DescribeMyUserProfileResultTypeDef,
     DescribePermissionsResultTypeDef,
     DescribeRaidArraysResultTypeDef,
     DescribeRdsDbInstancesResultTypeDef,
@@ -594,42 +591,42 @@
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

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/__init__.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/__init__.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/__main__.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorks 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.OpsWorks 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/client.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 
     def describe_elastic_ips(
         self, *, InstanceId: str = ..., StackId: str = ..., Ips: Sequence[str] = ...
     ) -> DescribeElasticIpsResultTypeDef:
         """
         Describes [Elastic IP
         addresses](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-
-        addresses-eip.html)_ .
+        addresses-eip.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_elastic_ips)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_elastic_ips)
         """
 
     def describe_elastic_load_balancers(
         self, *, StackId: str = ..., LayerIds: Sequence[str] = ...
@@ -621,15 +621,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_stack_provisioning_parameters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_stack_provisioning_parameters)
         """
 
     def describe_stack_summary(self, *, StackId: str) -> DescribeStackSummaryResultTypeDef:
         """
         Describes the number of layers and apps in a specified stack, and the number of
-        instances in each state, such as `running_setup` or `online` .
+        instances in each state, such as `running_setup` or `online`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_stack_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_stack_summary)
         """
 
     def describe_stacks(self, *, StackIds: Sequence[str] = ...) -> DescribeStacksResultTypeDef:
         """
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/client.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -473,15 +473,15 @@
         """
     def describe_elastic_ips(
         self, *, InstanceId: str = ..., StackId: str = ..., Ips: Sequence[str] = ...
     ) -> DescribeElasticIpsResultTypeDef:
         """
         Describes [Elastic IP
         addresses](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-
-        addresses-eip.html)_ .
+        addresses-eip.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_elastic_ips)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_elastic_ips)
         """
     def describe_elastic_load_balancers(
         self, *, StackId: str = ..., LayerIds: Sequence[str] = ...
     ) -> DescribeElasticLoadBalancersResultTypeDef:
@@ -576,15 +576,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_stack_provisioning_parameters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_stack_provisioning_parameters)
         """
     def describe_stack_summary(self, *, StackId: str) -> DescribeStackSummaryResultTypeDef:
         """
         Describes the number of layers and apps in a specified stack, and the number of
-        instances in each state, such as `running_setup` or `online` .
+        instances in each state, such as `running_setup` or `online`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_stack_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_stack_summary)
         """
     def describe_stacks(self, *, StackIds: Sequence[str] = ...) -> DescribeStacksResultTypeDef:
         """
         Requests a description of one or more stacks.
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/literals.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AppAttributesKeysType",
     "AppExistsWaiterName",
     "AppTypeType",
     "ArchitectureType",
     "AutoScalingTypeType",
     "CloudWatchLogsEncodingType",
@@ -46,15 +45,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AppAttributesKeysType = Literal[
     "AutoBundleOnDeploy", "AwsFlowRubySettings", "DocumentRoot", "RailsEnv"
 ]
 AppExistsWaiterName = Literal["app_exists"]
 AppTypeType = Literal["aws-flow-ruby", "java", "nodejs", "other", "php", "rails", "static"]
 ArchitectureType = Literal["i386", "x86_64"]
 AutoScalingTypeType = Literal["load", "timer"]
@@ -232,23 +230,25 @@
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
@@ -258,30 +258,35 @@
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
@@ -307,14 +312,15 @@
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
@@ -359,51 +365,57 @@
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
@@ -416,14 +428,15 @@
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
@@ -435,28 +448,35 @@
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
@@ -465,14 +485,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -483,55 +504,64 @@
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
+    "scheduler",
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

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/literals.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AppAttributesKeysType",
     "AppExistsWaiterName",
     "AppTypeType",
     "ArchitectureType",
     "AutoScalingTypeType",
     "CloudWatchLogsEncodingType",
@@ -45,14 +46,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AppAttributesKeysType = Literal[
     "AutoBundleOnDeploy", "AwsFlowRubySettings", "DocumentRoot", "RailsEnv"
 ]
 AppExistsWaiterName = Literal["app_exists"]
 AppTypeType = Literal["aws-flow-ruby", "java", "nodejs", "other", "php", "rails", "static"]
 ArchitectureType = Literal["i386", "x86_64"]
 AutoScalingTypeType = Literal["load", "timer"]
@@ -230,23 +232,25 @@
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
@@ -256,30 +260,35 @@
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
@@ -305,14 +314,15 @@
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
@@ -357,51 +367,57 @@
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
@@ -414,14 +430,15 @@
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
@@ -433,28 +450,35 @@
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
@@ -463,14 +487,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -481,55 +506,64 @@
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
+    "scheduler",
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

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/paginator.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/paginator.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/service_resource.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/service_resource.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/type_defs.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -36,50 +36,56 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "StackConfigurationManagerTypeDef",
     "DataSourceTypeDef",
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
-    "ResponseMetadataTypeDef",
+    "ChefConfigurationResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
+    "CloneStackResultTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
+    "CreateAppResultTypeDef",
     "DeploymentCommandTypeDef",
+    "CreateDeploymentResultTypeDef",
+    "CreateInstanceResultTypeDef",
     "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
+    "CreateLayerResultTypeDef",
+    "CreateStackResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
+    "CreateUserProfileResultTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
     "DescribeCommandsRequestRequestTypeDef",
     "DescribeDeploymentsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     "DescribeEcsClustersRequestRequestTypeDef",
     "EcsClusterTypeDef",
     "DescribeElasticIpsRequestRequestTypeDef",
     "ElasticIpTypeDef",
     "DescribeElasticLoadBalancersRequestRequestTypeDef",
     "ElasticLoadBalancerTypeDef",
     "DescribeInstancesRequestRequestTypeDef",
@@ -91,42 +97,53 @@
     "DescribeRaidArraysRequestRequestTypeDef",
     "RaidArrayTypeDef",
     "DescribeRdsDbInstancesRequestRequestTypeDef",
     "RdsDbInstanceTypeDef",
     "DescribeServiceErrorsRequestRequestTypeDef",
     "ServiceErrorTypeDef",
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
+    "DescribeStackProvisioningParametersResultTypeDef",
     "DescribeStackSummaryRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeTimeBasedAutoScalingRequestRequestTypeDef",
     "DescribeUserProfilesRequestRequestTypeDef",
     "UserProfileTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "VolumeTypeDef",
     "DetachElasticLoadBalancerRequestRequestTypeDef",
     "DisassociateElasticIpRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
+    "GetHostnameSuggestionResultTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
+    "InstancesCountResponseMetadataTypeDef",
     "InstancesCountTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTagsResultTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
+    "PaginatorConfigTypeDef",
     "RebootInstanceRequestRequestTypeDef",
+    "RecipesResponseMetadataTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
+    "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
+    "RegisterElasticIpResultTypeDef",
+    "RegisterInstanceResultTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     "RegisterVolumeRequestRequestTypeDef",
-    "ServiceResourceLayerRequestTypeDef",
-    "ServiceResourceStackRequestTypeDef",
-    "ServiceResourceStackSummaryRequestTypeDef",
+    "RegisterVolumeResultTypeDef",
+    "ResponseMetadataTypeDef",
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
+    "SourceResponseMetadataTypeDef",
+    "StackConfigurationManagerResponseMetadataTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
@@ -141,34 +158,14 @@
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
-    "ChefConfigurationResponseMetadataTypeDef",
-    "CloneStackResultTypeDef",
-    "CreateAppResultTypeDef",
-    "CreateDeploymentResultTypeDef",
-    "CreateInstanceResultTypeDef",
-    "CreateLayerResultTypeDef",
-    "CreateStackResultTypeDef",
-    "CreateUserProfileResultTypeDef",
-    "DescribeStackProvisioningParametersResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetHostnameSuggestionResultTypeDef",
-    "InstancesCountResponseMetadataTypeDef",
-    "ListTagsResultTypeDef",
-    "RecipesResponseMetadataTypeDef",
-    "RegisterEcsClusterResultTypeDef",
-    "RegisterElasticIpResultTypeDef",
-    "RegisterInstanceResultTypeDef",
-    "RegisterVolumeResultTypeDef",
-    "SourceResponseMetadataTypeDef",
-    "StackConfigurationManagerResponseMetadataTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
@@ -177,15 +174,14 @@
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     "DescribeEcsClustersResultTypeDef",
     "DescribeElasticIpsResultTypeDef",
     "DescribeElasticLoadBalancersResultTypeDef",
     "DescribeMyUserProfileResultTypeDef",
     "DescribePermissionsResultTypeDef",
     "DescribeRaidArraysResultTypeDef",
     "DescribeRdsDbInstancesResultTypeDef",
@@ -248,21 +244,19 @@
     "_OptionalEnvironmentVariableTypeDef",
     {
         "Secure": bool,
     },
     total=False,
 )
 
-
 class EnvironmentVariableTypeDef(
     _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
@@ -283,19 +277,17 @@
     "_OptionalSslConfigurationTypeDef",
     {
         "Chain": str,
     },
     total=False,
 )
 
-
 class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
     pass
 
-
 AssignInstanceRequestRequestTypeDef = TypedDict(
     "AssignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LayerIds": Sequence[str],
     },
 )
@@ -310,43 +302,39 @@
     "_OptionalAssignVolumeRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-
 class AssignVolumeRequestRequestTypeDef(
     _RequiredAssignVolumeRequestRequestTypeDef, _OptionalAssignVolumeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAssociateElasticIpRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
     },
 )
 _OptionalAssociateElasticIpRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateElasticIpRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-
 class AssociateElasticIpRequestRequestTypeDef(
     _RequiredAssociateElasticIpRequestRequestTypeDef,
     _OptionalAssociateElasticIpRequestRequestTypeDef,
 ):
     pass
 
-
 AttachElasticLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
@@ -373,34 +361,40 @@
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "DeleteOnTermination": bool,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ChefConfigurationResponseMetadataTypeDef = TypedDict(
+    "ChefConfigurationResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ManageBerkshelf": bool,
+        "BerkshelfVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChefConfigurationTypeDef = TypedDict(
     "ChefConfigurationTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
     },
     total=False,
 )
 
+CloneStackResultTypeDef = TypedDict(
+    "CloneStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CloudWatchLogsLogStreamTypeDef = TypedDict(
     "CloudWatchLogsLogStreamTypeDef",
     {
         "LogGroupName": str,
         "DatetimeFormat": str,
         "TimeZone": CloudWatchLogsTimeZoneType,
         "File": str,
@@ -428,34 +422,56 @@
         "ExitCode": int,
         "LogUrl": str,
         "Type": str,
     },
     total=False,
 )
 
+CreateAppResultTypeDef = TypedDict(
+    "CreateAppResultTypeDef",
+    {
+        "AppId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeploymentCommandTypeDef = TypedDict(
     "_RequiredDeploymentCommandTypeDef",
     {
         "Name": DeploymentCommandNameType,
     },
 )
 _OptionalDeploymentCommandTypeDef = TypedDict(
     "_OptionalDeploymentCommandTypeDef",
     {
         "Args": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
+CreateDeploymentResultTypeDef = TypedDict(
+    "CreateDeploymentResultTypeDef",
+    {
+        "DeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateInstanceResultTypeDef = TypedDict(
+    "CreateInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 RecipesTypeDef = TypedDict(
     "RecipesTypeDef",
     {
         "Setup": Sequence[str],
         "Configure": Sequence[str],
         "Deploy": Sequence[str],
@@ -480,20 +496,34 @@
         "VolumeType": str,
         "Iops": int,
         "Encrypted": bool,
     },
     total=False,
 )
 
-
 class VolumeConfigurationTypeDef(
     _RequiredVolumeConfigurationTypeDef, _OptionalVolumeConfigurationTypeDef
 ):
     pass
 
+CreateLayerResultTypeDef = TypedDict(
+    "CreateLayerResultTypeDef",
+    {
+        "LayerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStackResultTypeDef = TypedDict(
+    "CreateStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
@@ -503,20 +533,26 @@
         "SshUsername": str,
         "SshPublicKey": str,
         "AllowSelfManagement": bool,
     },
     total=False,
 )
 
-
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "IamUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DeleteAppRequestRequestTypeDef = TypedDict(
     "DeleteAppRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
@@ -532,21 +568,19 @@
     {
         "DeleteElasticIp": bool,
         "DeleteVolumes": bool,
     },
     total=False,
 )
 
-
 class DeleteInstanceRequestRequestTypeDef(
     _RequiredDeleteInstanceRequestRequestTypeDef, _OptionalDeleteInstanceRequestRequestTypeDef
 ):
     pass
 
-
 DeleteLayerRequestRequestTypeDef = TypedDict(
     "DeleteLayerRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 
@@ -633,20 +667,20 @@
         "StackId": str,
         "AppId": str,
         "DeploymentIds": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "EcsClusterArns": Sequence[str],
+        "StackId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEcsClustersRequestRequestTypeDef = TypedDict(
     "DescribeEcsClustersRequestRequestTypeDef",
     {
@@ -814,22 +848,20 @@
     "_OptionalDescribeRdsDbInstancesRequestRequestTypeDef",
     {
         "RdsDbInstanceArns": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeRdsDbInstancesRequestRequestTypeDef(
     _RequiredDescribeRdsDbInstancesRequestRequestTypeDef,
     _OptionalDescribeRdsDbInstancesRequestRequestTypeDef,
 ):
     pass
 
-
 RdsDbInstanceTypeDef = TypedDict(
     "RdsDbInstanceTypeDef",
     {
         "RdsDbInstanceArn": str,
         "DbInstanceIdentifier": str,
         "DbUser": str,
         "DbPassword": str,
@@ -868,14 +900,23 @@
 DescribeStackProvisioningParametersRequestRequestTypeDef = TypedDict(
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
+DescribeStackProvisioningParametersResultTypeDef = TypedDict(
+    "DescribeStackProvisioningParametersResultTypeDef",
+    {
+        "AgentInstallerUrl": str,
+        "Parameters": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeStackSummaryRequestRequestTypeDef = TypedDict(
     "DescribeStackSummaryRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
@@ -957,42 +998,56 @@
 DisassociateElasticIpRequestRequestTypeDef = TypedDict(
     "DisassociateElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHostnameSuggestionRequestRequestTypeDef = TypedDict(
     "GetHostnameSuggestionRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 
+GetHostnameSuggestionResultTypeDef = TypedDict(
+    "GetHostnameSuggestionResultTypeDef",
+    {
+        "LayerId": str,
+        "Hostname": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGrantAccessRequestRequestTypeDef = TypedDict(
     "_RequiredGrantAccessRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalGrantAccessRequestRequestTypeDef = TypedDict(
     "_OptionalGrantAccessRequestRequestTypeDef",
     {
         "ValidForInMinutes": int,
     },
     total=False,
 )
 
-
 class GrantAccessRequestRequestTypeDef(
     _RequiredGrantAccessRequestRequestTypeDef, _OptionalGrantAccessRequestRequestTypeDef
 ):
     pass
 
-
 TemporaryCredentialTypeDef = TypedDict(
     "TemporaryCredentialTypeDef",
     {
         "Username": str,
         "Password": str,
         "ValidForInMinutes": int,
         "InstanceId": str,
@@ -1015,14 +1070,41 @@
         "Family": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
+InstancesCountResponseMetadataTypeDef = TypedDict(
+    "InstancesCountResponseMetadataTypeDef",
+    {
+        "Assigning": int,
+        "Booting": int,
+        "ConnectionLost": int,
+        "Deregistering": int,
+        "Online": int,
+        "Pending": int,
+        "Rebooting": int,
+        "Registered": int,
+        "Registering": int,
+        "Requested": int,
+        "RunningSetup": int,
+        "SetupFailed": int,
+        "ShuttingDown": int,
+        "StartFailed": int,
+        "StopFailed": int,
+        "Stopped": int,
+        "Stopping": int,
+        "Terminated": int,
+        "Terminating": int,
+        "Unassigning": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InstancesCountTypeDef = TypedDict(
     "InstancesCountTypeDef",
     {
         "Assigning": int,
         "Booting": int,
         "ConnectionLost": int,
         "Deregistering": int,
@@ -1066,53 +1148,106 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+ListTagsResultTypeDef = TypedDict(
+    "ListTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 OperatingSystemConfigurationManagerTypeDef = TypedDict(
     "OperatingSystemConfigurationManagerTypeDef",
     {
         "Name": str,
         "Version": str,
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
 RebootInstanceRequestRequestTypeDef = TypedDict(
     "RebootInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
+RecipesResponseMetadataTypeDef = TypedDict(
+    "RecipesResponseMetadataTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterEcsClusterRequestRequestTypeDef = TypedDict(
     "RegisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
         "StackId": str,
     },
 )
 
+RegisterEcsClusterResultTypeDef = TypedDict(
+    "RegisterEcsClusterResultTypeDef",
+    {
+        "EcsClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterElasticIpRequestRequestTypeDef = TypedDict(
     "RegisterElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
         "StackId": str,
     },
 )
 
+RegisterElasticIpResultTypeDef = TypedDict(
+    "RegisterElasticIpResultTypeDef",
+    {
+        "ElasticIp": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterInstanceResultTypeDef = TypedDict(
+    "RegisterInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterRdsDbInstanceRequestRequestTypeDef = TypedDict(
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     {
         "StackId": str,
         "RdsDbInstanceArn": str,
         "DbUser": str,
         "DbPassword": str,
@@ -1129,39 +1264,35 @@
     "_OptionalRegisterVolumeRequestRequestTypeDef",
     {
         "Ec2VolumeId": str,
     },
     total=False,
 )
 
-
 class RegisterVolumeRequestRequestTypeDef(
     _RequiredRegisterVolumeRequestRequestTypeDef, _OptionalRegisterVolumeRequestRequestTypeDef
 ):
     pass
 
-
-ServiceResourceLayerRequestTypeDef = TypedDict(
-    "ServiceResourceLayerRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-ServiceResourceStackRequestTypeDef = TypedDict(
-    "ServiceResourceStackRequestTypeDef",
+RegisterVolumeResultTypeDef = TypedDict(
+    "RegisterVolumeResultTypeDef",
     {
-        "id": str,
+        "VolumeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServiceResourceStackSummaryRequestTypeDef = TypedDict(
-    "ServiceResourceStackSummaryRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "stack_id": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredSetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredSetPermissionRequestRequestTypeDef",
     {
         "StackId": str,
@@ -1174,35 +1305,55 @@
         "AllowSsh": bool,
         "AllowSudo": bool,
         "Level": str,
     },
     total=False,
 )
 
-
 class SetPermissionRequestRequestTypeDef(
     _RequiredSetPermissionRequestRequestTypeDef, _OptionalSetPermissionRequestRequestTypeDef
 ):
     pass
 
-
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
         "Monday": Dict[str, str],
         "Tuesday": Dict[str, str],
         "Wednesday": Dict[str, str],
         "Thursday": Dict[str, str],
         "Friday": Dict[str, str],
         "Saturday": Dict[str, str],
         "Sunday": Dict[str, str],
     },
     total=False,
 )
 
+SourceResponseMetadataTypeDef = TypedDict(
+    "SourceResponseMetadataTypeDef",
+    {
+        "Type": SourceTypeType,
+        "Url": str,
+        "Username": str,
+        "Password": str,
+        "SshKey": str,
+        "Revision": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
+    "StackConfigurationManagerResponseMetadataTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1223,21 +1374,19 @@
     "_OptionalStopInstanceRequestRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
-
 class StopInstanceRequestRequestTypeDef(
     _RequiredStopInstanceRequestRequestTypeDef, _OptionalStopInstanceRequestRequestTypeDef
 ):
     pass
 
-
 StopStackRequestRequestTypeDef = TypedDict(
     "StopStackRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
@@ -1281,21 +1430,19 @@
     "_OptionalUpdateElasticIpRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateElasticIpRequestRequestTypeDef(
     _RequiredUpdateElasticIpRequestRequestTypeDef, _OptionalUpdateElasticIpRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalUpdateInstanceRequestRequestTypeDef = TypedDict(
@@ -1312,21 +1459,19 @@
         "InstallUpdatesOnBoot": bool,
         "EbsOptimized": bool,
         "AgentVersion": str,
     },
     total=False,
 )
 
-
 class UpdateInstanceRequestRequestTypeDef(
     _RequiredUpdateInstanceRequestRequestTypeDef, _OptionalUpdateInstanceRequestRequestTypeDef
 ):
     pass
 
-
 UpdateMyUserProfileRequestRequestTypeDef = TypedDict(
     "UpdateMyUserProfileRequestRequestTypeDef",
     {
         "SshPublicKey": str,
     },
     total=False,
 )
@@ -1342,22 +1487,20 @@
     {
         "DbUser": str,
         "DbPassword": str,
     },
     total=False,
 )
 
-
 class UpdateRdsDbInstanceRequestRequestTypeDef(
     _RequiredUpdateRdsDbInstanceRequestRequestTypeDef,
     _OptionalUpdateRdsDbInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -1366,21 +1509,19 @@
         "SshUsername": str,
         "SshPublicKey": str,
         "AllowSelfManagement": bool,
     },
     total=False,
 )
 
-
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
@@ -1388,21 +1529,19 @@
     {
         "Name": str,
         "MountPoint": str,
     },
     total=False,
 )
 
-
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
-
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "Version": str,
         "ConfigurationManager": StackConfigurationManagerTypeDef,
     },
     total=False,
@@ -1458,21 +1597,19 @@
         "SslConfiguration": SslConfigurationTypeDef,
         "Attributes": Mapping[AppAttributesKeysType, str],
         "Environment": Sequence[EnvironmentVariableTypeDef],
     },
     total=False,
 )
 
-
 class CreateAppRequestRequestTypeDef(
     _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateAppRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalUpdateAppRequestRequestTypeDef = TypedDict(
@@ -1488,21 +1625,19 @@
         "SslConfiguration": SslConfigurationTypeDef,
         "Attributes": Mapping[AppAttributesKeysType, str],
         "Environment": Sequence[EnvironmentVariableTypeDef],
     },
     total=False,
 )
 
-
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
-
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsTypeDef,
         "DownScaling": AutoScalingThresholdsTypeDef,
@@ -1522,225 +1657,31 @@
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsTypeDef,
         "DownScaling": AutoScalingThresholdsTypeDef,
     },
     total=False,
 )
 
-
 class SetLoadBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
-
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "NoDevice": str,
         "VirtualName": str,
         "Ebs": EbsBlockDeviceTypeDef,
     },
     total=False,
 )
 
-ChefConfigurationResponseMetadataTypeDef = TypedDict(
-    "ChefConfigurationResponseMetadataTypeDef",
-    {
-        "ManageBerkshelf": bool,
-        "BerkshelfVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CloneStackResultTypeDef = TypedDict(
-    "CloneStackResultTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppResultTypeDef = TypedDict(
-    "CreateAppResultTypeDef",
-    {
-        "AppId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResultTypeDef = TypedDict(
-    "CreateDeploymentResultTypeDef",
-    {
-        "DeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateInstanceResultTypeDef = TypedDict(
-    "CreateInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLayerResultTypeDef = TypedDict(
-    "CreateLayerResultTypeDef",
-    {
-        "LayerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackResultTypeDef = TypedDict(
-    "CreateStackResultTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "IamUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStackProvisioningParametersResultTypeDef = TypedDict(
-    "DescribeStackProvisioningParametersResultTypeDef",
-    {
-        "AgentInstallerUrl": str,
-        "Parameters": Dict[str, str],
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
-GetHostnameSuggestionResultTypeDef = TypedDict(
-    "GetHostnameSuggestionResultTypeDef",
-    {
-        "LayerId": str,
-        "Hostname": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InstancesCountResponseMetadataTypeDef = TypedDict(
-    "InstancesCountResponseMetadataTypeDef",
-    {
-        "Assigning": int,
-        "Booting": int,
-        "ConnectionLost": int,
-        "Deregistering": int,
-        "Online": int,
-        "Pending": int,
-        "Rebooting": int,
-        "Registered": int,
-        "Registering": int,
-        "Requested": int,
-        "RunningSetup": int,
-        "SetupFailed": int,
-        "ShuttingDown": int,
-        "StartFailed": int,
-        "StopFailed": int,
-        "Stopped": int,
-        "Stopping": int,
-        "Terminated": int,
-        "Terminating": int,
-        "Unassigning": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResultTypeDef = TypedDict(
-    "ListTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecipesResponseMetadataTypeDef = TypedDict(
-    "RecipesResponseMetadataTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterEcsClusterResultTypeDef = TypedDict(
-    "RegisterEcsClusterResultTypeDef",
-    {
-        "EcsClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterElasticIpResultTypeDef = TypedDict(
-    "RegisterElasticIpResultTypeDef",
-    {
-        "ElasticIp": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterInstanceResultTypeDef = TypedDict(
-    "RegisterInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterVolumeResultTypeDef = TypedDict(
-    "RegisterVolumeResultTypeDef",
-    {
-        "VolumeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SourceResponseMetadataTypeDef = TypedDict(
-    "SourceResponseMetadataTypeDef",
-    {
-        "Type": SourceTypeType,
-        "Url": str,
-        "Username": str,
-        "Password": str,
-        "SshKey": str,
-        "Revision": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
-    "StackConfigurationManagerResponseMetadataTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCloneStackRequestRequestTypeDef = TypedDict(
     "_RequiredCloneStackRequestRequestTypeDef",
     {
         "SourceStackId": str,
         "ServiceRoleArn": str,
     },
 )
@@ -1767,21 +1708,19 @@
         "CloneAppIds": Sequence[str],
         "DefaultRootDeviceType": RootDeviceTypeType,
         "AgentVersion": str,
     },
     total=False,
 )
 
-
 class CloneStackRequestRequestTypeDef(
     _RequiredCloneStackRequestRequestTypeDef, _OptionalCloneStackRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStackRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStackRequestRequestTypeDef",
     {
         "Name": str,
         "Region": str,
         "ServiceRoleArn": str,
         "DefaultInstanceProfileArn": str,
@@ -1805,21 +1744,19 @@
         "DefaultSshKeyName": str,
         "DefaultRootDeviceType": RootDeviceTypeType,
         "AgentVersion": str,
     },
     total=False,
 )
 
-
 class CreateStackRequestRequestTypeDef(
     _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStackRequestServiceResourceCreateStackTypeDef = TypedDict(
     "_RequiredCreateStackRequestServiceResourceCreateStackTypeDef",
     {
         "Name": str,
         "Region": str,
         "ServiceRoleArn": str,
         "DefaultInstanceProfileArn": str,
@@ -1843,22 +1780,20 @@
         "DefaultSshKeyName": str,
         "DefaultRootDeviceType": RootDeviceTypeType,
         "AgentVersion": str,
     },
     total=False,
 )
 
-
 class CreateStackRequestServiceResourceCreateStackTypeDef(
     _RequiredCreateStackRequestServiceResourceCreateStackTypeDef,
     _OptionalCreateStackRequestServiceResourceCreateStackTypeDef,
 ):
     pass
 
-
 StackTypeDef = TypedDict(
     "StackTypeDef",
     {
         "StackId": str,
         "Name": str,
         "Arn": str,
         "Region": str,
@@ -1910,27 +1845,25 @@
         "DefaultRootDeviceType": RootDeviceTypeType,
         "UseOpsworksSecurityGroups": bool,
         "AgentVersion": str,
     },
     total=False,
 )
 
-
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
-
 CloudWatchLogsConfigurationResponseMetadataTypeDef = TypedDict(
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     {
         "Enabled": bool,
         "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
@@ -1939,15 +1872,15 @@
     total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "StackId": str,
@@ -1962,21 +1895,19 @@
         "LayerIds": Sequence[str],
         "Comment": str,
         "CustomJson": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": str,
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
@@ -2053,110 +1984,100 @@
         "LayerId": str,
         "InstanceIds": Sequence[str],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
-    {
-        "EcsClusterArns": Sequence[str],
-        "StackId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeEcsClustersResultTypeDef = TypedDict(
     "DescribeEcsClustersResultTypeDef",
     {
         "EcsClusters": List[EcsClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticIpsResultTypeDef = TypedDict(
     "DescribeElasticIpsResultTypeDef",
     {
         "ElasticIps": List[ElasticIpTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticLoadBalancersResultTypeDef = TypedDict(
     "DescribeElasticLoadBalancersResultTypeDef",
     {
         "ElasticLoadBalancers": List[ElasticLoadBalancerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMyUserProfileResultTypeDef = TypedDict(
     "DescribeMyUserProfileResultTypeDef",
     {
         "UserProfile": SelfUserProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePermissionsResultTypeDef = TypedDict(
     "DescribePermissionsResultTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRaidArraysResultTypeDef = TypedDict(
     "DescribeRaidArraysResultTypeDef",
     {
         "RaidArrays": List[RaidArrayTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRdsDbInstancesResultTypeDef = TypedDict(
     "DescribeRdsDbInstancesResultTypeDef",
     {
         "RdsDbInstances": List[RdsDbInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServiceErrorsResultTypeDef = TypedDict(
     "DescribeServiceErrorsResultTypeDef",
     {
         "ServiceErrors": List[ServiceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserProfilesResultTypeDef = TypedDict(
     "DescribeUserProfilesResultTypeDef",
     {
         "UserProfiles": List[UserProfileTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVolumesResultTypeDef = TypedDict(
     "DescribeVolumesResultTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GrantAccessResultTypeDef = TypedDict(
     "GrantAccessResultTypeDef",
     {
         "TemporaryCredential": TemporaryCredentialTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2171,21 +2092,19 @@
         "RsaPublicKey": str,
         "RsaPublicKeyFingerprint": str,
         "InstanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
-
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
-
 StackSummaryTypeDef = TypedDict(
     "StackSummaryTypeDef",
     {
         "StackId": str,
         "Name": str,
         "Arn": str,
         "LayersCount": int,
@@ -2195,15 +2114,15 @@
     total=False,
 )
 
 LifecycleEventConfigurationResponseMetadataTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseMetadataTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleEventConfigurationTypeDef = TypedDict(
     "LifecycleEventConfigurationTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
@@ -2235,52 +2154,50 @@
     "_OptionalSetTimeBasedAutoScalingRequestRequestTypeDef",
     {
         "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
     },
     total=False,
 )
 
-
 class SetTimeBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetTimeBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetTimeBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
-
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": str,
         "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
     },
     total=False,
 )
 
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppsResultTypeDef = TypedDict(
     "DescribeAppsResultTypeDef",
     {
         "Apps": List[AppTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeLoadBasedAutoScalingResultTypeDef",
     {
         "LoadBasedAutoScalingConfigurations": List[LoadBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2306,21 +2223,19 @@
         "EbsOptimized": bool,
         "AgentVersion": str,
         "Tenancy": str,
     },
     total=False,
 )
 
-
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
-
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AgentVersion": str,
         "AmiId": str,
         "Architecture": ArchitectureType,
         "Arn": str,
@@ -2365,31 +2280,31 @@
     total=False,
 )
 
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackSummaryResultTypeDef = TypedDict(
     "DescribeStackSummaryResultTypeDef",
     {
         "StackSummary": StackSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLayerRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2415,21 +2330,19 @@
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateLayerRequestRequestTypeDef(
     _RequiredCreateLayerRequestRequestTypeDef, _OptionalCreateLayerRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLayerRequestStackCreateLayerTypeDef = TypedDict(
     "_RequiredCreateLayerRequestStackCreateLayerTypeDef",
     {
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
     },
@@ -2451,22 +2364,20 @@
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateLayerRequestStackCreateLayerTypeDef(
     _RequiredCreateLayerRequestStackCreateLayerTypeDef,
     _OptionalCreateLayerRequestStackCreateLayerTypeDef,
 ):
     pass
 
-
 LayerTypeDef = TypedDict(
     "LayerTypeDef",
     {
         "Arn": str,
         "StackId": str,
         "LayerId": str,
         "Type": LayerTypeType,
@@ -2518,45 +2429,43 @@
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateLayerRequestRequestTypeDef(
     _RequiredUpdateLayerRequestRequestTypeDef, _OptionalUpdateLayerRequestRequestTypeDef
 ):
     pass
 
-
 DescribeOperatingSystemsResponseTypeDef = TypedDict(
     "DescribeOperatingSystemsResponseTypeDef",
     {
         "OperatingSystems": List[OperatingSystemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTimeBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeTimeBasedAutoScalingResultTypeDef",
     {
         "TimeBasedAutoScalingConfigurations": List[TimeBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstancesResultTypeDef = TypedDict(
     "DescribeInstancesResultTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLayersResultTypeDef = TypedDict(
     "DescribeLayersResultTypeDef",
     {
         "Layers": List[LayerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/type_defs.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,49 +36,57 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "StackConfigurationManagerTypeDef",
     "DataSourceTypeDef",
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
-    "ResponseMetadataTypeDef",
+    "ChefConfigurationResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
+    "CloneStackResultTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
+    "CreateAppResultTypeDef",
     "DeploymentCommandTypeDef",
+    "CreateDeploymentResultTypeDef",
+    "CreateInstanceResultTypeDef",
     "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
+    "CreateLayerResultTypeDef",
+    "CreateStackResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
+    "CreateUserProfileResultTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
     "DescribeCommandsRequestRequestTypeDef",
     "DescribeDeploymentsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     "DescribeEcsClustersRequestRequestTypeDef",
     "EcsClusterTypeDef",
     "DescribeElasticIpsRequestRequestTypeDef",
     "ElasticIpTypeDef",
     "DescribeElasticLoadBalancersRequestRequestTypeDef",
     "ElasticLoadBalancerTypeDef",
     "DescribeInstancesRequestRequestTypeDef",
@@ -90,42 +98,53 @@
     "DescribeRaidArraysRequestRequestTypeDef",
     "RaidArrayTypeDef",
     "DescribeRdsDbInstancesRequestRequestTypeDef",
     "RdsDbInstanceTypeDef",
     "DescribeServiceErrorsRequestRequestTypeDef",
     "ServiceErrorTypeDef",
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
+    "DescribeStackProvisioningParametersResultTypeDef",
     "DescribeStackSummaryRequestRequestTypeDef",
     "DescribeStacksRequestRequestTypeDef",
     "DescribeTimeBasedAutoScalingRequestRequestTypeDef",
     "DescribeUserProfilesRequestRequestTypeDef",
     "UserProfileTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "VolumeTypeDef",
     "DetachElasticLoadBalancerRequestRequestTypeDef",
     "DisassociateElasticIpRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
+    "GetHostnameSuggestionResultTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
+    "InstancesCountResponseMetadataTypeDef",
     "InstancesCountTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTagsResultTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
+    "PaginatorConfigTypeDef",
     "RebootInstanceRequestRequestTypeDef",
+    "RecipesResponseMetadataTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
+    "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
+    "RegisterElasticIpResultTypeDef",
+    "RegisterInstanceResultTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     "RegisterVolumeRequestRequestTypeDef",
-    "ServiceResourceLayerRequestTypeDef",
-    "ServiceResourceStackRequestTypeDef",
-    "ServiceResourceStackSummaryRequestTypeDef",
+    "RegisterVolumeResultTypeDef",
+    "ResponseMetadataTypeDef",
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
+    "SourceResponseMetadataTypeDef",
+    "StackConfigurationManagerResponseMetadataTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
@@ -140,34 +159,14 @@
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
-    "ChefConfigurationResponseMetadataTypeDef",
-    "CloneStackResultTypeDef",
-    "CreateAppResultTypeDef",
-    "CreateDeploymentResultTypeDef",
-    "CreateInstanceResultTypeDef",
-    "CreateLayerResultTypeDef",
-    "CreateStackResultTypeDef",
-    "CreateUserProfileResultTypeDef",
-    "DescribeStackProvisioningParametersResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetHostnameSuggestionResultTypeDef",
-    "InstancesCountResponseMetadataTypeDef",
-    "ListTagsResultTypeDef",
-    "RecipesResponseMetadataTypeDef",
-    "RegisterEcsClusterResultTypeDef",
-    "RegisterElasticIpResultTypeDef",
-    "RegisterInstanceResultTypeDef",
-    "RegisterVolumeResultTypeDef",
-    "SourceResponseMetadataTypeDef",
-    "StackConfigurationManagerResponseMetadataTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
@@ -176,15 +175,14 @@
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     "DescribeEcsClustersResultTypeDef",
     "DescribeElasticIpsResultTypeDef",
     "DescribeElasticLoadBalancersResultTypeDef",
     "DescribeMyUserProfileResultTypeDef",
     "DescribePermissionsResultTypeDef",
     "DescribeRaidArraysResultTypeDef",
     "DescribeRdsDbInstancesResultTypeDef",
@@ -247,19 +245,21 @@
     "_OptionalEnvironmentVariableTypeDef",
     {
         "Secure": bool,
     },
     total=False,
 )
 
+
 class EnvironmentVariableTypeDef(
     _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "Type": SourceTypeType,
         "Url": str,
         "Username": str,
         "Password": str,
@@ -280,17 +280,19 @@
     "_OptionalSslConfigurationTypeDef",
     {
         "Chain": str,
     },
     total=False,
 )
 
+
 class SslConfigurationTypeDef(_RequiredSslConfigurationTypeDef, _OptionalSslConfigurationTypeDef):
     pass
 
+
 AssignInstanceRequestRequestTypeDef = TypedDict(
     "AssignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "LayerIds": Sequence[str],
     },
 )
@@ -305,39 +307,43 @@
     "_OptionalAssignVolumeRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
+
 class AssignVolumeRequestRequestTypeDef(
     _RequiredAssignVolumeRequestRequestTypeDef, _OptionalAssignVolumeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAssociateElasticIpRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
     },
 )
 _OptionalAssociateElasticIpRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateElasticIpRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
+
 class AssociateElasticIpRequestRequestTypeDef(
     _RequiredAssociateElasticIpRequestRequestTypeDef,
     _OptionalAssociateElasticIpRequestRequestTypeDef,
 ):
     pass
 
+
 AttachElasticLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
@@ -364,34 +370,40 @@
         "VolumeSize": int,
         "VolumeType": VolumeTypeType,
         "DeleteOnTermination": bool,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ChefConfigurationResponseMetadataTypeDef = TypedDict(
+    "ChefConfigurationResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ManageBerkshelf": bool,
+        "BerkshelfVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChefConfigurationTypeDef = TypedDict(
     "ChefConfigurationTypeDef",
     {
         "ManageBerkshelf": bool,
         "BerkshelfVersion": str,
     },
     total=False,
 )
 
+CloneStackResultTypeDef = TypedDict(
+    "CloneStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CloudWatchLogsLogStreamTypeDef = TypedDict(
     "CloudWatchLogsLogStreamTypeDef",
     {
         "LogGroupName": str,
         "DatetimeFormat": str,
         "TimeZone": CloudWatchLogsTimeZoneType,
         "File": str,
@@ -419,33 +431,59 @@
         "ExitCode": int,
         "LogUrl": str,
         "Type": str,
     },
     total=False,
 )
 
+CreateAppResultTypeDef = TypedDict(
+    "CreateAppResultTypeDef",
+    {
+        "AppId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeploymentCommandTypeDef = TypedDict(
     "_RequiredDeploymentCommandTypeDef",
     {
         "Name": DeploymentCommandNameType,
     },
 )
 _OptionalDeploymentCommandTypeDef = TypedDict(
     "_OptionalDeploymentCommandTypeDef",
     {
         "Args": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
+
+CreateDeploymentResultTypeDef = TypedDict(
+    "CreateDeploymentResultTypeDef",
+    {
+        "DeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateInstanceResultTypeDef = TypedDict(
+    "CreateInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecipesTypeDef = TypedDict(
     "RecipesTypeDef",
     {
         "Setup": Sequence[str],
         "Configure": Sequence[str],
         "Deploy": Sequence[str],
         "Undeploy": Sequence[str],
@@ -469,19 +507,37 @@
         "VolumeType": str,
         "Iops": int,
         "Encrypted": bool,
     },
     total=False,
 )
 
+
 class VolumeConfigurationTypeDef(
     _RequiredVolumeConfigurationTypeDef, _OptionalVolumeConfigurationTypeDef
 ):
     pass
 
+
+CreateLayerResultTypeDef = TypedDict(
+    "CreateLayerResultTypeDef",
+    {
+        "LayerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStackResultTypeDef = TypedDict(
+    "CreateStackResultTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 _OptionalCreateUserProfileRequestRequestTypeDef = TypedDict(
@@ -490,19 +546,29 @@
         "SshUsername": str,
         "SshPublicKey": str,
         "AllowSelfManagement": bool,
     },
     total=False,
 )
 
+
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "IamUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAppRequestRequestTypeDef = TypedDict(
     "DeleteAppRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 
@@ -517,19 +583,21 @@
     {
         "DeleteElasticIp": bool,
         "DeleteVolumes": bool,
     },
     total=False,
 )
 
+
 class DeleteInstanceRequestRequestTypeDef(
     _RequiredDeleteInstanceRequestRequestTypeDef, _OptionalDeleteInstanceRequestRequestTypeDef
 ):
     pass
 
+
 DeleteLayerRequestRequestTypeDef = TypedDict(
     "DeleteLayerRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 
@@ -616,20 +684,20 @@
         "StackId": str,
         "AppId": str,
         "DeploymentIds": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
+    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "EcsClusterArns": Sequence[str],
+        "StackId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEcsClustersRequestRequestTypeDef = TypedDict(
     "DescribeEcsClustersRequestRequestTypeDef",
     {
@@ -797,20 +865,22 @@
     "_OptionalDescribeRdsDbInstancesRequestRequestTypeDef",
     {
         "RdsDbInstanceArns": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeRdsDbInstancesRequestRequestTypeDef(
     _RequiredDescribeRdsDbInstancesRequestRequestTypeDef,
     _OptionalDescribeRdsDbInstancesRequestRequestTypeDef,
 ):
     pass
 
+
 RdsDbInstanceTypeDef = TypedDict(
     "RdsDbInstanceTypeDef",
     {
         "RdsDbInstanceArn": str,
         "DbInstanceIdentifier": str,
         "DbUser": str,
         "DbPassword": str,
@@ -849,14 +919,23 @@
 DescribeStackProvisioningParametersRequestRequestTypeDef = TypedDict(
     "DescribeStackProvisioningParametersRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
+DescribeStackProvisioningParametersResultTypeDef = TypedDict(
+    "DescribeStackProvisioningParametersResultTypeDef",
+    {
+        "AgentInstallerUrl": str,
+        "Parameters": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeStackSummaryRequestRequestTypeDef = TypedDict(
     "DescribeStackSummaryRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
@@ -938,40 +1017,58 @@
 DisassociateElasticIpRequestRequestTypeDef = TypedDict(
     "DisassociateElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetHostnameSuggestionRequestRequestTypeDef = TypedDict(
     "GetHostnameSuggestionRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 
+GetHostnameSuggestionResultTypeDef = TypedDict(
+    "GetHostnameSuggestionResultTypeDef",
+    {
+        "LayerId": str,
+        "Hostname": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGrantAccessRequestRequestTypeDef = TypedDict(
     "_RequiredGrantAccessRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalGrantAccessRequestRequestTypeDef = TypedDict(
     "_OptionalGrantAccessRequestRequestTypeDef",
     {
         "ValidForInMinutes": int,
     },
     total=False,
 )
 
+
 class GrantAccessRequestRequestTypeDef(
     _RequiredGrantAccessRequestRequestTypeDef, _OptionalGrantAccessRequestRequestTypeDef
 ):
     pass
 
+
 TemporaryCredentialTypeDef = TypedDict(
     "TemporaryCredentialTypeDef",
     {
         "Username": str,
         "Password": str,
         "ValidForInMinutes": int,
         "InstanceId": str,
@@ -994,14 +1091,41 @@
         "Family": str,
         "Name": str,
         "Version": str,
     },
     total=False,
 )
 
+InstancesCountResponseMetadataTypeDef = TypedDict(
+    "InstancesCountResponseMetadataTypeDef",
+    {
+        "Assigning": int,
+        "Booting": int,
+        "ConnectionLost": int,
+        "Deregistering": int,
+        "Online": int,
+        "Pending": int,
+        "Rebooting": int,
+        "Registered": int,
+        "Registering": int,
+        "Requested": int,
+        "RunningSetup": int,
+        "SetupFailed": int,
+        "ShuttingDown": int,
+        "StartFailed": int,
+        "StopFailed": int,
+        "Stopped": int,
+        "Stopping": int,
+        "Terminated": int,
+        "Terminating": int,
+        "Unassigning": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InstancesCountTypeDef = TypedDict(
     "InstancesCountTypeDef",
     {
         "Assigning": int,
         "Booting": int,
         "ConnectionLost": int,
         "Deregistering": int,
@@ -1045,51 +1169,108 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
+ListTagsResultTypeDef = TypedDict(
+    "ListTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OperatingSystemConfigurationManagerTypeDef = TypedDict(
     "OperatingSystemConfigurationManagerTypeDef",
     {
         "Name": str,
         "Version": str,
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
 RebootInstanceRequestRequestTypeDef = TypedDict(
     "RebootInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
+RecipesResponseMetadataTypeDef = TypedDict(
+    "RecipesResponseMetadataTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterEcsClusterRequestRequestTypeDef = TypedDict(
     "RegisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
         "StackId": str,
     },
 )
 
+RegisterEcsClusterResultTypeDef = TypedDict(
+    "RegisterEcsClusterResultTypeDef",
+    {
+        "EcsClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterElasticIpRequestRequestTypeDef = TypedDict(
     "RegisterElasticIpRequestRequestTypeDef",
     {
         "ElasticIp": str,
         "StackId": str,
     },
 )
 
+RegisterElasticIpResultTypeDef = TypedDict(
+    "RegisterElasticIpResultTypeDef",
+    {
+        "ElasticIp": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RegisterInstanceResultTypeDef = TypedDict(
+    "RegisterInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterRdsDbInstanceRequestRequestTypeDef = TypedDict(
     "RegisterRdsDbInstanceRequestRequestTypeDef",
     {
         "StackId": str,
         "RdsDbInstanceArn": str,
         "DbUser": str,
         "DbPassword": str,
@@ -1106,37 +1287,37 @@
     "_OptionalRegisterVolumeRequestRequestTypeDef",
     {
         "Ec2VolumeId": str,
     },
     total=False,
 )
 
+
 class RegisterVolumeRequestRequestTypeDef(
     _RequiredRegisterVolumeRequestRequestTypeDef, _OptionalRegisterVolumeRequestRequestTypeDef
 ):
     pass
 
-ServiceResourceLayerRequestTypeDef = TypedDict(
-    "ServiceResourceLayerRequestTypeDef",
-    {
-        "id": str,
-    },
-)
 
-ServiceResourceStackRequestTypeDef = TypedDict(
-    "ServiceResourceStackRequestTypeDef",
+RegisterVolumeResultTypeDef = TypedDict(
+    "RegisterVolumeResultTypeDef",
     {
-        "id": str,
+        "VolumeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServiceResourceStackSummaryRequestTypeDef = TypedDict(
-    "ServiceResourceStackSummaryRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "stack_id": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredSetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredSetPermissionRequestRequestTypeDef",
     {
         "StackId": str,
@@ -1149,33 +1330,57 @@
         "AllowSsh": bool,
         "AllowSudo": bool,
         "Level": str,
     },
     total=False,
 )
 
+
 class SetPermissionRequestRequestTypeDef(
     _RequiredSetPermissionRequestRequestTypeDef, _OptionalSetPermissionRequestRequestTypeDef
 ):
     pass
 
+
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
         "Monday": Dict[str, str],
         "Tuesday": Dict[str, str],
         "Wednesday": Dict[str, str],
         "Thursday": Dict[str, str],
         "Friday": Dict[str, str],
         "Saturday": Dict[str, str],
         "Sunday": Dict[str, str],
     },
     total=False,
 )
 
+SourceResponseMetadataTypeDef = TypedDict(
+    "SourceResponseMetadataTypeDef",
+    {
+        "Type": SourceTypeType,
+        "Url": str,
+        "Username": str,
+        "Password": str,
+        "SshKey": str,
+        "Revision": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
+    "StackConfigurationManagerResponseMetadataTypeDef",
+    {
+        "Name": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1196,19 +1401,21 @@
     "_OptionalStopInstanceRequestRequestTypeDef",
     {
         "Force": bool,
     },
     total=False,
 )
 
+
 class StopInstanceRequestRequestTypeDef(
     _RequiredStopInstanceRequestRequestTypeDef, _OptionalStopInstanceRequestRequestTypeDef
 ):
     pass
 
+
 StopStackRequestRequestTypeDef = TypedDict(
     "StopStackRequestRequestTypeDef",
     {
         "StackId": str,
     },
 )
 
@@ -1252,19 +1459,21 @@
     "_OptionalUpdateElasticIpRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateElasticIpRequestRequestTypeDef(
     _RequiredUpdateElasticIpRequestRequestTypeDef, _OptionalUpdateElasticIpRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalUpdateInstanceRequestRequestTypeDef = TypedDict(
@@ -1281,19 +1490,21 @@
         "InstallUpdatesOnBoot": bool,
         "EbsOptimized": bool,
         "AgentVersion": str,
     },
     total=False,
 )
 
+
 class UpdateInstanceRequestRequestTypeDef(
     _RequiredUpdateInstanceRequestRequestTypeDef, _OptionalUpdateInstanceRequestRequestTypeDef
 ):
     pass
 
+
 UpdateMyUserProfileRequestRequestTypeDef = TypedDict(
     "UpdateMyUserProfileRequestRequestTypeDef",
     {
         "SshPublicKey": str,
     },
     total=False,
 )
@@ -1309,20 +1520,22 @@
     {
         "DbUser": str,
         "DbPassword": str,
     },
     total=False,
 )
 
+
 class UpdateRdsDbInstanceRequestRequestTypeDef(
     _RequiredUpdateRdsDbInstanceRequestRequestTypeDef,
     _OptionalUpdateRdsDbInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -1331,19 +1544,21 @@
         "SshUsername": str,
         "SshPublicKey": str,
         "AllowSelfManagement": bool,
     },
     total=False,
 )
 
+
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
@@ -1351,19 +1566,21 @@
     {
         "Name": str,
         "MountPoint": str,
     },
     total=False,
 )
 
+
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
+
 AgentVersionTypeDef = TypedDict(
     "AgentVersionTypeDef",
     {
         "Version": str,
         "ConfigurationManager": StackConfigurationManagerTypeDef,
     },
     total=False,
@@ -1419,19 +1636,21 @@
         "SslConfiguration": SslConfigurationTypeDef,
         "Attributes": Mapping[AppAttributesKeysType, str],
         "Environment": Sequence[EnvironmentVariableTypeDef],
     },
     total=False,
 )
 
+
 class CreateAppRequestRequestTypeDef(
     _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateAppRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalUpdateAppRequestRequestTypeDef = TypedDict(
@@ -1447,19 +1666,21 @@
         "SslConfiguration": SslConfigurationTypeDef,
         "Attributes": Mapping[AppAttributesKeysType, str],
         "Environment": Sequence[EnvironmentVariableTypeDef],
     },
     total=False,
 )
 
+
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
+
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsTypeDef,
         "DownScaling": AutoScalingThresholdsTypeDef,
@@ -1479,223 +1700,33 @@
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsTypeDef,
         "DownScaling": AutoScalingThresholdsTypeDef,
     },
     total=False,
 )
 
+
 class SetLoadBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
+
 BlockDeviceMappingTypeDef = TypedDict(
     "BlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
         "NoDevice": str,
         "VirtualName": str,
         "Ebs": EbsBlockDeviceTypeDef,
     },
     total=False,
 )
 
-ChefConfigurationResponseMetadataTypeDef = TypedDict(
-    "ChefConfigurationResponseMetadataTypeDef",
-    {
-        "ManageBerkshelf": bool,
-        "BerkshelfVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CloneStackResultTypeDef = TypedDict(
-    "CloneStackResultTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppResultTypeDef = TypedDict(
-    "CreateAppResultTypeDef",
-    {
-        "AppId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResultTypeDef = TypedDict(
-    "CreateDeploymentResultTypeDef",
-    {
-        "DeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateInstanceResultTypeDef = TypedDict(
-    "CreateInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLayerResultTypeDef = TypedDict(
-    "CreateLayerResultTypeDef",
-    {
-        "LayerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStackResultTypeDef = TypedDict(
-    "CreateStackResultTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "IamUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeStackProvisioningParametersResultTypeDef = TypedDict(
-    "DescribeStackProvisioningParametersResultTypeDef",
-    {
-        "AgentInstallerUrl": str,
-        "Parameters": Dict[str, str],
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
-GetHostnameSuggestionResultTypeDef = TypedDict(
-    "GetHostnameSuggestionResultTypeDef",
-    {
-        "LayerId": str,
-        "Hostname": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InstancesCountResponseMetadataTypeDef = TypedDict(
-    "InstancesCountResponseMetadataTypeDef",
-    {
-        "Assigning": int,
-        "Booting": int,
-        "ConnectionLost": int,
-        "Deregistering": int,
-        "Online": int,
-        "Pending": int,
-        "Rebooting": int,
-        "Registered": int,
-        "Registering": int,
-        "Requested": int,
-        "RunningSetup": int,
-        "SetupFailed": int,
-        "ShuttingDown": int,
-        "StartFailed": int,
-        "StopFailed": int,
-        "Stopped": int,
-        "Stopping": int,
-        "Terminated": int,
-        "Terminating": int,
-        "Unassigning": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResultTypeDef = TypedDict(
-    "ListTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RecipesResponseMetadataTypeDef = TypedDict(
-    "RecipesResponseMetadataTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterEcsClusterResultTypeDef = TypedDict(
-    "RegisterEcsClusterResultTypeDef",
-    {
-        "EcsClusterArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterElasticIpResultTypeDef = TypedDict(
-    "RegisterElasticIpResultTypeDef",
-    {
-        "ElasticIp": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterInstanceResultTypeDef = TypedDict(
-    "RegisterInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterVolumeResultTypeDef = TypedDict(
-    "RegisterVolumeResultTypeDef",
-    {
-        "VolumeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SourceResponseMetadataTypeDef = TypedDict(
-    "SourceResponseMetadataTypeDef",
-    {
-        "Type": SourceTypeType,
-        "Url": str,
-        "Username": str,
-        "Password": str,
-        "SshKey": str,
-        "Revision": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StackConfigurationManagerResponseMetadataTypeDef = TypedDict(
-    "StackConfigurationManagerResponseMetadataTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCloneStackRequestRequestTypeDef = TypedDict(
     "_RequiredCloneStackRequestRequestTypeDef",
     {
         "SourceStackId": str,
         "ServiceRoleArn": str,
     },
 )
@@ -1722,19 +1753,21 @@
         "CloneAppIds": Sequence[str],
         "DefaultRootDeviceType": RootDeviceTypeType,
         "AgentVersion": str,
     },
     total=False,
 )
 
+
 class CloneStackRequestRequestTypeDef(
     _RequiredCloneStackRequestRequestTypeDef, _OptionalCloneStackRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStackRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStackRequestRequestTypeDef",
     {
         "Name": str,
         "Region": str,
         "ServiceRoleArn": str,
         "DefaultInstanceProfileArn": str,
@@ -1758,19 +1791,21 @@
         "DefaultSshKeyName": str,
         "DefaultRootDeviceType": RootDeviceTypeType,
         "AgentVersion": str,
     },
     total=False,
 )
 
+
 class CreateStackRequestRequestTypeDef(
     _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStackRequestServiceResourceCreateStackTypeDef = TypedDict(
     "_RequiredCreateStackRequestServiceResourceCreateStackTypeDef",
     {
         "Name": str,
         "Region": str,
         "ServiceRoleArn": str,
         "DefaultInstanceProfileArn": str,
@@ -1794,20 +1829,22 @@
         "DefaultSshKeyName": str,
         "DefaultRootDeviceType": RootDeviceTypeType,
         "AgentVersion": str,
     },
     total=False,
 )
 
+
 class CreateStackRequestServiceResourceCreateStackTypeDef(
     _RequiredCreateStackRequestServiceResourceCreateStackTypeDef,
     _OptionalCreateStackRequestServiceResourceCreateStackTypeDef,
 ):
     pass
 
+
 StackTypeDef = TypedDict(
     "StackTypeDef",
     {
         "StackId": str,
         "Name": str,
         "Arn": str,
         "Region": str,
@@ -1859,25 +1896,27 @@
         "DefaultRootDeviceType": RootDeviceTypeType,
         "UseOpsworksSecurityGroups": bool,
         "AgentVersion": str,
     },
     total=False,
 )
 
+
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
+
 CloudWatchLogsConfigurationResponseMetadataTypeDef = TypedDict(
     "CloudWatchLogsConfigurationResponseMetadataTypeDef",
     {
         "Enabled": bool,
         "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
@@ -1886,15 +1925,15 @@
     total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "StackId": str,
@@ -1909,19 +1948,21 @@
         "LayerIds": Sequence[str],
         "Comment": str,
         "CustomJson": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": str,
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
@@ -1998,110 +2039,100 @@
         "LayerId": str,
         "InstanceIds": Sequence[str],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef = TypedDict(
-    "DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef",
-    {
-        "EcsClusterArns": Sequence[str],
-        "StackId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeEcsClustersResultTypeDef = TypedDict(
     "DescribeEcsClustersResultTypeDef",
     {
         "EcsClusters": List[EcsClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticIpsResultTypeDef = TypedDict(
     "DescribeElasticIpsResultTypeDef",
     {
         "ElasticIps": List[ElasticIpTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeElasticLoadBalancersResultTypeDef = TypedDict(
     "DescribeElasticLoadBalancersResultTypeDef",
     {
         "ElasticLoadBalancers": List[ElasticLoadBalancerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMyUserProfileResultTypeDef = TypedDict(
     "DescribeMyUserProfileResultTypeDef",
     {
         "UserProfile": SelfUserProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePermissionsResultTypeDef = TypedDict(
     "DescribePermissionsResultTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRaidArraysResultTypeDef = TypedDict(
     "DescribeRaidArraysResultTypeDef",
     {
         "RaidArrays": List[RaidArrayTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRdsDbInstancesResultTypeDef = TypedDict(
     "DescribeRdsDbInstancesResultTypeDef",
     {
         "RdsDbInstances": List[RdsDbInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServiceErrorsResultTypeDef = TypedDict(
     "DescribeServiceErrorsResultTypeDef",
     {
         "ServiceErrors": List[ServiceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserProfilesResultTypeDef = TypedDict(
     "DescribeUserProfilesResultTypeDef",
     {
         "UserProfiles": List[UserProfileTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVolumesResultTypeDef = TypedDict(
     "DescribeVolumesResultTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GrantAccessResultTypeDef = TypedDict(
     "GrantAccessResultTypeDef",
     {
         "TemporaryCredential": TemporaryCredentialTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2116,19 +2147,21 @@
         "RsaPublicKey": str,
         "RsaPublicKeyFingerprint": str,
         "InstanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
+
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
+
 StackSummaryTypeDef = TypedDict(
     "StackSummaryTypeDef",
     {
         "StackId": str,
         "Name": str,
         "Arn": str,
         "LayersCount": int,
@@ -2138,15 +2171,15 @@
     total=False,
 )
 
 LifecycleEventConfigurationResponseMetadataTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseMetadataTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleEventConfigurationTypeDef = TypedDict(
     "LifecycleEventConfigurationTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
@@ -2178,50 +2211,52 @@
     "_OptionalSetTimeBasedAutoScalingRequestRequestTypeDef",
     {
         "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
     },
     total=False,
 )
 
+
 class SetTimeBasedAutoScalingRequestRequestTypeDef(
     _RequiredSetTimeBasedAutoScalingRequestRequestTypeDef,
     _OptionalSetTimeBasedAutoScalingRequestRequestTypeDef,
 ):
     pass
 
+
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": str,
         "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
     },
     total=False,
 )
 
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppsResultTypeDef = TypedDict(
     "DescribeAppsResultTypeDef",
     {
         "Apps": List[AppTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeLoadBasedAutoScalingResultTypeDef",
     {
         "LoadBasedAutoScalingConfigurations": List[LoadBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2247,19 +2282,21 @@
         "EbsOptimized": bool,
         "AgentVersion": str,
         "Tenancy": str,
     },
     total=False,
 )
 
+
 class CreateInstanceRequestRequestTypeDef(
     _RequiredCreateInstanceRequestRequestTypeDef, _OptionalCreateInstanceRequestRequestTypeDef
 ):
     pass
 
+
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AgentVersion": str,
         "AmiId": str,
         "Architecture": ArchitectureType,
         "Arn": str,
@@ -2304,31 +2341,31 @@
     total=False,
 )
 
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStackSummaryResultTypeDef = TypedDict(
     "DescribeStackSummaryResultTypeDef",
     {
         "StackSummary": StackSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLayerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLayerRequestRequestTypeDef",
     {
         "StackId": str,
@@ -2354,19 +2391,21 @@
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateLayerRequestRequestTypeDef(
     _RequiredCreateLayerRequestRequestTypeDef, _OptionalCreateLayerRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLayerRequestStackCreateLayerTypeDef = TypedDict(
     "_RequiredCreateLayerRequestStackCreateLayerTypeDef",
     {
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
     },
@@ -2388,20 +2427,22 @@
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateLayerRequestStackCreateLayerTypeDef(
     _RequiredCreateLayerRequestStackCreateLayerTypeDef,
     _OptionalCreateLayerRequestStackCreateLayerTypeDef,
 ):
     pass
 
+
 LayerTypeDef = TypedDict(
     "LayerTypeDef",
     {
         "Arn": str,
         "StackId": str,
         "LayerId": str,
         "Type": LayerTypeType,
@@ -2453,43 +2494,45 @@
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateLayerRequestRequestTypeDef(
     _RequiredUpdateLayerRequestRequestTypeDef, _OptionalUpdateLayerRequestRequestTypeDef
 ):
     pass
 
+
 DescribeOperatingSystemsResponseTypeDef = TypedDict(
     "DescribeOperatingSystemsResponseTypeDef",
     {
         "OperatingSystems": List[OperatingSystemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTimeBasedAutoScalingResultTypeDef = TypedDict(
     "DescribeTimeBasedAutoScalingResultTypeDef",
     {
         "TimeBasedAutoScalingConfigurations": List[TimeBasedAutoScalingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInstancesResultTypeDef = TypedDict(
     "DescribeInstancesResultTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLayersResultTypeDef = TypedDict(
     "DescribeLayersResultTypeDef",
     {
         "Layers": List[LayerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/waiter.py` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks/waiter.pyi` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/PKG-INFO` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.OpsWorks 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.OpsWorks 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
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
 
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworks?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -448,37 +449,44 @@
     SslConfigurationTypeDef,
     AssignInstanceRequestRequestTypeDef,
     AssignVolumeRequestRequestTypeDef,
     AssociateElasticIpRequestRequestTypeDef,
     AttachElasticLoadBalancerRequestRequestTypeDef,
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
-    ResponseMetadataTypeDef,
+    ChefConfigurationResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
+    CloneStackResultTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
+    CreateAppResultTypeDef,
     DeploymentCommandTypeDef,
+    CreateDeploymentResultTypeDef,
+    CreateInstanceResultTypeDef,
     RecipesTypeDef,
     VolumeConfigurationTypeDef,
+    CreateLayerResultTypeDef,
+    CreateStackResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
+    CreateUserProfileResultTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
     DeregisterEcsClusterRequestRequestTypeDef,
     DeregisterElasticIpRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DeregisterRdsDbInstanceRequestRequestTypeDef,
     DeregisterVolumeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAppsRequestRequestTypeDef,
     DescribeCommandsRequestRequestTypeDef,
     DescribeDeploymentsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersRequestRequestTypeDef,
     EcsClusterTypeDef,
     DescribeElasticIpsRequestRequestTypeDef,
     ElasticIpTypeDef,
     DescribeElasticLoadBalancersRequestRequestTypeDef,
     ElasticLoadBalancerTypeDef,
     DescribeInstancesRequestRequestTypeDef,
@@ -490,42 +498,53 @@
     DescribeRaidArraysRequestRequestTypeDef,
     RaidArrayTypeDef,
     DescribeRdsDbInstancesRequestRequestTypeDef,
     RdsDbInstanceTypeDef,
     DescribeServiceErrorsRequestRequestTypeDef,
     ServiceErrorTypeDef,
     DescribeStackProvisioningParametersRequestRequestTypeDef,
+    DescribeStackProvisioningParametersResultTypeDef,
     DescribeStackSummaryRequestRequestTypeDef,
     DescribeStacksRequestRequestTypeDef,
     DescribeTimeBasedAutoScalingRequestRequestTypeDef,
     DescribeUserProfilesRequestRequestTypeDef,
     UserProfileTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     VolumeTypeDef,
     DetachElasticLoadBalancerRequestRequestTypeDef,
     DisassociateElasticIpRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionRequestRequestTypeDef,
+    GetHostnameSuggestionResultTypeDef,
     GrantAccessRequestRequestTypeDef,
     TemporaryCredentialTypeDef,
     InstanceIdentityTypeDef,
     ReportedOsTypeDef,
+    InstancesCountResponseMetadataTypeDef,
     InstancesCountTypeDef,
     ShutdownEventConfigurationTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResultTypeDef,
     OperatingSystemConfigurationManagerTypeDef,
+    PaginatorConfigTypeDef,
     RebootInstanceRequestRequestTypeDef,
+    RecipesResponseMetadataTypeDef,
     RegisterEcsClusterRequestRequestTypeDef,
+    RegisterEcsClusterResultTypeDef,
     RegisterElasticIpRequestRequestTypeDef,
+    RegisterElasticIpResultTypeDef,
+    RegisterInstanceResultTypeDef,
     RegisterRdsDbInstanceRequestRequestTypeDef,
     RegisterVolumeRequestRequestTypeDef,
-    ServiceResourceLayerRequestTypeDef,
-    ServiceResourceStackRequestTypeDef,
-    ServiceResourceStackSummaryRequestTypeDef,
+    RegisterVolumeResultTypeDef,
+    ResponseMetadataTypeDef,
     SetPermissionRequestRequestTypeDef,
     WeeklyAutoScalingScheduleTypeDef,
+    SourceResponseMetadataTypeDef,
+    StackConfigurationManagerResponseMetadataTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartStackRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopStackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UnassignInstanceRequestRequestTypeDef,
     UnassignVolumeRequestRequestTypeDef,
@@ -540,34 +559,14 @@
     DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
     BlockDeviceMappingTypeDef,
-    ChefConfigurationResponseMetadataTypeDef,
-    CloneStackResultTypeDef,
-    CreateAppResultTypeDef,
-    CreateDeploymentResultTypeDef,
-    CreateInstanceResultTypeDef,
-    CreateLayerResultTypeDef,
-    CreateStackResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DescribeStackProvisioningParametersResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetHostnameSuggestionResultTypeDef,
-    InstancesCountResponseMetadataTypeDef,
-    ListTagsResultTypeDef,
-    RecipesResponseMetadataTypeDef,
-    RegisterEcsClusterResultTypeDef,
-    RegisterElasticIpResultTypeDef,
-    RegisterInstanceResultTypeDef,
-    RegisterVolumeResultTypeDef,
-    SourceResponseMetadataTypeDef,
-    StackConfigurationManagerResponseMetadataTypeDef,
     CloneStackRequestRequestTypeDef,
     CreateStackRequestRequestTypeDef,
     CreateStackRequestServiceResourceCreateStackTypeDef,
     StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationResponseMetadataTypeDef,
     CloudWatchLogsConfigurationTypeDef,
@@ -576,15 +575,14 @@
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
-    DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
     DescribeMyUserProfileResultTypeDef,
     DescribePermissionsResultTypeDef,
     DescribeRaidArraysResultTypeDef,
     DescribeRdsDbInstancesResultTypeDef,
@@ -625,42 +623,42 @@
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

### Comparing `mypy-boto3-opsworks-1.26.0.post1/mypy_boto3_opsworks.egg-info/SOURCES.txt` & `mypy-boto3-opsworks-1.27.0/mypy_boto3_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.26.0.post1/setup.py` & `mypy-boto3-opsworks-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-opsworks.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworks",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorks 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.OpsWorks 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 opsworks type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_opsworks": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_opsworks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/",
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


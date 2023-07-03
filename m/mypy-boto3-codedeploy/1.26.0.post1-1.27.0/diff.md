# Comparing `tmp/mypy-boto3-codedeploy-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codedeploy-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codedeploy-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:14 2022, max compression
+gzip compressed data, was "mypy-boto3-codedeploy-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-codedeploy-1.26.0.post1.tar` & `mypy-boto3-codedeploy-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.096817 mypy-boto3-codedeploy-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21664 2022-11-01 21:43:14.096817 mypy-boto3-codedeploy-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20211 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.072817 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46184 2022-11-01 21:31:52.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    46120 2022-11-01 21:31:52.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13661 2022-11-01 21:31:53.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13659 2022-11-01 21:31:53.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12109 2022-11-01 21:31:52.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12098 2022-11-01 21:31:52.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    50593 2022-11-01 21:31:54.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    50560 2022-11-01 21:31:53.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-11-01 21:31:52.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-11-01 21:31:52.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.096817 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21664 2022-11-01 21:43:13.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-01 21:43:13.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:13.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:13.000000 mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:14.096817 mypy-boto3-codedeploy-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-01 21:31:51.000000 mypy-boto3-codedeploy-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.858986 mypy-boto3-codedeploy-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-07-03 19:50:31.854986 mypy-boto3-codedeploy-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.854986 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46184 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50681 2023-07-03 19:34:20.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-03 19:34:19.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.854986 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-07-03 19:50:31.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:50:31.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:31.000000 mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.858986 mypy-boto3-codedeploy-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:34:18.000000 mypy-boto3-codedeploy-1.27.0/setup.py
```

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/LICENSE` & `mypy-boto3-codedeploy-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/PKG-INFO` & `mypy-boto3-codedeploy-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeDeploy 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeDeploy 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
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
 
 <a id="mypy-boto3-codedeploy"></a>
 
 # mypy-boto3-codedeploy
 
 [![PyPI - mypy-boto3-codedeploy](https://img.shields.io/pypi/v/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codedeploy?color=blue)](https://pypistats.org/packages/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -421,119 +422,119 @@
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
+    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
     TriggerConfigTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
     GitHubLocationTypeDef,
     LambdaFunctionInfoTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
     TimeRangeTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
+    StopDeploymentOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
+    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    CreateApplicationOutputTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
-    DeleteDeploymentGroupOutputTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
-    StopDeploymentOutputTypeDef,
+    DeleteDeploymentGroupOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
     EC2TagSetTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
     OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
@@ -578,42 +579,42 @@
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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/README.md` & `mypy-boto3-codedeploy-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codedeploy"></a>
 
 # mypy-boto3-codedeploy
 
 [![PyPI - mypy-boto3-codedeploy](https://img.shields.io/pypi/v/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codedeploy?color=blue)](https://pypistats.org/packages/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,119 +390,119 @@
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
+    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
     TriggerConfigTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
     GitHubLocationTypeDef,
     LambdaFunctionInfoTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
     TimeRangeTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
+    StopDeploymentOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
+    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    CreateApplicationOutputTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
-    DeleteDeploymentGroupOutputTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
-    StopDeploymentOutputTypeDef,
+    DeleteDeploymentGroupOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
     EC2TagSetTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
     OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
@@ -547,42 +547,42 @@
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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/__init__.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/__init__.pyi` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/__main__.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeDeploy 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CodeDeploy 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/client.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/client.pyi` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/literals.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,23 +200,25 @@
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
@@ -226,30 +228,35 @@
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
@@ -275,14 +282,15 @@
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
@@ -327,51 +335,57 @@
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
@@ -384,14 +398,15 @@
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
@@ -403,28 +418,35 @@
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
@@ -433,14 +455,15 @@
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
@@ -451,55 +474,64 @@
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
@@ -536,21 +568,25 @@
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
+    "eu-central-2",
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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/literals.pyi` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -198,23 +198,25 @@
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
@@ -224,30 +226,35 @@
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
@@ -273,14 +280,15 @@
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
@@ -325,51 +333,57 @@
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
@@ -382,14 +396,15 @@
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
@@ -401,28 +416,35 @@
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
@@ -431,14 +453,15 @@
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
@@ -449,55 +472,64 @@
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
@@ -534,21 +566,25 @@
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
+    "eu-central-2",
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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/paginator.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,60 +98,60 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
         """
 
 
 class ListDeploymentConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
         """
 
 
 class ListDeploymentGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
     """
 
     def paginate(
-        self, *, applicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
         """
 
 
@@ -163,15 +163,15 @@
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
 
@@ -182,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         deploymentId: str = ...,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
 
@@ -204,30 +204,30 @@
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentspaginator)
         """
 
 
 class ListGitHubAccountTokenNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGitHubAccountTokenNamesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
         """
 
 
@@ -238,13 +238,13 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/paginator.pyi` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -95,57 +95,57 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listapplicationspaginator)
         """
 
 class ListDeploymentConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentconfigspaginator)
         """
 
 class ListDeploymentGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
     """
 
     def paginate(
-        self, *, applicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentgroupspaginator)
         """
 
 class ListDeploymentInstancesPaginator(Paginator):
@@ -156,15 +156,15 @@
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
 class ListDeploymentTargetsPaginator(Paginator):
@@ -174,15 +174,15 @@
     """
 
     def paginate(
         self,
         *,
         deploymentId: str = ...,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
@@ -195,29 +195,29 @@
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listdeploymentspaginator)
         """
 
 class ListGitHubAccountTokenNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGitHubAccountTokenNamesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listgithubaccounttokennamespaginator)
         """
 
 class ListOnPremisesInstancesPaginator(Paginator):
@@ -227,13 +227,13 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/type_defs.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,119 +60,119 @@
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
+    "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
+    "CreateDeploymentConfigOutputTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
     "TriggerConfigTypeDef",
+    "CreateDeploymentGroupOutputTypeDef",
+    "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
+    "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
     "ELBInfoTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
     "GitHubLocationTypeDef",
     "LambdaFunctionInfoTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
+    "ListApplicationsOutputTypeDef",
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
+    "ListDeploymentConfigsOutputTypeDef",
+    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
+    "ListDeploymentGroupsOutputTypeDef",
+    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
+    "ListDeploymentInstancesOutputTypeDef",
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
+    "ListDeploymentTargetsOutputTypeDef",
     "TimeRangeTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
+    "StopDeploymentOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "AlarmConfigurationTypeDef",
     "BatchGetApplicationsOutputTypeDef",
-    "CreateApplicationOutputTypeDef",
-    "CreateDeploymentConfigOutputTypeDef",
-    "CreateDeploymentGroupOutputTypeDef",
-    "CreateDeploymentOutputTypeDef",
-    "DeleteDeploymentGroupOutputTypeDef",
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationOutputTypeDef",
-    "ListApplicationsOutputTypeDef",
-    "ListDeploymentConfigsOutputTypeDef",
-    "ListDeploymentGroupsOutputTypeDef",
-    "ListDeploymentInstancesOutputTypeDef",
-    "ListDeploymentTargetsOutputTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    "ListOnPremisesInstancesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    "StopDeploymentOutputTypeDef",
+    "DeleteDeploymentGroupOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
     "EC2TagSetTypeDef",
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
     "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
-    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "RevisionLocationTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
@@ -262,25 +262,14 @@
     {
         "name": str,
         "hook": str,
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
 BatchGetApplicationsInputRequestTypeDef = TypedDict(
     "BatchGetApplicationsInputRequestTypeDef",
     {
         "applicationNames": Sequence[str],
     },
 )
 
@@ -354,23 +343,39 @@
     {
         "deploymentId": str,
         "deploymentWaitType": DeploymentWaitTypeType,
     },
     total=False,
 )
 
+CreateApplicationOutputTypeDef = TypedDict(
+    "CreateApplicationOutputTypeDef",
+    {
+        "applicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MinimumHealthyHostsTypeDef = TypedDict(
     "MinimumHealthyHostsTypeDef",
     {
         "type": MinimumHealthyHostsTypeType,
         "value": int,
     },
     total=False,
 )
 
+CreateDeploymentConfigOutputTypeDef = TypedDict(
+    "CreateDeploymentConfigOutputTypeDef",
+    {
+        "deploymentConfigId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeploymentStyleTypeDef = TypedDict(
     "DeploymentStyleTypeDef",
     {
         "deploymentType": DeploymentTypeType,
         "deploymentOption": DeploymentOptionType,
     },
     total=False,
@@ -411,14 +416,30 @@
         "triggerName": str,
         "triggerTargetArn": str,
         "triggerEvents": List[TriggerEventTypeType],
     },
     total=False,
 )
 
+CreateDeploymentGroupOutputTypeDef = TypedDict(
+    "CreateDeploymentGroupOutputTypeDef",
+    {
+        "deploymentGroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDeploymentOutputTypeDef = TypedDict(
+    "CreateDeploymentOutputTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -441,14 +462,22 @@
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     {
         "tokenName": str,
     },
     total=False,
 )
 
+DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    {
+        "tokenName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcesByExternalIdInputRequestTypeDef = TypedDict(
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
@@ -535,14 +564,21 @@
     "ELBInfoTypeDef",
     {
         "name": str,
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
 GenericRevisionInfoTypeDef = TypedDict(
     "GenericRevisionInfoTypeDef",
     {
         "description": str,
         "deploymentGroups": List[str],
         "firstUsedTime": datetime,
         "lastUsedTime": datetime,
@@ -630,24 +666,41 @@
         "currentVersion": str,
         "targetVersion": str,
         "targetVersionWeight": float,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "applicationName": str,
+    },
+)
+_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "sortBy": ApplicationRevisionSortByType,
+        "sortOrder": SortOrderType,
+        "s3Bucket": str,
+        "s3KeyPrefix": str,
+        "deployed": ListStateFilterActionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
+    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApplicationRevisionsInputRequestTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputRequestTypeDef = TypedDict(
@@ -667,30 +720,86 @@
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
 
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
+    {
+        "applications": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeploymentConfigsInputRequestTypeDef = TypedDict(
     "ListDeploymentConfigsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListDeploymentConfigsOutputTypeDef = TypedDict(
+    "ListDeploymentConfigsOutputTypeDef",
+    {
+        "deploymentConfigsList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "applicationName": str,
+    },
+)
+_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
+    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentGroupsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListDeploymentGroupsInputRequestTypeDef = TypedDict(
@@ -705,14 +814,48 @@
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
 
+ListDeploymentGroupsOutputTypeDef = TypedDict(
+    "ListDeploymentGroupsOutputTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "deploymentId": str,
+    },
+)
+_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "instanceStatusFilter": Sequence[InstanceStatusType],
+        "instanceTypeFilter": Sequence[InstanceTypeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
+    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputRequestTypeDef = TypedDict(
@@ -729,41 +872,104 @@
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
 
+ListDeploymentInstancesOutputTypeDef = TypedDict(
+    "ListDeploymentInstancesOutputTypeDef",
+    {
+        "instancesList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    {
+        "deploymentId": str,
+        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
+ListDeploymentTargetsOutputTypeDef = TypedDict(
+    "ListDeploymentTargetsOutputTypeDef",
+    {
+        "targetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "start": Union[datetime, str],
         "end": Union[datetime, str],
     },
     total=False,
 )
 
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    {
+        "tokenNameList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListOnPremisesInstancesOutputTypeDef = TypedDict(
+    "ListOnPremisesInstancesOutputTypeDef",
+    {
+        "instanceNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -777,24 +983,42 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
     total=False,
 )
 
+PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    {
+        "lifecycleEventHookExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -819,14 +1043,25 @@
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
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
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -860,14 +1095,23 @@
 
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
 
+StopDeploymentOutputTypeDef = TypedDict(
+    "StopDeploymentOutputTypeDef",
+    {
+        "status": StopStatusType,
+        "statusMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
         "listenerArns": List[str],
     },
     total=False,
 )
@@ -947,14 +1191,23 @@
         "registerTime": datetime,
         "deregisterTime": datetime,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -977,185 +1230,39 @@
     total=False,
 )
 
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationOutputTypeDef = TypedDict(
-    "CreateApplicationOutputTypeDef",
-    {
-        "applicationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentConfigOutputTypeDef = TypedDict(
-    "CreateDeploymentConfigOutputTypeDef",
-    {
-        "deploymentConfigId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentGroupOutputTypeDef = TypedDict(
-    "CreateDeploymentGroupOutputTypeDef",
-    {
-        "deploymentGroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentOutputTypeDef = TypedDict(
-    "CreateDeploymentOutputTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDeploymentGroupOutputTypeDef = TypedDict(
-    "DeleteDeploymentGroupOutputTypeDef",
-    {
-        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    {
-        "tokenName": str,
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
 
 GetApplicationOutputTypeDef = TypedDict(
     "GetApplicationOutputTypeDef",
     {
         "application": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
-    {
-        "applications": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentConfigsOutputTypeDef = TypedDict(
-    "ListDeploymentConfigsOutputTypeDef",
-    {
-        "deploymentConfigsList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentGroupsOutputTypeDef = TypedDict(
-    "ListDeploymentGroupsOutputTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDeploymentInstancesOutputTypeDef = TypedDict(
-    "ListDeploymentInstancesOutputTypeDef",
-    {
-        "instancesList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentTargetsOutputTypeDef = TypedDict(
-    "ListDeploymentTargetsOutputTypeDef",
-    {
-        "targetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
-    {
-        "deployments": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    {
-        "tokenNameList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListOnPremisesInstancesOutputTypeDef = TypedDict(
-    "ListOnPremisesInstancesOutputTypeDef",
-    {
-        "instanceNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    {
-        "lifecycleEventHookExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopDeploymentOutputTypeDef = TypedDict(
-    "StopDeploymentOutputTypeDef",
+DeleteDeploymentGroupOutputTypeDef = TypedDict(
+    "DeleteDeploymentGroupOutputTypeDef",
     {
-        "status": StopStatusType,
-        "statusMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDeploymentGroupOutputTypeDef = TypedDict(
     "UpdateDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
@@ -1169,14 +1276,24 @@
     "EC2TagSetTypeDef",
     {
         "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
+ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+        "tagFilters": Sequence[TagFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
@@ -1236,140 +1353,23 @@
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
 
-_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "sortBy": ApplicationRevisionSortByType,
-        "sortOrder": SortOrderType,
-        "s3Bucket": str,
-        "s3KeyPrefix": str,
-        "deployed": ListStateFilterActionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
-    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-):
-    pass
-
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
-    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "deploymentId": str,
-    },
-)
-_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "instanceStatusFilter": Sequence[InstanceStatusType],
-        "instanceTypeFilter": Sequence[InstanceTypeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
-    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-):
-    pass
-
-
-ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    {
-        "deploymentId": str,
-        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
-    {
-        "registrationStatus": RegistrationStatusType,
-        "tagFilters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "externalId": str,
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDeploymentsInputRequestTypeDef = TypedDict(
     "ListDeploymentsInputRequestTypeDef",
     {
@@ -1415,23 +1415,23 @@
     total=False,
 )
 
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOnPremisesInstanceOutputTypeDef = TypedDict(
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetInstancesTypeDef = TypedDict(
     "TargetInstancesTypeDef",
     {
         "tagFilters": List[EC2TagFilterTypeDef],
@@ -1528,24 +1528,24 @@
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
         "revision": RevisionLocationTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
         "revisions": List[RevisionLocationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1655,23 +1655,23 @@
 
 
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentInstanceOutputTypeDef = TypedDict(
     "GetDeploymentInstanceOutputTypeDef",
     {
         "instanceSummary": InstanceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentTargetTypeDef = TypedDict(
     "DeploymentTargetTypeDef",
     {
         "deploymentTargetType": DeploymentTargetTypeType,
@@ -1685,15 +1685,15 @@
 
 BatchGetApplicationRevisionsOutputTypeDef = TypedDict(
     "BatchGetApplicationRevisionsOutputTypeDef",
     {
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1835,59 +1835,59 @@
     pass
 
 
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDeploymentTargetsOutputTypeDef = TypedDict(
     "BatchGetDeploymentTargetsOutputTypeDef",
     {
         "deploymentTargets": List[DeploymentTargetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentTargetOutputTypeDef = TypedDict(
     "GetDeploymentTargetOutputTypeDef",
     {
         "deploymentTarget": DeploymentTargetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDeploymentGroupsOutputTypeDef = TypedDict(
     "BatchGetDeploymentGroupsOutputTypeDef",
     {
         "deploymentGroupsInfo": List[DeploymentGroupInfoTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentGroupOutputTypeDef = TypedDict(
     "GetDeploymentGroupOutputTypeDef",
     {
         "deploymentGroupInfo": DeploymentGroupInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDeploymentsOutputTypeDef = TypedDict(
     "BatchGetDeploymentsOutputTypeDef",
     {
         "deploymentsInfo": List[DeploymentInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentOutputTypeDef = TypedDict(
     "GetDeploymentOutputTypeDef",
     {
         "deploymentInfo": DeploymentInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/type_defs.pyi` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -59,119 +59,119 @@
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
+    "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
+    "CreateDeploymentConfigOutputTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
     "TriggerConfigTypeDef",
+    "CreateDeploymentGroupOutputTypeDef",
+    "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
+    "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
     "ELBInfoTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
     "GitHubLocationTypeDef",
     "LambdaFunctionInfoTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
+    "ListApplicationsOutputTypeDef",
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
+    "ListDeploymentConfigsOutputTypeDef",
+    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
+    "ListDeploymentGroupsOutputTypeDef",
+    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
+    "ListDeploymentInstancesOutputTypeDef",
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
+    "ListDeploymentTargetsOutputTypeDef",
     "TimeRangeTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
+    "StopDeploymentOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "AlarmConfigurationTypeDef",
     "BatchGetApplicationsOutputTypeDef",
-    "CreateApplicationOutputTypeDef",
-    "CreateDeploymentConfigOutputTypeDef",
-    "CreateDeploymentGroupOutputTypeDef",
-    "CreateDeploymentOutputTypeDef",
-    "DeleteDeploymentGroupOutputTypeDef",
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationOutputTypeDef",
-    "ListApplicationsOutputTypeDef",
-    "ListDeploymentConfigsOutputTypeDef",
-    "ListDeploymentGroupsOutputTypeDef",
-    "ListDeploymentInstancesOutputTypeDef",
-    "ListDeploymentTargetsOutputTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    "ListOnPremisesInstancesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    "StopDeploymentOutputTypeDef",
+    "DeleteDeploymentGroupOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
     "EC2TagSetTypeDef",
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
     "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
-    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "RevisionLocationTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
@@ -261,25 +261,14 @@
     {
         "name": str,
         "hook": str,
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
 BatchGetApplicationsInputRequestTypeDef = TypedDict(
     "BatchGetApplicationsInputRequestTypeDef",
     {
         "applicationNames": Sequence[str],
     },
 )
 
@@ -353,23 +342,39 @@
     {
         "deploymentId": str,
         "deploymentWaitType": DeploymentWaitTypeType,
     },
     total=False,
 )
 
+CreateApplicationOutputTypeDef = TypedDict(
+    "CreateApplicationOutputTypeDef",
+    {
+        "applicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MinimumHealthyHostsTypeDef = TypedDict(
     "MinimumHealthyHostsTypeDef",
     {
         "type": MinimumHealthyHostsTypeType,
         "value": int,
     },
     total=False,
 )
 
+CreateDeploymentConfigOutputTypeDef = TypedDict(
+    "CreateDeploymentConfigOutputTypeDef",
+    {
+        "deploymentConfigId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeploymentStyleTypeDef = TypedDict(
     "DeploymentStyleTypeDef",
     {
         "deploymentType": DeploymentTypeType,
         "deploymentOption": DeploymentOptionType,
     },
     total=False,
@@ -410,14 +415,30 @@
         "triggerName": str,
         "triggerTargetArn": str,
         "triggerEvents": List[TriggerEventTypeType],
     },
     total=False,
 )
 
+CreateDeploymentGroupOutputTypeDef = TypedDict(
+    "CreateDeploymentGroupOutputTypeDef",
+    {
+        "deploymentGroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDeploymentOutputTypeDef = TypedDict(
+    "CreateDeploymentOutputTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -440,14 +461,22 @@
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     {
         "tokenName": str,
     },
     total=False,
 )
 
+DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    {
+        "tokenName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcesByExternalIdInputRequestTypeDef = TypedDict(
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
@@ -534,14 +563,21 @@
     "ELBInfoTypeDef",
     {
         "name": str,
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
 GenericRevisionInfoTypeDef = TypedDict(
     "GenericRevisionInfoTypeDef",
     {
         "description": str,
         "deploymentGroups": List[str],
         "firstUsedTime": datetime,
         "lastUsedTime": datetime,
@@ -629,24 +665,39 @@
         "currentVersion": str,
         "targetVersion": str,
         "targetVersionWeight": float,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "applicationName": str,
+    },
+)
+_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "sortBy": ApplicationRevisionSortByType,
+        "sortOrder": SortOrderType,
+        "s3Bucket": str,
+        "s3KeyPrefix": str,
+        "deployed": ListStateFilterActionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
+    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListApplicationRevisionsInputRequestTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputRequestTypeDef = TypedDict(
@@ -664,30 +715,84 @@
 
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
+    {
+        "applications": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeploymentConfigsInputRequestTypeDef = TypedDict(
     "ListDeploymentConfigsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListDeploymentConfigsOutputTypeDef = TypedDict(
+    "ListDeploymentConfigsOutputTypeDef",
+    {
+        "deploymentConfigsList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "applicationName": str,
+    },
+)
+_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
+    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentGroupsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListDeploymentGroupsInputRequestTypeDef = TypedDict(
@@ -700,14 +805,46 @@
 
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
+ListDeploymentGroupsOutputTypeDef = TypedDict(
+    "ListDeploymentGroupsOutputTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "deploymentId": str,
+    },
+)
+_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "instanceStatusFilter": Sequence[InstanceStatusType],
+        "instanceTypeFilter": Sequence[InstanceTypeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
+    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputRequestTypeDef = TypedDict(
@@ -722,41 +859,104 @@
 
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
+ListDeploymentInstancesOutputTypeDef = TypedDict(
+    "ListDeploymentInstancesOutputTypeDef",
+    {
+        "instancesList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    {
+        "deploymentId": str,
+        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
+ListDeploymentTargetsOutputTypeDef = TypedDict(
+    "ListDeploymentTargetsOutputTypeDef",
+    {
+        "targetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "start": Union[datetime, str],
         "end": Union[datetime, str],
     },
     total=False,
 )
 
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    {
+        "tokenNameList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListOnPremisesInstancesOutputTypeDef = TypedDict(
+    "ListOnPremisesInstancesOutputTypeDef",
+    {
+        "instanceNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -768,24 +968,42 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
     total=False,
 )
 
+PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    {
+        "lifecycleEventHookExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -808,14 +1026,25 @@
 
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
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
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -847,14 +1076,23 @@
 )
 
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
+StopDeploymentOutputTypeDef = TypedDict(
+    "StopDeploymentOutputTypeDef",
+    {
+        "status": StopStatusType,
+        "statusMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
         "listenerArns": List[str],
     },
     total=False,
 )
@@ -932,14 +1170,23 @@
         "registerTime": datetime,
         "deregisterTime": datetime,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -962,185 +1209,39 @@
     total=False,
 )
 
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationOutputTypeDef = TypedDict(
-    "CreateApplicationOutputTypeDef",
-    {
-        "applicationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentConfigOutputTypeDef = TypedDict(
-    "CreateDeploymentConfigOutputTypeDef",
-    {
-        "deploymentConfigId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentGroupOutputTypeDef = TypedDict(
-    "CreateDeploymentGroupOutputTypeDef",
-    {
-        "deploymentGroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentOutputTypeDef = TypedDict(
-    "CreateDeploymentOutputTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDeploymentGroupOutputTypeDef = TypedDict(
-    "DeleteDeploymentGroupOutputTypeDef",
-    {
-        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    {
-        "tokenName": str,
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
 
 GetApplicationOutputTypeDef = TypedDict(
     "GetApplicationOutputTypeDef",
     {
         "application": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
-    {
-        "applications": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentConfigsOutputTypeDef = TypedDict(
-    "ListDeploymentConfigsOutputTypeDef",
-    {
-        "deploymentConfigsList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentGroupsOutputTypeDef = TypedDict(
-    "ListDeploymentGroupsOutputTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDeploymentInstancesOutputTypeDef = TypedDict(
-    "ListDeploymentInstancesOutputTypeDef",
-    {
-        "instancesList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentTargetsOutputTypeDef = TypedDict(
-    "ListDeploymentTargetsOutputTypeDef",
-    {
-        "targetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
-    {
-        "deployments": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    {
-        "tokenNameList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListOnPremisesInstancesOutputTypeDef = TypedDict(
-    "ListOnPremisesInstancesOutputTypeDef",
-    {
-        "instanceNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    {
-        "lifecycleEventHookExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopDeploymentOutputTypeDef = TypedDict(
-    "StopDeploymentOutputTypeDef",
+DeleteDeploymentGroupOutputTypeDef = TypedDict(
+    "DeleteDeploymentGroupOutputTypeDef",
     {
-        "status": StopStatusType,
-        "statusMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDeploymentGroupOutputTypeDef = TypedDict(
     "UpdateDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
@@ -1154,14 +1255,24 @@
     "EC2TagSetTypeDef",
     {
         "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
+ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+        "tagFilters": Sequence[TagFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
@@ -1219,134 +1330,23 @@
 
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
-_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "sortBy": ApplicationRevisionSortByType,
-        "sortOrder": SortOrderType,
-        "s3Bucket": str,
-        "s3KeyPrefix": str,
-        "deployed": ListStateFilterActionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
-    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-):
-    pass
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
-    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "deploymentId": str,
-    },
-)
-_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "instanceStatusFilter": Sequence[InstanceStatusType],
-        "instanceTypeFilter": Sequence[InstanceTypeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
-    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-):
-    pass
-
-ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    {
-        "deploymentId": str,
-        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
-    {
-        "registrationStatus": RegistrationStatusType,
-        "tagFilters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     {
         "applicationName": str,
         "deploymentGroupName": str,
         "externalId": str,
         "includeOnlyStatuses": Sequence[DeploymentStatusType],
         "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDeploymentsInputRequestTypeDef = TypedDict(
     "ListDeploymentsInputRequestTypeDef",
     {
@@ -1392,23 +1392,23 @@
     total=False,
 )
 
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOnPremisesInstanceOutputTypeDef = TypedDict(
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetInstancesTypeDef = TypedDict(
     "TargetInstancesTypeDef",
     {
         "tagFilters": List[EC2TagFilterTypeDef],
@@ -1505,24 +1505,24 @@
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
         "revision": RevisionLocationTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
         "revisions": List[RevisionLocationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1626,23 +1626,23 @@
     pass
 
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentInstanceOutputTypeDef = TypedDict(
     "GetDeploymentInstanceOutputTypeDef",
     {
         "instanceSummary": InstanceSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentTargetTypeDef = TypedDict(
     "DeploymentTargetTypeDef",
     {
         "deploymentTargetType": DeploymentTargetTypeType,
@@ -1656,15 +1656,15 @@
 
 BatchGetApplicationRevisionsOutputTypeDef = TypedDict(
     "BatchGetApplicationRevisionsOutputTypeDef",
     {
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1802,59 +1802,59 @@
 ):
     pass
 
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDeploymentTargetsOutputTypeDef = TypedDict(
     "BatchGetDeploymentTargetsOutputTypeDef",
     {
         "deploymentTargets": List[DeploymentTargetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentTargetOutputTypeDef = TypedDict(
     "GetDeploymentTargetOutputTypeDef",
     {
         "deploymentTarget": DeploymentTargetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDeploymentGroupsOutputTypeDef = TypedDict(
     "BatchGetDeploymentGroupsOutputTypeDef",
     {
         "deploymentGroupsInfo": List[DeploymentGroupInfoTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentGroupOutputTypeDef = TypedDict(
     "GetDeploymentGroupOutputTypeDef",
     {
         "deploymentGroupInfo": DeploymentGroupInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDeploymentsOutputTypeDef = TypedDict(
     "BatchGetDeploymentsOutputTypeDef",
     {
         "deploymentsInfo": List[DeploymentInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentOutputTypeDef = TypedDict(
     "GetDeploymentOutputTypeDef",
     {
         "deploymentInfo": DeploymentInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/waiter.py` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy/waiter.pyi` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/PKG-INFO` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codedeploy
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeDeploy 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeDeploy 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/
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
 
 <a id="mypy-boto3-codedeploy"></a>
 
 # mypy-boto3-codedeploy
 
 [![PyPI - mypy-boto3-codedeploy](https://img.shields.io/pypi/v/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codedeploy.svg?color=blue)](https://pypi.org/project/mypy-boto3-codedeploy)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codedeploy?color=blue)](https://pypistats.org/packages/mypy-boto3-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeDeploy 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
+[boto3.CodeDeploy 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [mypy-boto3-codedeploy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -421,119 +422,119 @@
 from mypy_boto3_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
+    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
     TriggerConfigTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
+    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
     GitHubLocationTypeDef,
     LambdaFunctionInfoTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
     TimeRangeTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
+    StopDeploymentOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
+    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     AlarmConfigurationTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    CreateApplicationOutputTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
-    DeleteDeploymentGroupOutputTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
-    StopDeploymentOutputTypeDef,
+    DeleteDeploymentGroupOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
     EC2TagSetTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
     OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListDeploymentsInputListDeploymentsPaginateTypeDef,
     ListDeploymentsInputRequestTypeDef,
     RevisionLocationTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
@@ -578,42 +579,42 @@
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

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/mypy_boto3_codedeploy.egg-info/SOURCES.txt` & `mypy-boto3-codedeploy-1.27.0/mypy_boto3_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codedeploy-1.26.0.post1/setup.py` & `mypy-boto3-codedeploy-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codedeploy.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codedeploy",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeDeploy 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CodeDeploy 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 codedeploy type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codedeploy": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codedeploy": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/",
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


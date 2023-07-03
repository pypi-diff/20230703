# Comparing `tmp/mypy-boto3-devicefarm-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-devicefarm-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devicefarm-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:20 2022, max compression
+gzip compressed data, was "mypy-boto3-devicefarm-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-devicefarm-1.26.0.post1.tar` & `mypy-boto3-devicefarm-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:20.196823 mypy-boto3-devicefarm-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    24679 2022-11-01 21:43:20.196823 mypy-boto3-devicefarm-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23226 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:20.196823 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    57699 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    57595 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    15009 2022-11-01 21:32:47.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    15007 2022-11-01 21:32:46.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22346 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    22324 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    73078 2022-11-01 21:32:48.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    72987 2022-11-01 21:32:47.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:20.196823 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24679 2022-11-01 21:43:20.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-01 21:43:20.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:20.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:20.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:20.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:20.000000 mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:20.196823 mypy-boto3-devicefarm-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-01 21:32:45.000000 mypy-boto3-devicefarm-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.755111 mypy-boto3-devicefarm-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24704 2023-07-03 19:50:38.751111 mypy-boto3-devicefarm-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.751111 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57697 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57593 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15714 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    73250 2023-07-03 19:35:30.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73159 2023-07-03 19:35:29.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.751111 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24704 2023-07-03 19:50:38.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:38.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:38.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:38.000000 mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.755111 mypy-boto3-devicefarm-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:35:27.000000 mypy-boto3-devicefarm-1.27.0/setup.py
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/LICENSE` & `mypy-boto3-devicefarm-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/PKG-INFO` & `mypy-boto3-devicefarm-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DeviceFarm 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.DeviceFarm 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
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
 
 <a id="mypy-boto3-devicefarm"></a>
 
 # mypy-boto3-devicefarm
 
 [![PyPI - mypy-boto3-devicefarm](https://img.shields.io/pypi/v/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devicefarm?color=blue)](https://pypistats.org/packages/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -427,23 +428,23 @@
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
     RuleTypeDef,
-    ResponseMetadataTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     InstanceProfileTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     VpcConfigTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
+    CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
@@ -462,76 +463,95 @@
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
     GetOfferingStatusRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetRemoteAccessSessionRequestRequestTypeDef,
     GetRunRequestRequestTypeDef,
     GetSuiteRequestRequestTypeDef,
     GetTestGridProjectRequestRequestTypeDef,
     GetTestGridSessionRequestRequestTypeDef,
     TestGridSessionTypeDef,
     GetTestRequestRequestTypeDef,
     GetUploadRequestRequestTypeDef,
     GetVPCEConfigurationRequestRequestTypeDef,
     InstallToRemoteAccessSessionRequestRequestTypeDef,
+    ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListArtifactsRequestRequestTypeDef,
+    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDeviceInstancesRequestRequestTypeDef,
+    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     ListDevicePoolsRequestRequestTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListNetworkProfilesRequestRequestTypeDef,
+    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingPromotionsRequestRequestTypeDef,
     OfferingPromotionTypeDef,
+    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingTransactionsRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
+    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
     ListRemoteAccessSessionsRequestRequestTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
+    ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
+    ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
+    ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
+    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
+    ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
+    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
+    PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
+    ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
     DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
-    CreateTestGridUrlResultTypeDef,
-    ListArtifactsResultTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
@@ -551,37 +571,18 @@
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionConfigurationTypeDef,
     DeviceSelectionResultTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
-    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
-    ListArtifactsRequestListArtifactsPaginateTypeDef,
-    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
-    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
-    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
-    ListSamplesRequestListSamplesPaginateTypeDef,
-    ListSuitesRequestListSuitesPaginateTypeDef,
-    ListTestsRequestListTestsPaginateTypeDef,
-    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    ListUploadsRequestListUploadsPaginateTypeDef,
-    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
@@ -650,42 +651,42 @@
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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/README.md` & `mypy-boto3-devicefarm-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-devicefarm"></a>
 
 # mypy-boto3-devicefarm
 
 [![PyPI - mypy-boto3-devicefarm](https://img.shields.io/pypi/v/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devicefarm?color=blue)](https://pypistats.org/packages/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,23 +396,23 @@
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
     RuleTypeDef,
-    ResponseMetadataTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     InstanceProfileTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     VpcConfigTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
+    CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
@@ -431,76 +431,95 @@
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
     GetOfferingStatusRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetRemoteAccessSessionRequestRequestTypeDef,
     GetRunRequestRequestTypeDef,
     GetSuiteRequestRequestTypeDef,
     GetTestGridProjectRequestRequestTypeDef,
     GetTestGridSessionRequestRequestTypeDef,
     TestGridSessionTypeDef,
     GetTestRequestRequestTypeDef,
     GetUploadRequestRequestTypeDef,
     GetVPCEConfigurationRequestRequestTypeDef,
     InstallToRemoteAccessSessionRequestRequestTypeDef,
+    ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListArtifactsRequestRequestTypeDef,
+    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDeviceInstancesRequestRequestTypeDef,
+    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     ListDevicePoolsRequestRequestTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListNetworkProfilesRequestRequestTypeDef,
+    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingPromotionsRequestRequestTypeDef,
     OfferingPromotionTypeDef,
+    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingTransactionsRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
+    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
     ListRemoteAccessSessionsRequestRequestTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
+    ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
+    ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
+    ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
+    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
+    ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
+    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
+    PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
+    ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
     DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
-    CreateTestGridUrlResultTypeDef,
-    ListArtifactsResultTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
@@ -520,37 +539,18 @@
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionConfigurationTypeDef,
     DeviceSelectionResultTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
-    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
-    ListArtifactsRequestListArtifactsPaginateTypeDef,
-    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
-    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
-    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
-    ListSamplesRequestListSamplesPaginateTypeDef,
-    ListSuitesRequestListSuitesPaginateTypeDef,
-    ListTestsRequestListTestsPaginateTypeDef,
-    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    ListUploadsRequestListUploadsPaginateTypeDef,
-    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
@@ -619,42 +619,42 @@
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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/__init__.py` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/__init__.pyi` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/__main__.py` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DeviceFarm 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.DeviceFarm 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/client.py` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,15 +746,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_projects)
         """
 
     def list_test_grid_session_actions(
         self, *, sessionArn: str, maxResult: int = ..., nextToken: str = ...
     ) -> ListTestGridSessionActionsResultTypeDef:
         """
-        Returns a list of the actions taken in a  TestGridSession .
+        Returns a list of the actions taken in a  TestGridSession.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_session_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_session_actions)
         """
 
     def list_test_grid_session_artifacts(
         self,
@@ -780,15 +780,15 @@
         creationTimeBefore: Union[datetime, str] = ...,
         endTimeAfter: Union[datetime, str] = ...,
         endTimeBefore: Union[datetime, str] = ...,
         maxResult: int = ...,
         nextToken: str = ...
     ) -> ListTestGridSessionsResultTypeDef:
         """
-        Retrieves a list of sessions for a  TestGridProject .
+        Retrieves a list of sessions for a  TestGridProject.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_sessions)
         """
 
     def list_tests(self, *, arn: str, nextToken: str = ...) -> ListTestsResultTypeDef:
         """
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/client.pyi` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_projects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_projects)
         """
     def list_test_grid_session_actions(
         self, *, sessionArn: str, maxResult: int = ..., nextToken: str = ...
     ) -> ListTestGridSessionActionsResultTypeDef:
         """
-        Returns a list of the actions taken in a  TestGridSession .
+        Returns a list of the actions taken in a  TestGridSession.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_session_actions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_session_actions)
         """
     def list_test_grid_session_artifacts(
         self,
         *,
@@ -716,15 +716,15 @@
         creationTimeBefore: Union[datetime, str] = ...,
         endTimeAfter: Union[datetime, str] = ...,
         endTimeBefore: Union[datetime, str] = ...,
         maxResult: int = ...,
         nextToken: str = ...
     ) -> ListTestGridSessionsResultTypeDef:
         """
-        Retrieves a list of sessions for a  TestGridProject .
+        Retrieves a list of sessions for a  TestGridProject.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_sessions)
         """
     def list_tests(self, *, arn: str, nextToken: str = ...) -> ListTestsResultTypeDef:
         """
         Gets information about tests in a given test suite.
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/literals.py` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,23 +286,25 @@
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
@@ -312,30 +314,35 @@
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
@@ -361,14 +368,15 @@
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
@@ -413,51 +421,57 @@
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
@@ -470,14 +484,15 @@
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
@@ -489,28 +504,35 @@
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
@@ -519,14 +541,15 @@
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
@@ -537,55 +560,64 @@
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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/literals.pyi` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -284,23 +284,25 @@
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
@@ -310,30 +312,35 @@
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
@@ -359,14 +366,15 @@
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
@@ -411,51 +419,57 @@
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
@@ -468,14 +482,15 @@
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
@@ -487,28 +502,35 @@
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
@@ -517,14 +539,15 @@
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
@@ -535,55 +558,64 @@
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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/paginator.py` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 class GetOfferingStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetOfferingStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
         """
 
 
@@ -148,30 +148,30 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: ArtifactCategoryType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listartifactspaginator)
         """
 
 
 class ListDeviceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
         """
 
 
@@ -182,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: DevicePoolTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicepoolspaginator)
         """
 
 
@@ -201,45 +201,45 @@
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
         filters: Sequence[DeviceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
 
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstanceProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
         """
 
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
         """
 
 
@@ -250,165 +250,165 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: NetworkProfileTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworkProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listnetworkprofilespaginator)
         """
 
 
 class ListOfferingPromotionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingPromotionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
         """
 
 
 class ListOfferingTransactionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingTransactionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
         """
 
 
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, arn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
         """
 
 
 class ListRemoteAccessSessionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRemoteAccessSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
         """
 
 
 class ListRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRunsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
         """
 
 
 class ListSamplesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSamplesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
         """
 
 
 class ListSuitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSuitesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
         """
 
 
 class ListTestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTestsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
         """
 
 
 class ListUniqueProblemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUniqueProblemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
         """
 
 
@@ -419,28 +419,28 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: UploadTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUploadsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuploadspaginator)
         """
 
 
 class ListVPCEConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVPCEConfigurationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/paginator.pyi` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 class GetOfferingStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetOfferingStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.GetOfferingStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#getofferingstatuspaginator)
         """
 
 class ListArtifactsPaginator(Paginator):
@@ -144,29 +144,29 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: ArtifactCategoryType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listartifactspaginator)
         """
 
 class ListDeviceInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDeviceInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdeviceinstancespaginator)
         """
 
 class ListDevicePoolsPaginator(Paginator):
@@ -176,15 +176,15 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: DevicePoolTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevicePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicepoolspaginator)
         """
 
 class ListDevicesPaginator(Paginator):
@@ -194,43 +194,43 @@
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
         filters: Sequence[DeviceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstanceProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listinstanceprofilespaginator)
         """
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listjobspaginator)
         """
 
 class ListNetworkProfilesPaginator(Paginator):
@@ -240,155 +240,155 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: NetworkProfileTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNetworkProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListNetworkProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listnetworkprofilespaginator)
         """
 
 class ListOfferingPromotionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingPromotionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingPromotions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingpromotionspaginator)
         """
 
 class ListOfferingTransactionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingTransactionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferingTransactions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingtransactionspaginator)
         """
 
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listofferingspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, arn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listprojectspaginator)
         """
 
 class ListRemoteAccessSessionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRemoteAccessSessionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRemoteAccessSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listremoteaccesssessionspaginator)
         """
 
 class ListRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRunsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listrunspaginator)
         """
 
 class ListSamplesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSamplesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSamples.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsamplespaginator)
         """
 
 class ListSuitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSuitesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListSuites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listsuitespaginator)
         """
 
 class ListTestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTestsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListTests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listtestspaginator)
         """
 
 class ListUniqueProblemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUniqueProblemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUniqueProblems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuniqueproblemspaginator)
         """
 
 class ListUploadsPaginator(Paginator):
@@ -398,27 +398,27 @@
     """
 
     def paginate(
         self,
         *,
         arn: str,
         type: UploadTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUploadsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listuploadspaginator)
         """
 
 class ListVPCEConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVPCEConfigurationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListVPCEConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listvpceconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/type_defs.py` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,23 @@
 
 __all__ = (
     "TrialMinutesTypeDef",
     "ArtifactTypeDef",
     "CPUTypeDef",
     "CountersTypeDef",
     "RuleTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "InstanceProfileTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "VpcConfigTypeDef",
     "CreateRemoteAccessSessionConfigurationTypeDef",
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
+    "CreateTestGridUrlResultTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
@@ -90,76 +90,95 @@
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
     "GetDevicePoolRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     "GetOfferingStatusRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetRemoteAccessSessionRequestRequestTypeDef",
     "GetRunRequestRequestTypeDef",
     "GetSuiteRequestRequestTypeDef",
     "GetTestGridProjectRequestRequestTypeDef",
     "GetTestGridSessionRequestRequestTypeDef",
     "TestGridSessionTypeDef",
     "GetTestRequestRequestTypeDef",
     "GetUploadRequestRequestTypeDef",
     "GetVPCEConfigurationRequestRequestTypeDef",
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
+    "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListArtifactsRequestRequestTypeDef",
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDeviceInstancesRequestRequestTypeDef",
+    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
     "ListDevicePoolsRequestRequestTypeDef",
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListNetworkProfilesRequestRequestTypeDef",
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingPromotionsRequestRequestTypeDef",
     "OfferingPromotionTypeDef",
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingTransactionsRequestRequestTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
+    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
     "ListRemoteAccessSessionsRequestRequestTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
+    "ListSamplesRequestListSamplesPaginateTypeDef",
     "ListSamplesRequestRequestTypeDef",
     "SampleTypeDef",
+    "ListSuitesRequestListSuitesPaginateTypeDef",
     "ListSuitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
+    "ListTestsRequestListTestsPaginateTypeDef",
     "ListTestsRequestRequestTypeDef",
+    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
+    "ListUploadsRequestListUploadsPaginateTypeDef",
     "ListUploadsRequestRequestTypeDef",
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
+    "PaginatorConfigTypeDef",
     "ProblemDetailTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
+    "ListArtifactsResultTypeDef",
     "CreateDevicePoolRequestRequestTypeDef",
     "DevicePoolTypeDef",
     "UpdateDevicePoolRequestRequestTypeDef",
-    "CreateTestGridUrlResultTypeDef",
-    "ListArtifactsResultTypeDef",
     "CreateInstanceProfileResultTypeDef",
     "DeviceInstanceTypeDef",
     "GetInstanceProfileResultTypeDef",
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
@@ -179,37 +198,18 @@
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
     "DeviceSelectionConfigurationTypeDef",
     "DeviceSelectionResultTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
-    "ListArtifactsRequestListArtifactsPaginateTypeDef",
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
-    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
-    "ListSamplesRequestListSamplesPaginateTypeDef",
-    "ListSuitesRequestListSuitesPaginateTypeDef",
-    "ListTestsRequestListTestsPaginateTypeDef",
-    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    "ListUploadsRequestListUploadsPaginateTypeDef",
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "GetTestGridSessionResultTypeDef",
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
@@ -321,25 +321,14 @@
         "attribute": DeviceAttributeType,
         "operator": RuleOperatorType,
         "value": str,
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
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -456,14 +445,23 @@
     "CreateTestGridUrlRequestRequestTypeDef",
     {
         "projectArn": str,
         "expiresInSeconds": int,
     },
 )
 
+CreateTestGridUrlResultTypeDef = TypedDict(
+    "CreateTestGridUrlResultTypeDef",
+    {
+        "url": str,
+        "expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUploadRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "type": UploadTypeType,
     },
@@ -718,20 +716,18 @@
 GetNetworkProfileRequestRequestTypeDef = TypedDict(
     "GetNetworkProfileRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetOfferingStatusRequestRequestTypeDef = TypedDict(
     "GetOfferingStatusRequestRequestTypeDef",
     {
@@ -823,14 +819,37 @@
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
     {
         "remoteAccessSessionArn": str,
         "appArn": str,
     },
 )
 
+_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
+    {
+        "arn": str,
+        "type": ArtifactCategoryType,
+    },
+)
+_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListArtifactsRequestListArtifactsPaginateTypeDef(
+    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
+    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListArtifactsRequestRequestTypeDef",
     {
         "arn": str,
         "type": ArtifactCategoryType,
     },
 )
@@ -845,23 +864,54 @@
 
 class ListArtifactsRequestRequestTypeDef(
     _RequiredListArtifactsRequestRequestTypeDef, _OptionalListArtifactsRequestRequestTypeDef
 ):
     pass
 
 
+ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeviceInstancesRequestRequestTypeDef = TypedDict(
     "ListDeviceInstancesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
+        "type": DevicePoolTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
+    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDevicePoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePoolsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListDevicePoolsRequestRequestTypeDef = TypedDict(
@@ -876,23 +926,52 @@
 
 class ListDevicePoolsRequestRequestTypeDef(
     _RequiredListDevicePoolsRequestRequestTypeDef, _OptionalListDevicePoolsRequestRequestTypeDef
 ):
     pass
 
 
+ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInstanceProfilesRequestRequestTypeDef = TypedDict(
     "ListInstanceProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsRequestListJobsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListJobsRequestListJobsPaginateTypeDef(
+    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
+):
+    pass
+
+
 _RequiredListJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListJobsRequestRequestTypeDef = TypedDict(
@@ -906,14 +985,37 @@
 
 class ListJobsRequestRequestTypeDef(
     _RequiredListJobsRequestRequestTypeDef, _OptionalListJobsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "type": NetworkProfileTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
+    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListNetworkProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkProfilesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListNetworkProfilesRequestRequestTypeDef = TypedDict(
@@ -929,14 +1031,22 @@
 class ListNetworkProfilesRequestRequestTypeDef(
     _RequiredListNetworkProfilesRequestRequestTypeDef,
     _OptionalListNetworkProfilesRequestRequestTypeDef,
 ):
     pass
 
 
+ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingPromotionsRequestRequestTypeDef = TypedDict(
     "ListOfferingPromotionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -946,39 +1056,86 @@
     {
         "id": str,
         "description": str,
     },
     total=False,
 )
 
+ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingTransactionsRequestRequestTypeDef = TypedDict(
     "ListOfferingTransactionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "arn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
+    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRemoteAccessSessionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
@@ -993,14 +1150,35 @@
 class ListRemoteAccessSessionsRequestRequestTypeDef(
     _RequiredListRemoteAccessSessionsRequestRequestTypeDef,
     _OptionalListRemoteAccessSessionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_RequiredListRunsRequestListRunsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_OptionalListRunsRequestListRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRunsRequestListRunsPaginateTypeDef(
+    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
+):
+    pass
+
+
 _RequiredListRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListRunsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRunsRequestRequestTypeDef = TypedDict(
@@ -1014,14 +1192,36 @@
 
 class ListRunsRequestRequestTypeDef(
     _RequiredListRunsRequestRequestTypeDef, _OptionalListRunsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSamplesRequestListSamplesPaginateTypeDef(
+    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
+    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSamplesRequestRequestTypeDef = TypedDict(
     "_RequiredListSamplesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSamplesRequestRequestTypeDef = TypedDict(
@@ -1045,14 +1245,36 @@
         "arn": str,
         "type": SampleTypeType,
         "url": str,
     },
     total=False,
 )
 
+_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSuitesRequestListSuitesPaginateTypeDef(
+    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
+    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSuitesRequestRequestTypeDef = TypedDict(
     "_RequiredListSuitesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSuitesRequestRequestTypeDef = TypedDict(
@@ -1187,14 +1409,36 @@
 class ListTestGridSessionsRequestRequestTypeDef(
     _RequiredListTestGridSessionsRequestRequestTypeDef,
     _OptionalListTestGridSessionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_RequiredListTestsRequestListTestsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_OptionalListTestsRequestListTestsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTestsRequestListTestsPaginateTypeDef(
+    _RequiredListTestsRequestListTestsPaginateTypeDef,
+    _OptionalListTestsRequestListTestsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTestsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListTestsRequestRequestTypeDef = TypedDict(
@@ -1208,14 +1452,36 @@
 
 class ListTestsRequestRequestTypeDef(
     _RequiredListTestsRequestRequestTypeDef, _OptionalListTestsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
+    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListUniqueProblemsRequestRequestTypeDef = TypedDict(
     "_RequiredListUniqueProblemsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUniqueProblemsRequestRequestTypeDef = TypedDict(
@@ -1230,14 +1496,37 @@
 class ListUniqueProblemsRequestRequestTypeDef(
     _RequiredListUniqueProblemsRequestRequestTypeDef,
     _OptionalListUniqueProblemsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "type": UploadTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUploadsRequestListUploadsPaginateTypeDef(
+    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
+    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListUploadsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUploadsRequestRequestTypeDef = TypedDict(
@@ -1252,14 +1541,22 @@
 
 class ListUploadsRequestRequestTypeDef(
     _RequiredListUploadsRequestRequestTypeDef, _OptionalListUploadsRequestRequestTypeDef
 ):
     pass
 
 
+ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVPCEConfigurationsRequestRequestTypeDef = TypedDict(
     "ListVPCEConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1278,14 +1575,24 @@
     {
         "amount": float,
         "currencyCode": Literal["USD"],
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
 ProblemDetailTypeDef = TypedDict(
     "ProblemDetailTypeDef",
     {
         "arn": str,
         "name": str,
     },
     total=False,
@@ -1328,14 +1635,25 @@
     "RenewOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
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
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -1501,14 +1819,23 @@
         "maxSlots": Dict[str, int],
         "defaultJobTimeoutMinutes": int,
         "skipAppResign": bool,
     },
     total=False,
 )
 
+ListArtifactsResultTypeDef = TypedDict(
+    "ListArtifactsResultTypeDef",
+    {
+        "artifacts": List[ArtifactTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevicePoolRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "rules": Sequence[RuleTypeDef],
     },
@@ -1563,37 +1890,19 @@
 
 class UpdateDevicePoolRequestRequestTypeDef(
     _RequiredUpdateDevicePoolRequestRequestTypeDef, _OptionalUpdateDevicePoolRequestRequestTypeDef
 ):
     pass
 
 
-CreateTestGridUrlResultTypeDef = TypedDict(
-    "CreateTestGridUrlResultTypeDef",
-    {
-        "url": str,
-        "expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListArtifactsResultTypeDef = TypedDict(
-    "ListArtifactsResultTypeDef",
-    {
-        "artifacts": List[ArtifactTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateInstanceProfileResultTypeDef = TypedDict(
     "CreateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceInstanceTypeDef = TypedDict(
     "DeviceInstanceTypeDef",
     {
         "arn": str,
@@ -1606,65 +1915,65 @@
     total=False,
 )
 
 GetInstanceProfileResultTypeDef = TypedDict(
     "GetInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstanceProfilesResultTypeDef = TypedDict(
     "ListInstanceProfilesResultTypeDef",
     {
         "instanceProfiles": List[InstanceProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceProfileResultTypeDef = TypedDict(
     "UpdateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNetworkProfileResultTypeDef = TypedDict(
     "CreateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkProfileResultTypeDef = TypedDict(
     "GetNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkProfilesResultTypeDef = TypedDict(
     "ListNetworkProfilesResultTypeDef",
     {
         "networkProfiles": List[NetworkProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNetworkProfileResultTypeDef = TypedDict(
     "UpdateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "name": str,
@@ -1812,81 +2121,81 @@
     pass
 
 
 CreateUploadResultTypeDef = TypedDict(
     "CreateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUploadResultTypeDef = TypedDict(
     "GetUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstallToRemoteAccessSessionResultTypeDef = TypedDict(
     "InstallToRemoteAccessSessionResultTypeDef",
     {
         "appUpload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUploadsResultTypeDef = TypedDict(
     "ListUploadsResultTypeDef",
     {
         "uploads": List[UploadTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUploadResultTypeDef = TypedDict(
     "UpdateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVPCEConfigurationResultTypeDef = TypedDict(
     "CreateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVPCEConfigurationResultTypeDef = TypedDict(
     "GetVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVPCEConfigurationsResultTypeDef = TypedDict(
     "ListVPCEConfigurationsResultTypeDef",
     {
         "vpceConfigurations": List[VPCEConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVPCEConfigurationResultTypeDef = TypedDict(
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceSelectionConfigurationTypeDef = TypedDict(
     "DeviceSelectionConfigurationTypeDef",
     {
         "filters": Sequence[DeviceFilterTypeDef],
@@ -1900,14 +2209,24 @@
         "filters": List[DeviceFilterTypeDef],
         "matchedDevicesCount": int,
         "maxDevices": int,
     },
     total=False,
 )
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
         "filters": Sequence[DeviceFilterTypeDef],
     },
@@ -1946,373 +2265,54 @@
         "counters": CountersTypeDef,
         "message": str,
         "deviceMinutes": DeviceMinutesTypeDef,
     },
     total=False,
 )
 
-GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "arn": str,
-        "type": ArtifactCategoryType,
-    },
-)
-_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListArtifactsRequestListArtifactsPaginateTypeDef(
-    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
-    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
-):
-    pass
-
-
-ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "type": DevicePoolTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
-    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-):
-    pass
-
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[DeviceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsRequestListJobsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListJobsRequestListJobsPaginateTypeDef(
-    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
-):
-    pass
-
-
-_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "type": NetworkProfileTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
-    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-):
-    pass
-
-
-ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "arn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
-    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_RequiredListRunsRequestListRunsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_OptionalListRunsRequestListRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRunsRequestListRunsPaginateTypeDef(
-    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
-):
-    pass
-
-
-_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSamplesRequestListSamplesPaginateTypeDef(
-    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
-    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSuitesRequestListSuitesPaginateTypeDef(
-    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
-    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_RequiredListTestsRequestListTestsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_OptionalListTestsRequestListTestsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTestsRequestListTestsPaginateTypeDef(
-    _RequiredListTestsRequestListTestsPaginateTypeDef,
-    _OptionalListTestsRequestListTestsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
-    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "type": UploadTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUploadsRequestListUploadsPaginateTypeDef(
-    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
-    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
-):
-    pass
-
-
-ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetTestGridSessionResultTypeDef = TypedDict(
     "GetTestGridSessionResultTypeDef",
     {
         "testGridSession": TestGridSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestGridSessionsResultTypeDef = TypedDict(
     "ListTestGridSessionsResultTypeDef",
     {
         "testGridSessions": List[TestGridSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingPromotionsResultTypeDef = TypedDict(
     "ListOfferingPromotionsResultTypeDef",
     {
         "offeringPromotions": List[OfferingPromotionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSamplesResultTypeDef = TypedDict(
     "ListSamplesResultTypeDef",
     {
         "samples": List[SampleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
@@ -2321,24 +2321,24 @@
 )
 
 ListTestGridSessionActionsResultTypeDef = TypedDict(
     "ListTestGridSessionActionsResultTypeDef",
     {
         "actions": List[TestGridSessionActionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestGridSessionArtifactsResultTypeDef = TypedDict(
     "ListTestGridSessionArtifactsResultTypeDef",
     {
         "artifacts": List[TestGridSessionArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "cost": MonetaryAmountTypeDef,
@@ -2363,48 +2363,48 @@
     total=False,
 )
 
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDevicePoolResultTypeDef = TypedDict(
     "CreateDevicePoolResultTypeDef",
     {
         "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevicePoolResultTypeDef = TypedDict(
     "GetDevicePoolResultTypeDef",
     {
         "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicePoolsResultTypeDef = TypedDict(
     "ListDevicePoolsResultTypeDef",
     {
         "devicePools": List[DevicePoolTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDevicePoolResultTypeDef = TypedDict(
     "UpdateDevicePoolResultTypeDef",
     {
         "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "arn": str,
@@ -2432,98 +2432,98 @@
     total=False,
 )
 
 GetDeviceInstanceResultTypeDef = TypedDict(
     "GetDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceInstancesResultTypeDef = TypedDict(
     "ListDeviceInstancesResultTypeDef",
     {
         "deviceInstances": List[DeviceInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDeviceInstanceResultTypeDef = TypedDict(
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProjectResultTypeDef = TypedDict(
     "CreateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProjectResultTypeDef = TypedDict(
     "GetProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectResultTypeDef = TypedDict(
     "UpdateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTestGridProjectResultTypeDef = TypedDict(
     "CreateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTestGridProjectResultTypeDef = TypedDict(
     "GetTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestGridProjectsResultTypeDef = TypedDict(
     "ListTestGridProjectsResultTypeDef",
     {
         "testGridProjects": List[TestGridProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTestGridProjectResultTypeDef = TypedDict(
     "UpdateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
@@ -2562,41 +2562,41 @@
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
         "suite": SuiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSuitesResultTypeDef = TypedDict(
     "ListSuitesResultTypeDef",
     {
         "suites": List[SuiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTestResultTypeDef = TypedDict(
     "GetTestResultTypeDef",
     {
         "test": TestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestsResultTypeDef = TypedDict(
     "ListTestsResultTypeDef",
     {
         "tests": List[TestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "id": str,
@@ -2670,15 +2670,15 @@
     total=False,
 )
 
 GetDeviceResultTypeDef = TypedDict(
     "GetDeviceResultTypeDef",
     {
         "device": DeviceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "arn": str,
@@ -2701,15 +2701,15 @@
 )
 
 ListDevicesResultTypeDef = TypedDict(
     "ListDevicesResultTypeDef",
     {
         "devices": List[DeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "run": ProblemDetailTypeDef,
@@ -2752,49 +2752,49 @@
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRunsResultTypeDef = TypedDict(
     "ListRunsResultTypeDef",
     {
         "runs": List[RunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduleRunResultTypeDef = TypedDict(
     "ScheduleRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRunResultTypeDef = TypedDict(
     "StopRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingsResultTypeDef = TypedDict(
     "ListOfferingsResultTypeDef",
     {
         "offerings": List[OfferingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingStatusTypeDef = TypedDict(
     "OfferingStatusTypeDef",
     {
         "type": OfferingTransactionTypeType,
@@ -2806,40 +2806,40 @@
 )
 
 GetDevicePoolCompatibilityResultTypeDef = TypedDict(
     "GetDevicePoolCompatibilityResultTypeDef",
     {
         "compatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
         "incompatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResultTypeDef = TypedDict(
     "GetJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "jobs": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopJobResultTypeDef = TypedDict(
     "StopJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UniqueProblemTypeDef = TypedDict(
     "UniqueProblemTypeDef",
     {
         "message": str,
@@ -2848,50 +2848,50 @@
     total=False,
 )
 
 CreateRemoteAccessSessionResultTypeDef = TypedDict(
     "CreateRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRemoteAccessSessionResultTypeDef = TypedDict(
     "GetRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRemoteAccessSessionsResultTypeDef = TypedDict(
     "ListRemoteAccessSessionsResultTypeDef",
     {
         "remoteAccessSessions": List[RemoteAccessSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRemoteAccessSessionResultTypeDef = TypedDict(
     "StopRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOfferingStatusResultTypeDef = TypedDict(
     "GetOfferingStatusResultTypeDef",
     {
         "current": Dict[str, OfferingStatusTypeDef],
         "nextPeriod": Dict[str, OfferingStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTransactionTypeDef = TypedDict(
     "OfferingTransactionTypeDef",
     {
         "offeringStatus": OfferingStatusTypeDef,
@@ -2904,35 +2904,35 @@
 )
 
 ListUniqueProblemsResultTypeDef = TypedDict(
     "ListUniqueProblemsResultTypeDef",
     {
         "uniqueProblems": Dict[ExecutionResultType, List[UniqueProblemTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingTransactionsResultTypeDef = TypedDict(
     "ListOfferingTransactionsResultTypeDef",
     {
         "offeringTransactions": List[OfferingTransactionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResultTypeDef = TypedDict(
     "PurchaseOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RenewOfferingResultTypeDef = TypedDict(
     "RenewOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm/type_defs.pyi` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
 __all__ = (
     "TrialMinutesTypeDef",
     "ArtifactTypeDef",
     "CPUTypeDef",
     "CountersTypeDef",
     "RuleTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "InstanceProfileTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "VpcConfigTypeDef",
     "CreateRemoteAccessSessionConfigurationTypeDef",
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
+    "CreateTestGridUrlResultTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
@@ -89,76 +89,95 @@
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
     "GetDevicePoolRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     "GetOfferingStatusRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetRemoteAccessSessionRequestRequestTypeDef",
     "GetRunRequestRequestTypeDef",
     "GetSuiteRequestRequestTypeDef",
     "GetTestGridProjectRequestRequestTypeDef",
     "GetTestGridSessionRequestRequestTypeDef",
     "TestGridSessionTypeDef",
     "GetTestRequestRequestTypeDef",
     "GetUploadRequestRequestTypeDef",
     "GetVPCEConfigurationRequestRequestTypeDef",
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
+    "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListArtifactsRequestRequestTypeDef",
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDeviceInstancesRequestRequestTypeDef",
+    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
     "ListDevicePoolsRequestRequestTypeDef",
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListNetworkProfilesRequestRequestTypeDef",
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingPromotionsRequestRequestTypeDef",
     "OfferingPromotionTypeDef",
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingTransactionsRequestRequestTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
+    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
     "ListRemoteAccessSessionsRequestRequestTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
+    "ListSamplesRequestListSamplesPaginateTypeDef",
     "ListSamplesRequestRequestTypeDef",
     "SampleTypeDef",
+    "ListSuitesRequestListSuitesPaginateTypeDef",
     "ListSuitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
+    "ListTestsRequestListTestsPaginateTypeDef",
     "ListTestsRequestRequestTypeDef",
+    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
+    "ListUploadsRequestListUploadsPaginateTypeDef",
     "ListUploadsRequestRequestTypeDef",
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
+    "PaginatorConfigTypeDef",
     "ProblemDetailTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
+    "ListArtifactsResultTypeDef",
     "CreateDevicePoolRequestRequestTypeDef",
     "DevicePoolTypeDef",
     "UpdateDevicePoolRequestRequestTypeDef",
-    "CreateTestGridUrlResultTypeDef",
-    "ListArtifactsResultTypeDef",
     "CreateInstanceProfileResultTypeDef",
     "DeviceInstanceTypeDef",
     "GetInstanceProfileResultTypeDef",
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
@@ -178,37 +197,18 @@
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
     "DeviceSelectionConfigurationTypeDef",
     "DeviceSelectionResultTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
-    "ListArtifactsRequestListArtifactsPaginateTypeDef",
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
-    "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
-    "ListSamplesRequestListSamplesPaginateTypeDef",
-    "ListSuitesRequestListSuitesPaginateTypeDef",
-    "ListTestsRequestListTestsPaginateTypeDef",
-    "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    "ListUploadsRequestListUploadsPaginateTypeDef",
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "GetTestGridSessionResultTypeDef",
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
@@ -320,25 +320,14 @@
         "attribute": DeviceAttributeType,
         "operator": RuleOperatorType,
         "value": str,
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
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -451,14 +440,23 @@
     "CreateTestGridUrlRequestRequestTypeDef",
     {
         "projectArn": str,
         "expiresInSeconds": int,
     },
 )
 
+CreateTestGridUrlResultTypeDef = TypedDict(
+    "CreateTestGridUrlResultTypeDef",
+    {
+        "url": str,
+        "expires": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUploadRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "type": UploadTypeType,
     },
@@ -707,20 +705,18 @@
 GetNetworkProfileRequestRequestTypeDef = TypedDict(
     "GetNetworkProfileRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
+    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetOfferingStatusRequestRequestTypeDef = TypedDict(
     "GetOfferingStatusRequestRequestTypeDef",
     {
@@ -812,14 +808,35 @@
     "InstallToRemoteAccessSessionRequestRequestTypeDef",
     {
         "remoteAccessSessionArn": str,
         "appArn": str,
     },
 )
 
+_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
+    {
+        "arn": str,
+        "type": ArtifactCategoryType,
+    },
+)
+_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListArtifactsRequestListArtifactsPaginateTypeDef(
+    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
+    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
+):
+    pass
+
 _RequiredListArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListArtifactsRequestRequestTypeDef",
     {
         "arn": str,
         "type": ArtifactCategoryType,
     },
 )
@@ -832,23 +849,52 @@
 )
 
 class ListArtifactsRequestRequestTypeDef(
     _RequiredListArtifactsRequestRequestTypeDef, _OptionalListArtifactsRequestRequestTypeDef
 ):
     pass
 
+ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
+    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeviceInstancesRequestRequestTypeDef = TypedDict(
     "ListDeviceInstancesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
+    {
+        "type": DevicePoolTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
+    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDevicePoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePoolsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListDevicePoolsRequestRequestTypeDef = TypedDict(
@@ -861,23 +907,50 @@
 )
 
 class ListDevicePoolsRequestRequestTypeDef(
     _RequiredListDevicePoolsRequestRequestTypeDef, _OptionalListDevicePoolsRequestRequestTypeDef
 ):
     pass
 
+ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInstanceProfilesRequestRequestTypeDef = TypedDict(
     "ListInstanceProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsRequestListJobsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListJobsRequestListJobsPaginateTypeDef(
+    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
+):
+    pass
+
 _RequiredListJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListJobsRequestRequestTypeDef = TypedDict(
@@ -889,14 +962,35 @@
 )
 
 class ListJobsRequestRequestTypeDef(
     _RequiredListJobsRequestRequestTypeDef, _OptionalListJobsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
+    {
+        "type": NetworkProfileTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
+    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
+):
+    pass
+
 _RequiredListNetworkProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListNetworkProfilesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListNetworkProfilesRequestRequestTypeDef = TypedDict(
@@ -910,14 +1004,22 @@
 
 class ListNetworkProfilesRequestRequestTypeDef(
     _RequiredListNetworkProfilesRequestRequestTypeDef,
     _OptionalListNetworkProfilesRequestRequestTypeDef,
 ):
     pass
 
+ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
+    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingPromotionsRequestRequestTypeDef = TypedDict(
     "ListOfferingPromotionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -927,39 +1029,84 @@
     {
         "id": str,
         "description": str,
     },
     total=False,
 )
 
+ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
+    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingTransactionsRequestRequestTypeDef = TypedDict(
     "ListOfferingTransactionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "arn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
+    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRemoteAccessSessionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRemoteAccessSessionsRequestRequestTypeDef = TypedDict(
@@ -972,14 +1119,33 @@
 
 class ListRemoteAccessSessionsRequestRequestTypeDef(
     _RequiredListRemoteAccessSessionsRequestRequestTypeDef,
     _OptionalListRemoteAccessSessionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_RequiredListRunsRequestListRunsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "_OptionalListRunsRequestListRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRunsRequestListRunsPaginateTypeDef(
+    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
+):
+    pass
+
 _RequiredListRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListRunsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListRunsRequestRequestTypeDef = TypedDict(
@@ -991,14 +1157,34 @@
 )
 
 class ListRunsRequestRequestTypeDef(
     _RequiredListRunsRequestRequestTypeDef, _OptionalListRunsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
+    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSamplesRequestListSamplesPaginateTypeDef(
+    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
+    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
+):
+    pass
+
 _RequiredListSamplesRequestRequestTypeDef = TypedDict(
     "_RequiredListSamplesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSamplesRequestRequestTypeDef = TypedDict(
@@ -1020,14 +1206,34 @@
         "arn": str,
         "type": SampleTypeType,
         "url": str,
     },
     total=False,
 )
 
+_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
+    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSuitesRequestListSuitesPaginateTypeDef(
+    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
+    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
+):
+    pass
+
 _RequiredListSuitesRequestRequestTypeDef = TypedDict(
     "_RequiredListSuitesRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListSuitesRequestRequestTypeDef = TypedDict(
@@ -1154,14 +1360,34 @@
 
 class ListTestGridSessionsRequestRequestTypeDef(
     _RequiredListTestGridSessionsRequestRequestTypeDef,
     _OptionalListTestGridSessionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_RequiredListTestsRequestListTestsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
+    "_OptionalListTestsRequestListTestsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTestsRequestListTestsPaginateTypeDef(
+    _RequiredListTestsRequestListTestsPaginateTypeDef,
+    _OptionalListTestsRequestListTestsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTestsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListTestsRequestRequestTypeDef = TypedDict(
@@ -1173,14 +1399,34 @@
 )
 
 class ListTestsRequestRequestTypeDef(
     _RequiredListTestsRequestRequestTypeDef, _OptionalListTestsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
+    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
+    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
+):
+    pass
+
 _RequiredListUniqueProblemsRequestRequestTypeDef = TypedDict(
     "_RequiredListUniqueProblemsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUniqueProblemsRequestRequestTypeDef = TypedDict(
@@ -1193,14 +1439,35 @@
 
 class ListUniqueProblemsRequestRequestTypeDef(
     _RequiredListUniqueProblemsRequestRequestTypeDef,
     _OptionalListUniqueProblemsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
+    {
+        "type": UploadTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUploadsRequestListUploadsPaginateTypeDef(
+    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
+    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
+):
+    pass
+
 _RequiredListUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListUploadsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListUploadsRequestRequestTypeDef = TypedDict(
@@ -1213,14 +1480,22 @@
 )
 
 class ListUploadsRequestRequestTypeDef(
     _RequiredListUploadsRequestRequestTypeDef, _OptionalListUploadsRequestRequestTypeDef
 ):
     pass
 
+ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
+    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVPCEConfigurationsRequestRequestTypeDef = TypedDict(
     "ListVPCEConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1239,14 +1514,24 @@
     {
         "amount": float,
         "currencyCode": Literal["USD"],
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
 ProblemDetailTypeDef = TypedDict(
     "ProblemDetailTypeDef",
     {
         "arn": str,
         "name": str,
     },
     total=False,
@@ -1287,14 +1572,25 @@
     "RenewOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
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
 StopJobRequestRequestTypeDef = TypedDict(
     "StopJobRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -1450,14 +1746,23 @@
         "maxSlots": Dict[str, int],
         "defaultJobTimeoutMinutes": int,
         "skipAppResign": bool,
     },
     total=False,
 )
 
+ListArtifactsResultTypeDef = TypedDict(
+    "ListArtifactsResultTypeDef",
+    {
+        "artifacts": List[ArtifactTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevicePoolRequestRequestTypeDef",
     {
         "projectArn": str,
         "name": str,
         "rules": Sequence[RuleTypeDef],
     },
@@ -1508,37 +1813,19 @@
 )
 
 class UpdateDevicePoolRequestRequestTypeDef(
     _RequiredUpdateDevicePoolRequestRequestTypeDef, _OptionalUpdateDevicePoolRequestRequestTypeDef
 ):
     pass
 
-CreateTestGridUrlResultTypeDef = TypedDict(
-    "CreateTestGridUrlResultTypeDef",
-    {
-        "url": str,
-        "expires": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListArtifactsResultTypeDef = TypedDict(
-    "ListArtifactsResultTypeDef",
-    {
-        "artifacts": List[ArtifactTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateInstanceProfileResultTypeDef = TypedDict(
     "CreateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceInstanceTypeDef = TypedDict(
     "DeviceInstanceTypeDef",
     {
         "arn": str,
@@ -1551,65 +1838,65 @@
     total=False,
 )
 
 GetInstanceProfileResultTypeDef = TypedDict(
     "GetInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInstanceProfilesResultTypeDef = TypedDict(
     "ListInstanceProfilesResultTypeDef",
     {
         "instanceProfiles": List[InstanceProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceProfileResultTypeDef = TypedDict(
     "UpdateInstanceProfileResultTypeDef",
     {
         "instanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateNetworkProfileResultTypeDef = TypedDict(
     "CreateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkProfileResultTypeDef = TypedDict(
     "GetNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkProfilesResultTypeDef = TypedDict(
     "ListNetworkProfilesResultTypeDef",
     {
         "networkProfiles": List[NetworkProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNetworkProfileResultTypeDef = TypedDict(
     "UpdateNetworkProfileResultTypeDef",
     {
         "networkProfile": NetworkProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "name": str,
@@ -1747,81 +2034,81 @@
 ):
     pass
 
 CreateUploadResultTypeDef = TypedDict(
     "CreateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUploadResultTypeDef = TypedDict(
     "GetUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstallToRemoteAccessSessionResultTypeDef = TypedDict(
     "InstallToRemoteAccessSessionResultTypeDef",
     {
         "appUpload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUploadsResultTypeDef = TypedDict(
     "ListUploadsResultTypeDef",
     {
         "uploads": List[UploadTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUploadResultTypeDef = TypedDict(
     "UpdateUploadResultTypeDef",
     {
         "upload": UploadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVPCEConfigurationResultTypeDef = TypedDict(
     "CreateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVPCEConfigurationResultTypeDef = TypedDict(
     "GetVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVPCEConfigurationsResultTypeDef = TypedDict(
     "ListVPCEConfigurationsResultTypeDef",
     {
         "vpceConfigurations": List[VPCEConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVPCEConfigurationResultTypeDef = TypedDict(
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceSelectionConfigurationTypeDef = TypedDict(
     "DeviceSelectionConfigurationTypeDef",
     {
         "filters": Sequence[DeviceFilterTypeDef],
@@ -1835,14 +2122,24 @@
         "filters": List[DeviceFilterTypeDef],
         "matchedDevicesCount": int,
         "maxDevices": int,
     },
     total=False,
 )
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
         "filters": Sequence[DeviceFilterTypeDef],
     },
@@ -1881,351 +2178,54 @@
         "counters": CountersTypeDef,
         "message": str,
         "deviceMinutes": DeviceMinutesTypeDef,
     },
     total=False,
 )
 
-GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef = TypedDict(
-    "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "arn": str,
-        "type": ArtifactCategoryType,
-    },
-)
-_OptionalListArtifactsRequestListArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListArtifactsRequestListArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListArtifactsRequestListArtifactsPaginateTypeDef(
-    _RequiredListArtifactsRequestListArtifactsPaginateTypeDef,
-    _OptionalListArtifactsRequestListArtifactsPaginateTypeDef,
-):
-    pass
-
-ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef = TypedDict(
-    "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    {
-        "type": DevicePoolTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
-    _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-):
-    pass
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[DeviceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsRequestListJobsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListJobsRequestListJobsPaginateTypeDef(
-    _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
-):
-    pass
-
-_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
-    {
-        "type": NetworkProfileTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef(
-    _RequiredListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    _OptionalListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-):
-    pass
-
-ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef = TypedDict(
-    "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef = TypedDict(
-    "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "arn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef(
-    _RequiredListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    _OptionalListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_RequiredListRunsRequestListRunsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "_OptionalListRunsRequestListRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRunsRequestListRunsPaginateTypeDef(
-    _RequiredListRunsRequestListRunsPaginateTypeDef, _OptionalListRunsRequestListRunsPaginateTypeDef
-):
-    pass
-
-_RequiredListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_RequiredListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSamplesRequestListSamplesPaginateTypeDef = TypedDict(
-    "_OptionalListSamplesRequestListSamplesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSamplesRequestListSamplesPaginateTypeDef(
-    _RequiredListSamplesRequestListSamplesPaginateTypeDef,
-    _OptionalListSamplesRequestListSamplesPaginateTypeDef,
-):
-    pass
-
-_RequiredListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_RequiredListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListSuitesRequestListSuitesPaginateTypeDef = TypedDict(
-    "_OptionalListSuitesRequestListSuitesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSuitesRequestListSuitesPaginateTypeDef(
-    _RequiredListSuitesRequestListSuitesPaginateTypeDef,
-    _OptionalListSuitesRequestListSuitesPaginateTypeDef,
-):
-    pass
-
-_RequiredListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_RequiredListTestsRequestListTestsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListTestsRequestListTestsPaginateTypeDef = TypedDict(
-    "_OptionalListTestsRequestListTestsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTestsRequestListTestsPaginateTypeDef(
-    _RequiredListTestsRequestListTestsPaginateTypeDef,
-    _OptionalListTestsRequestListTestsPaginateTypeDef,
-):
-    pass
-
-_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef = TypedDict(
-    "_OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef(
-    _RequiredListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    _OptionalListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-):
-    pass
-
-_RequiredListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListUploadsRequestListUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListUploadsRequestListUploadsPaginateTypeDef",
-    {
-        "type": UploadTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUploadsRequestListUploadsPaginateTypeDef(
-    _RequiredListUploadsRequestListUploadsPaginateTypeDef,
-    _OptionalListUploadsRequestListUploadsPaginateTypeDef,
-):
-    pass
-
-ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef = TypedDict(
-    "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetTestGridSessionResultTypeDef = TypedDict(
     "GetTestGridSessionResultTypeDef",
     {
         "testGridSession": TestGridSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestGridSessionsResultTypeDef = TypedDict(
     "ListTestGridSessionsResultTypeDef",
     {
         "testGridSessions": List[TestGridSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingPromotionsResultTypeDef = TypedDict(
     "ListOfferingPromotionsResultTypeDef",
     {
         "offeringPromotions": List[OfferingPromotionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSamplesResultTypeDef = TypedDict(
     "ListSamplesResultTypeDef",
     {
         "samples": List[SampleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
@@ -2234,24 +2234,24 @@
 )
 
 ListTestGridSessionActionsResultTypeDef = TypedDict(
     "ListTestGridSessionActionsResultTypeDef",
     {
         "actions": List[TestGridSessionActionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestGridSessionArtifactsResultTypeDef = TypedDict(
     "ListTestGridSessionArtifactsResultTypeDef",
     {
         "artifacts": List[TestGridSessionArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "cost": MonetaryAmountTypeDef,
@@ -2276,48 +2276,48 @@
     total=False,
 )
 
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDevicePoolResultTypeDef = TypedDict(
     "CreateDevicePoolResultTypeDef",
     {
         "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevicePoolResultTypeDef = TypedDict(
     "GetDevicePoolResultTypeDef",
     {
         "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicePoolsResultTypeDef = TypedDict(
     "ListDevicePoolsResultTypeDef",
     {
         "devicePools": List[DevicePoolTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDevicePoolResultTypeDef = TypedDict(
     "UpdateDevicePoolResultTypeDef",
     {
         "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "arn": str,
@@ -2345,98 +2345,98 @@
     total=False,
 )
 
 GetDeviceInstanceResultTypeDef = TypedDict(
     "GetDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceInstancesResultTypeDef = TypedDict(
     "ListDeviceInstancesResultTypeDef",
     {
         "deviceInstances": List[DeviceInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDeviceInstanceResultTypeDef = TypedDict(
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProjectResultTypeDef = TypedDict(
     "CreateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProjectResultTypeDef = TypedDict(
     "GetProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectResultTypeDef = TypedDict(
     "UpdateProjectResultTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTestGridProjectResultTypeDef = TypedDict(
     "CreateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTestGridProjectResultTypeDef = TypedDict(
     "GetTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestGridProjectsResultTypeDef = TypedDict(
     "ListTestGridProjectsResultTypeDef",
     {
         "testGridProjects": List[TestGridProjectTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTestGridProjectResultTypeDef = TypedDict(
     "UpdateTestGridProjectResultTypeDef",
     {
         "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
@@ -2475,41 +2475,41 @@
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
         "suite": SuiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSuitesResultTypeDef = TypedDict(
     "ListSuitesResultTypeDef",
     {
         "suites": List[SuiteTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTestResultTypeDef = TypedDict(
     "GetTestResultTypeDef",
     {
         "test": TestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestsResultTypeDef = TypedDict(
     "ListTestsResultTypeDef",
     {
         "tests": List[TestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "id": str,
@@ -2579,15 +2579,15 @@
     total=False,
 )
 
 GetDeviceResultTypeDef = TypedDict(
     "GetDeviceResultTypeDef",
     {
         "device": DeviceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "arn": str,
@@ -2610,15 +2610,15 @@
 )
 
 ListDevicesResultTypeDef = TypedDict(
     "ListDevicesResultTypeDef",
     {
         "devices": List[DeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProblemTypeDef = TypedDict(
     "ProblemTypeDef",
     {
         "run": ProblemDetailTypeDef,
@@ -2661,49 +2661,49 @@
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRunsResultTypeDef = TypedDict(
     "ListRunsResultTypeDef",
     {
         "runs": List[RunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduleRunResultTypeDef = TypedDict(
     "ScheduleRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRunResultTypeDef = TypedDict(
     "StopRunResultTypeDef",
     {
         "run": RunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingsResultTypeDef = TypedDict(
     "ListOfferingsResultTypeDef",
     {
         "offerings": List[OfferingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingStatusTypeDef = TypedDict(
     "OfferingStatusTypeDef",
     {
         "type": OfferingTransactionTypeType,
@@ -2715,40 +2715,40 @@
 )
 
 GetDevicePoolCompatibilityResultTypeDef = TypedDict(
     "GetDevicePoolCompatibilityResultTypeDef",
     {
         "compatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
         "incompatibleDevices": List[DevicePoolCompatibilityResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResultTypeDef = TypedDict(
     "GetJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "jobs": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopJobResultTypeDef = TypedDict(
     "StopJobResultTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UniqueProblemTypeDef = TypedDict(
     "UniqueProblemTypeDef",
     {
         "message": str,
@@ -2757,50 +2757,50 @@
     total=False,
 )
 
 CreateRemoteAccessSessionResultTypeDef = TypedDict(
     "CreateRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRemoteAccessSessionResultTypeDef = TypedDict(
     "GetRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRemoteAccessSessionsResultTypeDef = TypedDict(
     "ListRemoteAccessSessionsResultTypeDef",
     {
         "remoteAccessSessions": List[RemoteAccessSessionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopRemoteAccessSessionResultTypeDef = TypedDict(
     "StopRemoteAccessSessionResultTypeDef",
     {
         "remoteAccessSession": RemoteAccessSessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOfferingStatusResultTypeDef = TypedDict(
     "GetOfferingStatusResultTypeDef",
     {
         "current": Dict[str, OfferingStatusTypeDef],
         "nextPeriod": Dict[str, OfferingStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTransactionTypeDef = TypedDict(
     "OfferingTransactionTypeDef",
     {
         "offeringStatus": OfferingStatusTypeDef,
@@ -2813,35 +2813,35 @@
 )
 
 ListUniqueProblemsResultTypeDef = TypedDict(
     "ListUniqueProblemsResultTypeDef",
     {
         "uniqueProblems": Dict[ExecutionResultType, List[UniqueProblemTypeDef]],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOfferingTransactionsResultTypeDef = TypedDict(
     "ListOfferingTransactionsResultTypeDef",
     {
         "offeringTransactions": List[OfferingTransactionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResultTypeDef = TypedDict(
     "PurchaseOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RenewOfferingResultTypeDef = TypedDict(
     "RenewOfferingResultTypeDef",
     {
         "offeringTransaction": OfferingTransactionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/PKG-INFO` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DeviceFarm 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.DeviceFarm 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
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
 
 <a id="mypy-boto3-devicefarm"></a>
 
 # mypy-boto3-devicefarm
 
 [![PyPI - mypy-boto3-devicefarm](https://img.shields.io/pypi/v/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devicefarm?color=blue)](https://pypistats.org/packages/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -427,23 +428,23 @@
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
     RuleTypeDef,
-    ResponseMetadataTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     InstanceProfileTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     VpcConfigTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
+    CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
@@ -462,76 +463,95 @@
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
     GetOfferingStatusRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetRemoteAccessSessionRequestRequestTypeDef,
     GetRunRequestRequestTypeDef,
     GetSuiteRequestRequestTypeDef,
     GetTestGridProjectRequestRequestTypeDef,
     GetTestGridSessionRequestRequestTypeDef,
     TestGridSessionTypeDef,
     GetTestRequestRequestTypeDef,
     GetUploadRequestRequestTypeDef,
     GetVPCEConfigurationRequestRequestTypeDef,
     InstallToRemoteAccessSessionRequestRequestTypeDef,
+    ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListArtifactsRequestRequestTypeDef,
+    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDeviceInstancesRequestRequestTypeDef,
+    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     ListDevicePoolsRequestRequestTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListNetworkProfilesRequestRequestTypeDef,
+    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingPromotionsRequestRequestTypeDef,
     OfferingPromotionTypeDef,
+    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingTransactionsRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
+    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
     ListRemoteAccessSessionsRequestRequestTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
+    ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
+    ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
+    ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
+    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
+    ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
+    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
+    PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
+    ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
     DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
-    CreateTestGridUrlResultTypeDef,
-    ListArtifactsResultTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
@@ -551,37 +571,18 @@
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionConfigurationTypeDef,
     DeviceSelectionResultTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
-    GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
-    ListArtifactsRequestListArtifactsPaginateTypeDef,
-    ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
-    ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
-    ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
-    ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListRemoteAccessSessionsRequestListRemoteAccessSessionsPaginateTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
-    ListSamplesRequestListSamplesPaginateTypeDef,
-    ListSuitesRequestListSuitesPaginateTypeDef,
-    ListTestsRequestListTestsPaginateTypeDef,
-    ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
-    ListUploadsRequestListUploadsPaginateTypeDef,
-    ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
@@ -650,42 +651,42 @@
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

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/mypy_boto3_devicefarm.egg-info/SOURCES.txt` & `mypy-boto3-devicefarm-1.27.0/mypy_boto3_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.26.0.post1/setup.py` & `mypy-boto3-devicefarm-1.27.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-devicefarm.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devicefarm",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DeviceFarm 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.DeviceFarm 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 devicefarm type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_devicefarm": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_devicefarm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/",
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


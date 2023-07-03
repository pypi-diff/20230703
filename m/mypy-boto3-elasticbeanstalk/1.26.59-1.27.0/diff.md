# Comparing `tmp/mypy-boto3-elasticbeanstalk-1.26.59.tar.gz` & `tmp/mypy-boto3-elasticbeanstalk-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.27.0.tar", last modified: Mon Jul  3 19:50:43 2023, max compression
```

## Comparing `mypy-boto3-elasticbeanstalk-1.26.59.tar` & `mypy-boto3-elasticbeanstalk-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.568096 mypy-boto3-elasticbeanstalk-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-01-27 20:32:50.568096 mypy-boto3-elasticbeanstalk-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.568096 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42742 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42680 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52788 2023-01-27 20:32:05.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52749 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-01-27 20:32:04.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.568096 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-01-27 20:32:50.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-27 20:32:50.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 20:32:50.000000 mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.568096 mypy-boto3-elasticbeanstalk-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-01-27 20:32:03.000000 mypy-boto3-elasticbeanstalk-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.491197 mypy-boto3-elasticbeanstalk-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21444 2023-07-03 19:50:43.491197 mypy-boto3-elasticbeanstalk-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.483197 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42742 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42680 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-07-03 19:37:17.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-07-03 19:37:17.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52858 2023-07-03 19:37:19.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52819 2023-07-03 19:37:17.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.491197 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21444 2023-07-03 19:50:43.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:50:43.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:43.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:43.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:50:43.000000 mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:43.491197 mypy-boto3-elasticbeanstalk-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 19:37:16.000000 mypy-boto3-elasticbeanstalk-1.27.0/setup.py
```

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/LICENSE` & `mypy-boto3-elasticbeanstalk-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.26.59
-Summary: Type annotations for boto3.ElasticBeanstalk 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticBeanstalk 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-elasticbeanstalk"></a>
 
 # mypy-boto3-elasticbeanstalk
 
 [![PyPI - mypy-boto3-elasticbeanstalk](https://img.shields.io/pypi/v/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticbeanstalk?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,61 +395,67 @@
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
     S3LocationTypeDef,
     SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
@@ -457,29 +463,27 @@
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
+    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
+    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
-    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
     ConfigurationSettingsDescriptionResponseMetadataTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
@@ -493,18 +497,14 @@
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
@@ -548,42 +548,42 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/README.md` & `mypy-boto3-elasticbeanstalk-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elasticbeanstalk"></a>
 
 # mypy-boto3-elasticbeanstalk
 
 [![PyPI - mypy-boto3-elasticbeanstalk](https://img.shields.io/pypi/v/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticbeanstalk?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,61 +363,67 @@
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
     S3LocationTypeDef,
     SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
@@ -425,29 +431,27 @@
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
+    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
+    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
-    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
     ConfigurationSettingsDescriptionResponseMetadataTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
@@ -461,18 +465,14 @@
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
@@ -516,42 +516,42 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/__init__.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/__init__.pyi` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/__main__.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticBeanstalk 1.26.59\nVersion:         1.26.59\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ElasticBeanstalk 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/client.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/client.pyi` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/literals.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionHistoryStatusType",
     "ActionStatusType",
     "ActionTypeType",
     "ApplicationVersionStatusType",
     "ComputeTypeType",
     "ConfigurationDeploymentStatusType",
@@ -51,15 +50,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionHistoryStatusType = Literal["Completed", "Failed", "Unknown"]
 ActionStatusType = Literal["Pending", "Running", "Scheduled", "Unknown"]
 ActionTypeType = Literal["InstanceRefresh", "PlatformUpdate", "Unknown"]
 ApplicationVersionStatusType = Literal[
     "Building", "Failed", "Processed", "Processing", "Unprocessed"
 ]
 ComputeTypeType = Literal["BUILD_GENERAL1_LARGE", "BUILD_GENERAL1_MEDIUM", "BUILD_GENERAL1_SMALL"]
@@ -139,14 +137,15 @@
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
@@ -178,21 +177,23 @@
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
@@ -271,14 +272,15 @@
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
@@ -289,14 +291,15 @@
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
@@ -332,14 +335,15 @@
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
@@ -358,16 +362,19 @@
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
@@ -447,18 +454,21 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/literals.pyi` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/literals.py`

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
     "ActionHistoryStatusType",
     "ActionStatusType",
     "ActionTypeType",
     "ApplicationVersionStatusType",
     "ComputeTypeType",
     "ConfigurationDeploymentStatusType",
@@ -50,14 +51,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ActionHistoryStatusType = Literal["Completed", "Failed", "Unknown"]
 ActionStatusType = Literal["Pending", "Running", "Scheduled", "Unknown"]
 ActionTypeType = Literal["InstanceRefresh", "PlatformUpdate", "Unknown"]
 ApplicationVersionStatusType = Literal[
     "Building", "Failed", "Processed", "Processing", "Unprocessed"
 ]
 ComputeTypeType = Literal["BUILD_GENERAL1_LARGE", "BUILD_GENERAL1_MEDIUM", "BUILD_GENERAL1_SMALL"]
@@ -137,14 +139,15 @@
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
@@ -176,21 +179,23 @@
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
@@ -269,14 +274,15 @@
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
@@ -287,14 +293,15 @@
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
@@ -330,14 +337,15 @@
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
@@ -356,16 +364,19 @@
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
@@ -445,18 +456,21 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/paginator.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
 
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
 
@@ -111,15 +111,15 @@
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
 
@@ -138,15 +138,15 @@
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
 
@@ -156,13 +156,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/paginator.pyi` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
 class DescribeEnvironmentManagedActionHistoryPaginator(Paginator):
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
 class DescribeEnvironmentsPaginator(Paginator):
@@ -106,15 +106,15 @@
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
         IncludedDeletedBackTo: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -132,15 +132,15 @@
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
 class ListPlatformVersionsPaginator(Paginator):
@@ -149,13 +149,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/type_defs.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,61 +41,67 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
     "S3LocationTypeDef",
     "SourceBuildInformationTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
+    "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
+    "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
+    "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
     "DeleteApplicationVersionMessageRequestTypeDef",
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     "DeleteEnvironmentConfigurationMessageRequestTypeDef",
     "DeletePlatformVersionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
     "DescribeApplicationVersionsMessageRequestTypeDef",
     "DescribeApplicationsMessageRequestTypeDef",
     "DescribeConfigurationSettingsMessageRequestTypeDef",
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEnvironmentsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
@@ -103,29 +109,27 @@
     "EventDescriptionTypeDef",
     "SolutionStackDescriptionTypeDef",
     "SearchFilterTypeDef",
     "PlatformBranchSummaryTypeDef",
     "PlatformFilterTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ListenerTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
+    "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    "CreateStorageLocationResultMessageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
     "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
@@ -139,18 +143,14 @@
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
@@ -191,25 +191,14 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
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
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "P999": float,
         "P99": float,
         "P95": float,
         "P90": float,
@@ -309,14 +298,25 @@
 class ApplyEnvironmentManagedActionRequestRequestTypeDef(
     _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef,
     _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef,
 ):
     pass
 
 
+ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    {
+        "ActionId": str,
+        "ActionDescription": str,
+        "ActionType": ActionTypeType,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
         "OperationsRole": str,
     },
 )
@@ -379,14 +379,23 @@
 CheckDNSAvailabilityMessageRequestTypeDef = TypedDict(
     "CheckDNSAvailabilityMessageRequestTypeDef",
     {
         "CNAMEPrefix": str,
     },
 )
 
+CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    {
+        "Available": bool,
+        "FullyQualifiedCNAME": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ComposeEnvironmentsMessageRequestTypeDef = TypedDict(
     "ComposeEnvironmentsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "GroupName": str,
         "VersionLabels": Sequence[str],
     },
@@ -477,14 +486,22 @@
         "PlatformVersion": str,
         "PlatformBranchName": str,
         "PlatformBranchLifecycleState": str,
     },
     total=False,
 )
 
+CreateStorageLocationResultMessageTypeDef = TypedDict(
+    "CreateStorageLocationResultMessageTypeDef",
+    {
+        "S3Bucket": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomAmiTypeDef = TypedDict(
     "CustomAmiTypeDef",
     {
         "VirtualizationType": str,
         "ImageId": str,
     },
     total=False,
@@ -565,20 +582,20 @@
         "DeploymentId": int,
         "Status": str,
         "DeploymentTime": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ApplicationName": str,
+        "VersionLabels": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeApplicationVersionsMessageRequestTypeDef = TypedDict(
     "DescribeApplicationVersionsMessageRequestTypeDef",
     {
@@ -642,14 +659,24 @@
         "Warning": int,
         "Degraded": int,
         "Severe": int,
     },
     total=False,
 )
 
+DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    {
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
         "NextToken": str,
         "MaxItems": int,
@@ -699,14 +726,28 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -723,14 +764,32 @@
         "IncludedDeletedBackTo": Union[datetime, str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "TemplateName": str,
         "EnvironmentId": str,
@@ -768,14 +827,21 @@
 DisassociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnvironmentLinkTypeDef = TypedDict(
     "EnvironmentLinkTypeDef",
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -910,14 +976,24 @@
     {
         "Protocol": str,
         "Port": int,
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
 PlatformFrameworkTypeDef = TypedDict(
     "PlatformFrameworkTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -968,14 +1044,25 @@
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
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
 RestartAppServerMessageRequestTypeDef = TypedDict(
     "RestartAppServerMessageRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -1066,49 +1153,14 @@
 class UpdateApplicationVersionMessageRequestTypeDef(
     _RequiredUpdateApplicationVersionMessageRequestTypeDef,
     _OptionalUpdateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
 
-ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    {
-        "ActionId": str,
-        "ActionDescription": str,
-        "ActionType": ActionTypeType,
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    {
-        "Available": bool,
-        "FullyQualifiedCNAME": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStorageLocationResultMessageTypeDef = TypedDict(
-    "CreateStorageLocationResultMessageTypeDef",
-    {
-        "S3Bucket": str,
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
 ApplicationMetricsTypeDef = TypedDict(
     "ApplicationMetricsTypeDef",
     {
         "Duration": int,
         "RequestCount": int,
         "StatusCodes": StatusCodesTypeDef,
         "Latency": LatencyTypeDef,
@@ -1178,15 +1230,15 @@
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "OptionSettings": List[ConfigurationOptionSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
         "SolutionStackName": str,
@@ -1227,15 +1279,15 @@
     pass
 
 
 ConfigurationSettingsValidationMessagesTypeDef = TypedDict(
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1291,15 +1343,15 @@
 
 
 ResourceTagsDescriptionMessageTypeDef = TypedDict(
     "ResourceTagsDescriptionMessageTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1442,101 +1494,49 @@
 )
 
 CreatePlatformVersionResultTypeDef = TypedDict(
     "CreatePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
         "Builder": BuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePlatformVersionResultTypeDef = TypedDict(
     "DeletePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformVersionsResultTypeDef = TypedDict(
     "ListPlatformVersionsResultTypeDef",
     {
         "PlatformSummaryList": List[PlatformSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabels": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    {
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     {
         "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionsResultTypeDef",
     {
         "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
@@ -1584,15 +1584,15 @@
     total=False,
 )
 
 RetrieveEnvironmentInfoResultMessageTypeDef = TypedDict(
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     {
         "EnvironmentInfo": List[EnvironmentInfoDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentResourceDescriptionTypeDef = TypedDict(
     "EnvironmentResourceDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1608,24 +1608,24 @@
 )
 
 EventDescriptionsMessageTypeDef = TypedDict(
     "EventDescriptionsMessageTypeDef",
     {
         "Events": List[EventDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableSolutionStacksResultMessageTypeDef = TypedDict(
     "ListAvailableSolutionStacksResultMessageTypeDef",
     {
         "SolutionStacks": List[str],
         "SolutionStackDetails": List[SolutionStackDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformBranchesRequestRequestTypeDef = TypedDict(
     "ListPlatformBranchesRequestRequestTypeDef",
     {
         "Filters": Sequence[SearchFilterTypeDef],
@@ -1636,23 +1636,23 @@
 )
 
 ListPlatformBranchesResultTypeDef = TypedDict(
     "ListPlatformBranchesResultTypeDef",
     {
         "PlatformBranchSummaryList": List[PlatformBranchSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = TypedDict(
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     {
         "Filters": Sequence[PlatformFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPlatformVersionsRequestRequestTypeDef = TypedDict(
     "ListPlatformVersionsRequestRequestTypeDef",
     {
@@ -1720,32 +1720,32 @@
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
         "Causes": List[str],
         "ApplicationMetrics": ApplicationMetricsTypeDef,
         "InstancesHealth": InstanceHealthSummaryTypeDef,
         "RefreshedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationVersionDescriptionMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionMessageTypeDef",
     {
         "ApplicationVersion": ApplicationVersionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationVersionDescriptionsMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionsMessageTypeDef",
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
@@ -1773,31 +1773,31 @@
 
 ConfigurationOptionsDescriptionTypeDef = TypedDict(
     "ConfigurationOptionsDescriptionTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "Options": List[ConfigurationOptionDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationSettingsDescriptionsTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionsTypeDef",
     {
         "ConfigurationSettings": List[ConfigurationSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentResourceDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentResourceDescriptionsMessageTypeDef",
     {
         "EnvironmentResources": EnvironmentResourceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentResourcesDescriptionTypeDef = TypedDict(
     "EnvironmentResourcesDescriptionTypeDef",
     {
         "LoadBalancer": LoadBalancerDescriptionTypeDef,
@@ -1805,23 +1805,23 @@
     total=False,
 )
 
 DescribePlatformVersionResultTypeDef = TypedDict(
     "DescribePlatformVersionResultTypeDef",
     {
         "PlatformDescription": PlatformDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "ResourceQuotas": ResourceQuotasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationDescriptionTypeDef = TypedDict(
     "ApplicationDescriptionTypeDef",
     {
         "ApplicationArn": str,
@@ -1837,15 +1837,15 @@
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1878,15 +1878,15 @@
 
 DescribeInstancesHealthResultTypeDef = TypedDict(
     "DescribeInstancesHealthResultTypeDef",
     {
         "InstanceHealthList": List[SingleInstanceHealthTypeDef],
         "RefreshedAt": datetime,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentDescriptionResponseMetadataTypeDef = TypedDict(
     "EnvironmentDescriptionResponseMetadataTypeDef",
     {
         "EnvironmentName": str,
@@ -1906,15 +1906,15 @@
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
         "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentDescriptionTypeDef = TypedDict(
     "EnvironmentDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1942,27 +1942,27 @@
     total=False,
 )
 
 ApplicationDescriptionMessageTypeDef = TypedDict(
     "ApplicationDescriptionMessageTypeDef",
     {
         "Application": ApplicationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationDescriptionsMessageTypeDef = TypedDict(
     "ApplicationDescriptionsMessageTypeDef",
     {
         "Applications": List[ApplicationDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentDescriptionsMessageTypeDef",
     {
         "Environments": List[EnvironmentDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/type_defs.pyi` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,61 +40,67 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
     "S3LocationTypeDef",
     "SourceBuildInformationTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
+    "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
+    "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
+    "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
     "DeleteApplicationVersionMessageRequestTypeDef",
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     "DeleteEnvironmentConfigurationMessageRequestTypeDef",
     "DeletePlatformVersionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
     "DescribeApplicationVersionsMessageRequestTypeDef",
     "DescribeApplicationsMessageRequestTypeDef",
     "DescribeConfigurationSettingsMessageRequestTypeDef",
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEnvironmentsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
@@ -102,29 +108,27 @@
     "EventDescriptionTypeDef",
     "SolutionStackDescriptionTypeDef",
     "SearchFilterTypeDef",
     "PlatformBranchSummaryTypeDef",
     "PlatformFilterTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ListenerTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
+    "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    "CreateStorageLocationResultMessageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
     "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
@@ -138,18 +142,14 @@
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
@@ -190,25 +190,14 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
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
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "P999": float,
         "P99": float,
         "P95": float,
         "P90": float,
@@ -302,14 +291,25 @@
 
 class ApplyEnvironmentManagedActionRequestRequestTypeDef(
     _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef,
     _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef,
 ):
     pass
 
+ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    {
+        "ActionId": str,
+        "ActionDescription": str,
+        "ActionType": ActionTypeType,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
         "OperationsRole": str,
     },
 )
@@ -370,14 +370,23 @@
 CheckDNSAvailabilityMessageRequestTypeDef = TypedDict(
     "CheckDNSAvailabilityMessageRequestTypeDef",
     {
         "CNAMEPrefix": str,
     },
 )
 
+CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    {
+        "Available": bool,
+        "FullyQualifiedCNAME": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ComposeEnvironmentsMessageRequestTypeDef = TypedDict(
     "ComposeEnvironmentsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "GroupName": str,
         "VersionLabels": Sequence[str],
     },
@@ -468,14 +477,22 @@
         "PlatformVersion": str,
         "PlatformBranchName": str,
         "PlatformBranchLifecycleState": str,
     },
     total=False,
 )
 
+CreateStorageLocationResultMessageTypeDef = TypedDict(
+    "CreateStorageLocationResultMessageTypeDef",
+    {
+        "S3Bucket": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomAmiTypeDef = TypedDict(
     "CustomAmiTypeDef",
     {
         "VirtualizationType": str,
         "ImageId": str,
     },
     total=False,
@@ -552,20 +569,20 @@
         "DeploymentId": int,
         "Status": str,
         "DeploymentTime": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ApplicationName": str,
+        "VersionLabels": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeApplicationVersionsMessageRequestTypeDef = TypedDict(
     "DescribeApplicationVersionsMessageRequestTypeDef",
     {
@@ -627,14 +644,24 @@
         "Warning": int,
         "Degraded": int,
         "Severe": int,
     },
     total=False,
 )
 
+DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    {
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
         "NextToken": str,
         "MaxItems": int,
@@ -684,14 +711,28 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -708,14 +749,32 @@
         "IncludedDeletedBackTo": Union[datetime, str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "TemplateName": str,
         "EnvironmentId": str,
@@ -753,14 +812,21 @@
 DisassociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnvironmentLinkTypeDef = TypedDict(
     "EnvironmentLinkTypeDef",
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -895,14 +961,24 @@
     {
         "Protocol": str,
         "Port": int,
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
 PlatformFrameworkTypeDef = TypedDict(
     "PlatformFrameworkTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -951,14 +1027,25 @@
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
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
 RestartAppServerMessageRequestTypeDef = TypedDict(
     "RestartAppServerMessageRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -1043,49 +1130,14 @@
 
 class UpdateApplicationVersionMessageRequestTypeDef(
     _RequiredUpdateApplicationVersionMessageRequestTypeDef,
     _OptionalUpdateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
-ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    {
-        "ActionId": str,
-        "ActionDescription": str,
-        "ActionType": ActionTypeType,
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    {
-        "Available": bool,
-        "FullyQualifiedCNAME": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStorageLocationResultMessageTypeDef = TypedDict(
-    "CreateStorageLocationResultMessageTypeDef",
-    {
-        "S3Bucket": str,
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
 ApplicationMetricsTypeDef = TypedDict(
     "ApplicationMetricsTypeDef",
     {
         "Duration": int,
         "RequestCount": int,
         "StatusCodes": StatusCodesTypeDef,
         "Latency": LatencyTypeDef,
@@ -1155,15 +1207,15 @@
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "OptionSettings": List[ConfigurationOptionSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
         "SolutionStackName": str,
@@ -1202,15 +1254,15 @@
 ):
     pass
 
 ConfigurationSettingsValidationMessagesTypeDef = TypedDict(
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1262,15 +1314,15 @@
     pass
 
 ResourceTagsDescriptionMessageTypeDef = TypedDict(
     "ResourceTagsDescriptionMessageTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1405,101 +1457,49 @@
 )
 
 CreatePlatformVersionResultTypeDef = TypedDict(
     "CreatePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
         "Builder": BuilderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePlatformVersionResultTypeDef = TypedDict(
     "DeletePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformVersionsResultTypeDef = TypedDict(
     "ListPlatformVersionsResultTypeDef",
     {
         "PlatformSummaryList": List[PlatformSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabels": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    {
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     {
         "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionsResultTypeDef",
     {
         "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
@@ -1547,15 +1547,15 @@
     total=False,
 )
 
 RetrieveEnvironmentInfoResultMessageTypeDef = TypedDict(
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     {
         "EnvironmentInfo": List[EnvironmentInfoDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentResourceDescriptionTypeDef = TypedDict(
     "EnvironmentResourceDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1571,24 +1571,24 @@
 )
 
 EventDescriptionsMessageTypeDef = TypedDict(
     "EventDescriptionsMessageTypeDef",
     {
         "Events": List[EventDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableSolutionStacksResultMessageTypeDef = TypedDict(
     "ListAvailableSolutionStacksResultMessageTypeDef",
     {
         "SolutionStacks": List[str],
         "SolutionStackDetails": List[SolutionStackDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformBranchesRequestRequestTypeDef = TypedDict(
     "ListPlatformBranchesRequestRequestTypeDef",
     {
         "Filters": Sequence[SearchFilterTypeDef],
@@ -1599,23 +1599,23 @@
 )
 
 ListPlatformBranchesResultTypeDef = TypedDict(
     "ListPlatformBranchesResultTypeDef",
     {
         "PlatformBranchSummaryList": List[PlatformBranchSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = TypedDict(
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     {
         "Filters": Sequence[PlatformFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPlatformVersionsRequestRequestTypeDef = TypedDict(
     "ListPlatformVersionsRequestRequestTypeDef",
     {
@@ -1683,32 +1683,32 @@
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
         "Causes": List[str],
         "ApplicationMetrics": ApplicationMetricsTypeDef,
         "InstancesHealth": InstanceHealthSummaryTypeDef,
         "RefreshedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationVersionDescriptionMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionMessageTypeDef",
     {
         "ApplicationVersion": ApplicationVersionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationVersionDescriptionsMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionsMessageTypeDef",
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
@@ -1736,31 +1736,31 @@
 
 ConfigurationOptionsDescriptionTypeDef = TypedDict(
     "ConfigurationOptionsDescriptionTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "Options": List[ConfigurationOptionDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationSettingsDescriptionsTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionsTypeDef",
     {
         "ConfigurationSettings": List[ConfigurationSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentResourceDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentResourceDescriptionsMessageTypeDef",
     {
         "EnvironmentResources": EnvironmentResourceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentResourcesDescriptionTypeDef = TypedDict(
     "EnvironmentResourcesDescriptionTypeDef",
     {
         "LoadBalancer": LoadBalancerDescriptionTypeDef,
@@ -1768,23 +1768,23 @@
     total=False,
 )
 
 DescribePlatformVersionResultTypeDef = TypedDict(
     "DescribePlatformVersionResultTypeDef",
     {
         "PlatformDescription": PlatformDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "ResourceQuotas": ResourceQuotasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationDescriptionTypeDef = TypedDict(
     "ApplicationDescriptionTypeDef",
     {
         "ApplicationArn": str,
@@ -1800,15 +1800,15 @@
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1839,15 +1839,15 @@
 
 DescribeInstancesHealthResultTypeDef = TypedDict(
     "DescribeInstancesHealthResultTypeDef",
     {
         "InstanceHealthList": List[SingleInstanceHealthTypeDef],
         "RefreshedAt": datetime,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentDescriptionResponseMetadataTypeDef = TypedDict(
     "EnvironmentDescriptionResponseMetadataTypeDef",
     {
         "EnvironmentName": str,
@@ -1867,15 +1867,15 @@
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
         "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentDescriptionTypeDef = TypedDict(
     "EnvironmentDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1903,27 +1903,27 @@
     total=False,
 )
 
 ApplicationDescriptionMessageTypeDef = TypedDict(
     "ApplicationDescriptionMessageTypeDef",
     {
         "Application": ApplicationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationDescriptionsMessageTypeDef = TypedDict(
     "ApplicationDescriptionsMessageTypeDef",
     {
         "Applications": List[ApplicationDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentDescriptionsMessageTypeDef",
     {
         "Environments": List[EnvironmentDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/waiter.py` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk/waiter.pyi` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.26.59
-Summary: Type annotations for boto3.ElasticBeanstalk 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticBeanstalk 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-elasticbeanstalk"></a>
 
 # mypy-boto3-elasticbeanstalk
 
 [![PyPI - mypy-boto3-elasticbeanstalk](https://img.shields.io/pypi/v/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticbeanstalk?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -395,61 +395,67 @@
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
     S3LocationTypeDef,
     SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
@@ -457,29 +463,27 @@
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
+    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
+    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
-    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
     ConfigurationSettingsDescriptionResponseMetadataTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
@@ -493,18 +497,14 @@
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
@@ -548,42 +548,42 @@
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

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt` & `mypy-boto3-elasticbeanstalk-1.27.0/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.26.59/setup.py` & `mypy-boto3-elasticbeanstalk-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-elasticbeanstalk.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticbeanstalk",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticBeanstalk 1.26.59 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ElasticBeanstalk 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/",
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


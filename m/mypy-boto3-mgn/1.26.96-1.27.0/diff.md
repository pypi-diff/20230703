# Comparing `tmp/mypy-boto3-mgn-1.26.96.tar.gz` & `tmp/mypy-boto3-mgn-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgn-1.26.96.tar", last modified: Tue Mar 21 19:19:40 2023, max compression
+gzip compressed data, was "mypy-boto3-mgn-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
```

## Comparing `mypy-boto3-mgn-1.26.96.tar` & `mypy-boto3-mgn-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.913032 mypy-boto3-mgn-1.26.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-03-21 19:19:40.913032 mypy-boto3-mgn-1.26.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.913032 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48373 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48291 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-21 19:19:26.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-03-21 19:19:26.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-03-21 19:19:26.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68530 2023-03-21 19:19:27.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68465 2023-03-21 19:19:27.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 19:19:25.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.913032 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-03-21 19:19:40.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-21 19:19:40.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 19:19:40.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-21 19:19:40.000000 mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:19:40.913032 mypy-boto3-mgn-1.26.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-21 19:19:24.000000 mypy-boto3-mgn-1.26.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22999 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21530 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.491685 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48373 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48291 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-03 19:42:21.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-03 19:42:20.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68618 2023-07-03 19:42:23.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68553 2023-07-03 19:42:22.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22999 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:08.000000 mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.495685 mypy-boto3-mgn-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:42:19.000000 mypy-boto3-mgn-1.27.0/setup.py
```

### Comparing `mypy-boto3-mgn-1.26.96/LICENSE` & `mypy-boto3-mgn-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mgn-1.26.96/PKG-INFO` & `mypy-boto3-mgn-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.26.96
-Summary: Type annotations for boto3.mgn 1.26.96 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.mgn 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,15 +406,14 @@
 
 `mypy_boto3_mgn.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mgn.type_defs import (
     ApplicationAggregatedStatusTypeDef,
-    ResponseMetadataTypeDef,
     ArchiveApplicationRequestRequestTypeDef,
     ArchiveWaveRequestRequestTypeDef,
     AssociateApplicationsRequestRequestTypeDef,
     AssociateSourceServersRequestRequestTypeDef,
     CPUTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     CreateApplicationRequestRequestTypeDef,
@@ -428,27 +427,31 @@
     DeleteApplicationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
     DeleteVcenterClientRequestRequestTypeDef,
     DeleteWaveRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
+    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
     DescribeVcenterClientsRequestRequestTypeDef,
     VcenterClientTypeDef,
     DisassociateApplicationsRequestRequestTypeDef,
     DisassociateSourceServersRequestRequestTypeDef,
     DisconnectFromServiceRequestRequestTypeDef,
     DiskTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportErrorDataTypeDef,
     ExportTaskSummaryTypeDef,
     FinalizeCutoverRequestRequestTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
@@ -461,30 +464,36 @@
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
     ListApplicationsRequestFiltersTypeDef,
+    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
+    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PaginatorConfigTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
+    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -492,27 +501,18 @@
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     UpdateSourceServerReplicationTypeRequestRequestTypeDef,
     UpdateWaveRequestRequestTypeDef,
     WaveAggregatedStatusTypeDef,
-    ApplicationTypeDef,
     ApplicationResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ApplicationTypeDef,
     ChangeServerLifeCycleStateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
-    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
-    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
@@ -590,42 +590,42 @@
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

### Comparing `mypy-boto3-mgn-1.26.96/README.md` & `mypy-boto3-mgn-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,15 +374,14 @@
 
 `mypy_boto3_mgn.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mgn.type_defs import (
     ApplicationAggregatedStatusTypeDef,
-    ResponseMetadataTypeDef,
     ArchiveApplicationRequestRequestTypeDef,
     ArchiveWaveRequestRequestTypeDef,
     AssociateApplicationsRequestRequestTypeDef,
     AssociateSourceServersRequestRequestTypeDef,
     CPUTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     CreateApplicationRequestRequestTypeDef,
@@ -396,27 +395,31 @@
     DeleteApplicationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
     DeleteVcenterClientRequestRequestTypeDef,
     DeleteWaveRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
+    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
     DescribeVcenterClientsRequestRequestTypeDef,
     VcenterClientTypeDef,
     DisassociateApplicationsRequestRequestTypeDef,
     DisassociateSourceServersRequestRequestTypeDef,
     DisconnectFromServiceRequestRequestTypeDef,
     DiskTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportErrorDataTypeDef,
     ExportTaskSummaryTypeDef,
     FinalizeCutoverRequestRequestTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
@@ -429,30 +432,36 @@
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
     ListApplicationsRequestFiltersTypeDef,
+    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
+    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PaginatorConfigTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
+    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -460,27 +469,18 @@
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     UpdateSourceServerReplicationTypeRequestRequestTypeDef,
     UpdateWaveRequestRequestTypeDef,
     WaveAggregatedStatusTypeDef,
-    ApplicationTypeDef,
     ApplicationResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ApplicationTypeDef,
     ChangeServerLifeCycleStateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
-    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
-    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
@@ -558,42 +558,42 @@
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

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/__init__.py` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/__init__.pyi` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/__main__.py` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mgn 1.26.96\nVersion:         1.26.96\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.mgn 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.96")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/client.py` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/client.pyi` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/literals.py` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,15 @@
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
@@ -272,14 +273,15 @@
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
@@ -377,14 +379,15 @@
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
@@ -420,14 +423,15 @@
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
@@ -446,16 +450,19 @@
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
@@ -539,15 +546,17 @@
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
@@ -588,24 +597,29 @@
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
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/literals.pyi` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,15 @@
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
@@ -270,14 +271,15 @@
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
@@ -375,14 +377,15 @@
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
@@ -418,14 +421,15 @@
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
@@ -444,16 +448,19 @@
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
@@ -537,15 +544,17 @@
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
@@ -586,24 +595,29 @@
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
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/paginator.py` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
         """
 
 
@@ -124,15 +124,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
 
 
@@ -142,15 +142,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 
@@ -160,15 +160,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
@@ -178,30 +178,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
 
 
 class DescribeVcenterClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVcenterClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
         """
 
 
@@ -211,30 +211,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
 
 
 class ListExportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
     """
 
     def paginate(
-        self, *, exportID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, exportID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
         """
 
 
@@ -244,30 +244,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
         """
 
 
 class ListImportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
     """
 
     def paginate(
-        self, *, importID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, importID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
         """
 
 
@@ -277,15 +277,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 
@@ -296,15 +296,15 @@
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 
@@ -315,15 +315,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listtemplateactionspaginator)
         """
 
 
@@ -333,13 +333,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/paginator.pyi` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 class DescribeJobLogItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejoblogitemspaginator)
         """
 
 class DescribeJobsPaginator(Paginator):
@@ -120,15 +120,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describejobspaginator)
         """
 
 class DescribeLaunchConfigurationTemplatesPaginator(Paginator):
@@ -137,15 +137,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(Paginator):
@@ -154,15 +154,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 class DescribeSourceServersPaginator(Paginator):
@@ -171,29 +171,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describesourceserverspaginator)
         """
 
 class DescribeVcenterClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVcenterClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#describevcenterclientspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
@@ -202,29 +202,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listapplicationspaginator)
         """
 
 class ListExportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
     """
 
     def paginate(
-        self, *, exportID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, exportID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexporterrorspaginator)
         """
 
 class ListExportsPaginator(Paginator):
@@ -233,29 +233,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListExportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listexportspaginator)
         """
 
 class ListImportErrorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
     """
 
     def paginate(
-        self, *, importID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, importID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportErrorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImportErrors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimporterrorspaginator)
         """
 
 class ListImportsPaginator(Paginator):
@@ -264,15 +264,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListImportsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listimportspaginator)
         """
 
 class ListSourceServerActionsPaginator(Paginator):
@@ -282,15 +282,15 @@
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listsourceserveractionspaginator)
         """
 
 class ListTemplateActionsPaginator(Paginator):
@@ -300,15 +300,15 @@
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateID: str,
         filters: TemplateActionsRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplateActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListTemplateActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listtemplateactionspaginator)
         """
 
 class ListWavesPaginator(Paginator):
@@ -317,13 +317,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: ListWavesRequestFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/type_defs.py` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationAggregatedStatusTypeDef",
-    "ResponseMetadataTypeDef",
     "ArchiveApplicationRequestRequestTypeDef",
     "ArchiveWaveRequestRequestTypeDef",
     "AssociateApplicationsRequestRequestTypeDef",
     "AssociateSourceServersRequestRequestTypeDef",
     "CPUTypeDef",
     "ChangeServerLifeCycleStateSourceServerLifecycleTypeDef",
     "CreateApplicationRequestRequestTypeDef",
@@ -79,27 +78,31 @@
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
     "DeleteVcenterClientRequestRequestTypeDef",
     "DeleteWaveRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
     "DescribeVcenterClientsRequestRequestTypeDef",
     "VcenterClientTypeDef",
     "DisassociateApplicationsRequestRequestTypeDef",
     "DisassociateSourceServersRequestRequestTypeDef",
     "DisconnectFromServiceRequestRequestTypeDef",
     "DiskTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportErrorDataTypeDef",
     "ExportTaskSummaryTypeDef",
     "FinalizeCutoverRequestRequestTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ImportErrorDataTypeDef",
@@ -112,30 +115,36 @@
     "LifeCycleLastCutoverFinalizedTypeDef",
     "LifeCycleLastCutoverInitiatedTypeDef",
     "LifeCycleLastCutoverRevertedTypeDef",
     "LifeCycleLastTestFinalizedTypeDef",
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
     "ListApplicationsRequestFiltersTypeDef",
+    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
+    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PaginatorConfigTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
@@ -143,27 +152,18 @@
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
     "UpdateWaveRequestRequestTypeDef",
     "WaveAggregatedStatusTypeDef",
-    "ApplicationTypeDef",
     "ApplicationResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ApplicationTypeDef",
     "ChangeServerLifeCycleStateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
-    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
@@ -240,25 +240,14 @@
         "lastUpdateDateTime": str,
         "progressStatus": ApplicationProgressStatusType,
         "totalSourceServers": int,
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
 ArchiveApplicationRequestRequestTypeDef = TypedDict(
     "ArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
 
@@ -471,24 +460,36 @@
 DeleteWaveRequestRequestTypeDef = TypedDict(
     "DeleteWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -514,24 +515,42 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     {
         "launchConfigurationTemplateIDs": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
@@ -581,14 +600,22 @@
         "lifeCycleStates": Sequence[LifeCycleStateType],
         "replicationTypes": Sequence[ReplicationTypeType],
         "sourceServerIDs": Sequence[str],
     },
     total=False,
 )
 
+DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeVcenterClientsRequestRequestTypeDef = TypedDict(
     "DescribeVcenterClientsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -637,14 +664,21 @@
     {
         "bytes": int,
         "deviceName": str,
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
 ExportErrorDataTypeDef = TypedDict(
     "ExportErrorDataTypeDef",
     {
         "rawError": str,
     },
     total=False,
 )
@@ -829,14 +863,36 @@
         "applicationIDs": Sequence[str],
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "exportID": str,
+    },
+)
+_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
+    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListExportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListExportErrorsRequestRequestTypeDef",
     {
         "exportID": str,
     },
 )
 _OptionalListExportErrorsRequestRequestTypeDef = TypedDict(
@@ -859,14 +915,36 @@
     "ListExportsRequestFiltersTypeDef",
     {
         "exportIDs": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "importID": str,
+    },
+)
+_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
+    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListImportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListImportErrorsRequestRequestTypeDef",
     {
         "importID": str,
     },
 )
 _OptionalListImportErrorsRequestRequestTypeDef = TypedDict(
@@ -904,14 +982,22 @@
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
 TemplateActionsRequestFiltersTypeDef = TypedDict(
     "TemplateActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -946,14 +1032,24 @@
     "OSTypeDef",
     {
         "fullString": str,
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
 SsmExternalParameterTypeDef = TypedDict(
     "SsmExternalParameterTypeDef",
     {
         "dynamicPath": str,
     },
     total=False,
 )
@@ -990,14 +1086,47 @@
         "isBootDisk": bool,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
     },
     total=False,
 )
 
+ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -1218,83 +1347,46 @@
         "progressStatus": WaveProgressStatusType,
         "replicationStartedDateTime": str,
         "totalApplications": int,
     },
     total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+ApplicationResponseMetadataTypeDef = TypedDict(
+    "ApplicationResponseMetadataTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
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
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 ChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
     "ChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
@@ -1307,111 +1399,19 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
-
-DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    {
-        "launchConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "exportID": str,
-    },
-)
-_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
-    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "importID": str,
-    },
-)
-_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
-    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
-    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
-):
-    pass
-
-
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1423,23 +1423,23 @@
 )
 
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1451,15 +1451,15 @@
 )
 
 DescribeVcenterClientsResponseTypeDef = TypedDict(
     "DescribeVcenterClientsResponseTypeDef",
     {
         "items": List[VcenterClientTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTaskErrorTypeDef = TypedDict(
     "ExportTaskErrorTypeDef",
     {
         "errorData": ExportErrorDataTypeDef,
@@ -1555,15 +1555,15 @@
     total=False,
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "filters": ListApplicationsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
@@ -1574,15 +1574,15 @@
     total=False,
 )
 
 ListExportsRequestListExportsPaginateTypeDef = TypedDict(
     "ListExportsRequestListExportsPaginateTypeDef",
     {
         "filters": ListExportsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListExportsRequestRequestTypeDef = TypedDict(
     "ListExportsRequestRequestTypeDef",
     {
@@ -1593,15 +1593,15 @@
     total=False,
 )
 
 ListImportsRequestListImportsPaginateTypeDef = TypedDict(
     "ListImportsRequestListImportsPaginateTypeDef",
     {
         "filters": ListImportsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
@@ -1618,15 +1618,15 @@
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "filters": SourceServerActionsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(
     _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
@@ -1665,15 +1665,15 @@
         "launchConfigurationTemplateID": str,
     },
 )
 _OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef = TypedDict(
     "_OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     {
         "filters": TemplateActionsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListTemplateActionsRequestListTemplateActionsPaginateTypeDef(
     _RequiredListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
@@ -1706,15 +1706,15 @@
     pass
 
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
         "filters": ListWavesRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
@@ -1817,15 +1817,15 @@
         "documentIdentifier": str,
         "documentVersion": str,
         "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
         "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerActionDocumentTypeDef = TypedDict(
     "SourceServerActionDocumentTypeDef",
     {
         "actionID": str,
@@ -1879,15 +1879,15 @@
         "documentVersion": str,
         "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
         "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TemplateActionDocumentTypeDef = TypedDict(
     "TemplateActionDocumentTypeDef",
     {
         "actionID": str,
@@ -1921,15 +1921,15 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1972,15 +1972,15 @@
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveAggregatedStatus": WaveAggregatedStatusTypeDef,
         "waveID": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WaveTypeDef = TypedDict(
     "WaveTypeDef",
     {
         "arn": str,
@@ -1997,15 +1997,15 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "items": List[ApplicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -2020,41 +2020,41 @@
 )
 
 ListExportErrorsResponseTypeDef = TypedDict(
     "ListExportErrorsResponseTypeDef",
     {
         "items": List[ExportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "items": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartExportResponseTypeDef = TypedDict(
     "StartExportResponseTypeDef",
     {
         "exportTask": ExportTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportErrorsResponseTypeDef = TypedDict(
     "ListImportErrorsResponseTypeDef",
     {
         "items": List[ImportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTaskTypeDef = TypedDict(
     "ImportTaskTypeDef",
     {
         "creationDateTime": str,
@@ -2069,15 +2069,15 @@
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
         "items": List[JobLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
@@ -2092,15 +2092,15 @@
 )
 
 ListSourceServerActionsResponseTypeDef = TypedDict(
     "ListSourceServerActionsResponseTypeDef",
     {
         "items": List[SourceServerActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
@@ -2125,41 +2125,41 @@
 )
 
 ListTemplateActionsResponseTypeDef = TypedDict(
     "ListTemplateActionsResponseTypeDef",
     {
         "items": List[TemplateActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWavesResponseTypeDef = TypedDict(
     "ListWavesResponseTypeDef",
     {
         "items": List[WaveTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "items": List[ImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "importTask": ImportTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerResponseMetadataTypeDef = TypedDict(
     "SourceServerResponseMetadataTypeDef",
     {
         "applicationID": str,
@@ -2171,15 +2171,15 @@
         "lifeCycle": LifeCycleTypeDef,
         "replicationType": ReplicationTypeType,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "applicationID": str,
@@ -2245,15 +2245,15 @@
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
         "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
     "_RequiredLaunchConfigurationTemplateTypeDef",
     {
         "launchConfigurationTemplateID": str,
@@ -2300,15 +2300,15 @@
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "name": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -2374,15 +2374,15 @@
 
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredParticipatingServerTypeDef = TypedDict(
     "_RequiredParticipatingServerTypeDef",
     {
         "sourceServerID": str,
@@ -2406,15 +2406,15 @@
 
 
 DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     {
         "items": List[LaunchConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
@@ -2441,34 +2441,34 @@
 
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartCutoverResponseTypeDef = TypedDict(
     "StartCutoverResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTestResponseTypeDef = TypedDict(
     "StartTestResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TerminateTargetInstancesResponseTypeDef = TypedDict(
     "TerminateTargetInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn/type_defs.pyi` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationAggregatedStatusTypeDef",
-    "ResponseMetadataTypeDef",
     "ArchiveApplicationRequestRequestTypeDef",
     "ArchiveWaveRequestRequestTypeDef",
     "AssociateApplicationsRequestRequestTypeDef",
     "AssociateSourceServersRequestRequestTypeDef",
     "CPUTypeDef",
     "ChangeServerLifeCycleStateSourceServerLifecycleTypeDef",
     "CreateApplicationRequestRequestTypeDef",
@@ -78,27 +77,31 @@
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
     "DeleteVcenterClientRequestRequestTypeDef",
     "DeleteWaveRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
     "DescribeVcenterClientsRequestRequestTypeDef",
     "VcenterClientTypeDef",
     "DisassociateApplicationsRequestRequestTypeDef",
     "DisassociateSourceServersRequestRequestTypeDef",
     "DisconnectFromServiceRequestRequestTypeDef",
     "DiskTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportErrorDataTypeDef",
     "ExportTaskSummaryTypeDef",
     "FinalizeCutoverRequestRequestTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ImportErrorDataTypeDef",
@@ -111,30 +114,36 @@
     "LifeCycleLastCutoverFinalizedTypeDef",
     "LifeCycleLastCutoverInitiatedTypeDef",
     "LifeCycleLastCutoverRevertedTypeDef",
     "LifeCycleLastTestFinalizedTypeDef",
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
     "ListApplicationsRequestFiltersTypeDef",
+    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
+    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PaginatorConfigTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
@@ -142,27 +151,18 @@
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
     "UpdateWaveRequestRequestTypeDef",
     "WaveAggregatedStatusTypeDef",
-    "ApplicationTypeDef",
     "ApplicationResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ApplicationTypeDef",
     "ChangeServerLifeCycleStateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
-    "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
@@ -239,25 +239,14 @@
         "lastUpdateDateTime": str,
         "progressStatus": ApplicationProgressStatusType,
         "totalSourceServers": int,
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
 ArchiveApplicationRequestRequestTypeDef = TypedDict(
     "ArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
 
@@ -464,24 +453,34 @@
 DeleteWaveRequestRequestTypeDef = TypedDict(
     "DeleteWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -505,24 +504,42 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     {
         "launchConfigurationTemplateIDs": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
@@ -570,14 +587,22 @@
         "lifeCycleStates": Sequence[LifeCycleStateType],
         "replicationTypes": Sequence[ReplicationTypeType],
         "sourceServerIDs": Sequence[str],
     },
     total=False,
 )
 
+DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
+    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeVcenterClientsRequestRequestTypeDef = TypedDict(
     "DescribeVcenterClientsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -626,14 +651,21 @@
     {
         "bytes": int,
         "deviceName": str,
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
 ExportErrorDataTypeDef = TypedDict(
     "ExportErrorDataTypeDef",
     {
         "rawError": str,
     },
     total=False,
 )
@@ -816,14 +848,34 @@
         "applicationIDs": Sequence[str],
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "exportID": str,
+    },
+)
+_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
+    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
+    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
+):
+    pass
+
 _RequiredListExportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListExportErrorsRequestRequestTypeDef",
     {
         "exportID": str,
     },
 )
 _OptionalListExportErrorsRequestRequestTypeDef = TypedDict(
@@ -844,14 +896,34 @@
     "ListExportsRequestFiltersTypeDef",
     {
         "exportIDs": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "importID": str,
+    },
+)
+_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
+    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
+    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
+    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
+):
+    pass
+
 _RequiredListImportErrorsRequestRequestTypeDef = TypedDict(
     "_RequiredListImportErrorsRequestRequestTypeDef",
     {
         "importID": str,
     },
 )
 _OptionalListImportErrorsRequestRequestTypeDef = TypedDict(
@@ -887,14 +959,22 @@
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
 TemplateActionsRequestFiltersTypeDef = TypedDict(
     "TemplateActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -929,14 +1009,24 @@
     "OSTypeDef",
     {
         "fullString": str,
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
 SsmExternalParameterTypeDef = TypedDict(
     "SsmExternalParameterTypeDef",
     {
         "dynamicPath": str,
     },
     total=False,
 )
@@ -973,14 +1063,47 @@
         "isBootDisk": bool,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
     },
     total=False,
 )
 
+ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    {
+        "arn": str,
+        "associateDefaultSecurityGroup": bool,
+        "bandwidthThrottling": int,
+        "createPublicIP": bool,
+        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
+        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
+        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
+        "ebsEncryptionKeyArn": str,
+        "replicationConfigurationTemplateID": str,
+        "replicationServerInstanceType": str,
+        "replicationServersSecurityGroupsIDs": List[str],
+        "stagingAreaSubnetId": str,
+        "stagingAreaTags": Dict[str, str],
+        "tags": Dict[str, str],
+        "useDedicatedReplicationServer": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -1187,83 +1310,46 @@
         "progressStatus": WaveProgressStatusType,
         "replicationStartedDateTime": str,
         "totalApplications": int,
     },
     total=False,
 )
 
-ApplicationTypeDef = TypedDict(
-    "ApplicationTypeDef",
+ApplicationResponseMetadataTypeDef = TypedDict(
+    "ApplicationResponseMetadataTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
     {
         "applicationAggregatedStatus": ApplicationAggregatedStatusTypeDef,
         "applicationID": str,
         "arn": str,
         "creationDateTime": str,
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveID": str,
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
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
-    {
-        "arn": str,
-        "associateDefaultSecurityGroup": bool,
-        "bandwidthThrottling": int,
-        "createPublicIP": bool,
-        "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
-        "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
-        "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
-        "ebsEncryptionKeyArn": str,
-        "replicationConfigurationTemplateID": str,
-        "replicationServerInstanceType": str,
-        "replicationServersSecurityGroupsIDs": List[str],
-        "stagingAreaSubnetId": str,
-        "stagingAreaTags": Dict[str, str],
-        "tags": Dict[str, str],
-        "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 ChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
     "ChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
@@ -1276,105 +1362,19 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
-DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    {
-        "launchConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef = TypedDict(
-    "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "exportID": str,
-    },
-)
-_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListExportErrorsRequestListExportErrorsPaginateTypeDef(
-    _RequiredListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    _OptionalListExportErrorsRequestListExportErrorsPaginateTypeDef,
-):
-    pass
-
-_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "importID": str,
-    },
-)
-_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef = TypedDict(
-    "_OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
-    _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
-    _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
-):
-    pass
-
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1386,23 +1386,23 @@
 )
 
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1414,15 +1414,15 @@
 )
 
 DescribeVcenterClientsResponseTypeDef = TypedDict(
     "DescribeVcenterClientsResponseTypeDef",
     {
         "items": List[VcenterClientTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTaskErrorTypeDef = TypedDict(
     "ExportTaskErrorTypeDef",
     {
         "errorData": ExportErrorDataTypeDef,
@@ -1516,15 +1516,15 @@
     total=False,
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
         "filters": ListApplicationsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
@@ -1535,15 +1535,15 @@
     total=False,
 )
 
 ListExportsRequestListExportsPaginateTypeDef = TypedDict(
     "ListExportsRequestListExportsPaginateTypeDef",
     {
         "filters": ListExportsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListExportsRequestRequestTypeDef = TypedDict(
     "ListExportsRequestRequestTypeDef",
     {
@@ -1554,15 +1554,15 @@
     total=False,
 )
 
 ListImportsRequestListImportsPaginateTypeDef = TypedDict(
     "ListImportsRequestListImportsPaginateTypeDef",
     {
         "filters": ListImportsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
@@ -1579,15 +1579,15 @@
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "filters": SourceServerActionsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(
     _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
     _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef,
@@ -1622,15 +1622,15 @@
         "launchConfigurationTemplateID": str,
     },
 )
 _OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef = TypedDict(
     "_OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     {
         "filters": TemplateActionsRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListTemplateActionsRequestListTemplateActionsPaginateTypeDef(
     _RequiredListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
     _OptionalListTemplateActionsRequestListTemplateActionsPaginateTypeDef,
@@ -1659,15 +1659,15 @@
 ):
     pass
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
         "filters": ListWavesRequestFiltersTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
@@ -1766,15 +1766,15 @@
         "documentIdentifier": str,
         "documentVersion": str,
         "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "order": int,
         "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerActionDocumentTypeDef = TypedDict(
     "SourceServerActionDocumentTypeDef",
     {
         "actionID": str,
@@ -1826,15 +1826,15 @@
         "documentVersion": str,
         "externalParameters": Dict[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "operatingSystem": str,
         "order": int,
         "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TemplateActionDocumentTypeDef = TypedDict(
     "TemplateActionDocumentTypeDef",
     {
         "actionID": str,
@@ -1868,15 +1868,15 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1917,15 +1917,15 @@
         "description": str,
         "isArchived": bool,
         "lastModifiedDateTime": str,
         "name": str,
         "tags": Dict[str, str],
         "waveAggregatedStatus": WaveAggregatedStatusTypeDef,
         "waveID": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WaveTypeDef = TypedDict(
     "WaveTypeDef",
     {
         "arn": str,
@@ -1942,15 +1942,15 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "items": List[ApplicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -1965,41 +1965,41 @@
 )
 
 ListExportErrorsResponseTypeDef = TypedDict(
     "ListExportErrorsResponseTypeDef",
     {
         "items": List[ExportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsResponseTypeDef = TypedDict(
     "ListExportsResponseTypeDef",
     {
         "items": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartExportResponseTypeDef = TypedDict(
     "StartExportResponseTypeDef",
     {
         "exportTask": ExportTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportErrorsResponseTypeDef = TypedDict(
     "ListImportErrorsResponseTypeDef",
     {
         "items": List[ImportTaskErrorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTaskTypeDef = TypedDict(
     "ImportTaskTypeDef",
     {
         "creationDateTime": str,
@@ -2014,15 +2014,15 @@
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
         "items": List[JobLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifeCycleTypeDef = TypedDict(
     "LifeCycleTypeDef",
     {
         "addedToServiceDateTime": str,
@@ -2037,15 +2037,15 @@
 )
 
 ListSourceServerActionsResponseTypeDef = TypedDict(
     "ListSourceServerActionsResponseTypeDef",
     {
         "items": List[SourceServerActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
@@ -2070,41 +2070,41 @@
 )
 
 ListTemplateActionsResponseTypeDef = TypedDict(
     "ListTemplateActionsResponseTypeDef",
     {
         "items": List[TemplateActionDocumentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWavesResponseTypeDef = TypedDict(
     "ListWavesResponseTypeDef",
     {
         "items": List[WaveTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "items": List[ImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "importTask": ImportTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerResponseMetadataTypeDef = TypedDict(
     "SourceServerResponseMetadataTypeDef",
     {
         "applicationID": str,
@@ -2116,15 +2116,15 @@
         "lifeCycle": LifeCycleTypeDef,
         "replicationType": ReplicationTypeType,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
         "userProvidedID": str,
         "vcenterClientID": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "applicationID": str,
@@ -2190,15 +2190,15 @@
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
         "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLaunchConfigurationTemplateTypeDef = TypedDict(
     "_RequiredLaunchConfigurationTemplateTypeDef",
     {
         "launchConfigurationTemplateID": str,
@@ -2243,15 +2243,15 @@
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "name": str,
         "postLaunchActions": PostLaunchActionsTypeDef,
         "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -2313,15 +2313,15 @@
     pass
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredParticipatingServerTypeDef = TypedDict(
     "_RequiredParticipatingServerTypeDef",
     {
         "sourceServerID": str,
@@ -2343,15 +2343,15 @@
     pass
 
 DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     {
         "items": List[LaunchConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "jobID": str,
@@ -2376,34 +2376,34 @@
     pass
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartCutoverResponseTypeDef = TypedDict(
     "StartCutoverResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTestResponseTypeDef = TypedDict(
     "StartTestResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TerminateTargetInstancesResponseTypeDef = TypedDict(
     "TerminateTargetInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/PKG-INFO` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgn
-Version: 1.26.96
-Summary: Type annotations for boto3.mgn 1.26.96 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.mgn 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mgn"></a>
 
 # mypy-boto3-mgn
 
 [![PyPI - mypy-boto3-mgn](https://img.shields.io/pypi/v/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgn.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgn)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgn?color=blue)](https://pypistats.org/packages/mypy-boto3-mgn)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mgn 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
+[boto3.mgn 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
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
 [mypy-boto3-mgn docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,15 +406,14 @@
 
 `mypy_boto3_mgn.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mgn.type_defs import (
     ApplicationAggregatedStatusTypeDef,
-    ResponseMetadataTypeDef,
     ArchiveApplicationRequestRequestTypeDef,
     ArchiveWaveRequestRequestTypeDef,
     AssociateApplicationsRequestRequestTypeDef,
     AssociateSourceServersRequestRequestTypeDef,
     CPUTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
     CreateApplicationRequestRequestTypeDef,
@@ -428,27 +427,31 @@
     DeleteApplicationRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
     DeleteVcenterClientRequestRequestTypeDef,
     DeleteWaveRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
+    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
     DescribeVcenterClientsRequestRequestTypeDef,
     VcenterClientTypeDef,
     DisassociateApplicationsRequestRequestTypeDef,
     DisassociateSourceServersRequestRequestTypeDef,
     DisconnectFromServiceRequestRequestTypeDef,
     DiskTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportErrorDataTypeDef,
     ExportTaskSummaryTypeDef,
     FinalizeCutoverRequestRequestTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ImportErrorDataTypeDef,
@@ -461,30 +464,36 @@
     LifeCycleLastCutoverFinalizedTypeDef,
     LifeCycleLastCutoverInitiatedTypeDef,
     LifeCycleLastCutoverRevertedTypeDef,
     LifeCycleLastTestFinalizedTypeDef,
     LifeCycleLastTestInitiatedTypeDef,
     LifeCycleLastTestRevertedTypeDef,
     ListApplicationsRequestFiltersTypeDef,
+    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
     ListExportErrorsRequestRequestTypeDef,
     ListExportsRequestFiltersTypeDef,
+    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     ListImportErrorsRequestRequestTypeDef,
     ListImportsRequestFiltersTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TemplateActionsRequestFiltersTypeDef,
     ListWavesRequestFiltersTypeDef,
     MarkAsArchivedRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
+    PaginatorConfigTypeDef,
     SsmExternalParameterTypeDef,
     SsmParameterStoreParameterTypeDef,
     RemoveSourceServerActionRequestRequestTypeDef,
     RemoveTemplateActionRequestRequestTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
+    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     StartCutoverRequestRequestTypeDef,
     StartExportRequestRequestTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartTestRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateTargetInstancesRequestRequestTypeDef,
@@ -492,27 +501,18 @@
     UnarchiveWaveRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     UpdateSourceServerReplicationTypeRequestRequestTypeDef,
     UpdateWaveRequestRequestTypeDef,
     WaveAggregatedStatusTypeDef,
-    ApplicationTypeDef,
     ApplicationResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ApplicationTypeDef,
     ChangeServerLifeCycleStateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
-    DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef,
-    ListExportErrorsRequestListExportErrorsPaginateTypeDef,
-    ListImportErrorsRequestListImportErrorsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeReplicationConfigurationTemplatesResponseTypeDef,
     DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef,
     DescribeSourceServersRequestRequestTypeDef,
     DescribeVcenterClientsResponseTypeDef,
     ExportTaskErrorTypeDef,
@@ -590,42 +590,42 @@
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

### Comparing `mypy-boto3-mgn-1.26.96/mypy_boto3_mgn.egg-info/SOURCES.txt` & `mypy-boto3-mgn-1.27.0/mypy_boto3_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgn-1.26.96/setup.py` & `mypy-boto3-mgn-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-mgn.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgn",
-    version="1.26.96",
+    version="1.27.0",
     packages=["mypy_boto3_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mgn 1.26.96 service generated with mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.mgn 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgn/",
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


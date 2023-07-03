# Comparing `tmp/mypy-boto3-greengrass-1.26.59.tar.gz` & `tmp/mypy-boto3-greengrass-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrass-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrass-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-greengrass-1.26.59.tar` & `mypy-boto3-greengrass-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.584096 mypy-boto3-greengrass-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27740 2023-01-27 20:32:50.584096 mypy-boto3-greengrass-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.572096 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-01-27 20:32:11.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-01-27 20:32:11.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-01-27 20:32:11.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-01-27 20:32:11.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    88811 2023-01-27 20:32:13.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    88694 2023-01-27 20:32:11.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.584096 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27740 2023-01-27 20:32:50.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-27 20:32:50.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-27 20:32:50.000000 mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.584096 mypy-boto3-greengrass-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-27 20:32:10.000000 mypy-boto3-greengrass-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.031346 mypy-boto3-greengrass-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27719 2023-07-03 19:50:50.031346 mypy-boto3-greengrass-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.023346 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68713 2023-07-03 19:38:37.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68595 2023-07-03 19:38:37.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-03 19:38:37.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-03 19:38:37.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-07-03 19:38:37.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-03 19:38:37.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    89019 2023-07-03 19:38:39.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88902 2023-07-03 19:38:38.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.031346 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27719 2023-07-03 19:50:49.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:49.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:49.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:49.000000 mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.031346 mypy-boto3-greengrass-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:38:35.000000 mypy-boto3-greengrass-1.27.0/setup.py
```

### Comparing `mypy-boto3-greengrass-1.26.59/LICENSE` & `mypy-boto3-greengrass-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-greengrass-1.26.59/PKG-INFO` & `mypy-boto3-greengrass-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.26.59
-Summary: Type annotations for boto3.Greengrass 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Greengrass 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrass?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,151 +423,170 @@
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
     ConnectivityInfoTypeDef,
     ConnectorTypeDef,
     CoreTypeDef,
+    CreateConnectorDefinitionResponseTypeDef,
+    CreateConnectorDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionResponseTypeDef,
+    CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateDeviceDefinitionResponseTypeDef,
     DeviceTypeDef,
+    CreateDeviceDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionResponseTypeDef,
+    CreateFunctionDefinitionVersionResponseTypeDef,
     CreateGroupCertificateAuthorityRequestRequestTypeDef,
+    CreateGroupCertificateAuthorityResponseTypeDef,
     GroupVersionTypeDef,
+    CreateGroupResponseTypeDef,
     CreateGroupVersionRequestRequestTypeDef,
+    CreateGroupVersionResponseTypeDef,
+    CreateLoggerDefinitionResponseTypeDef,
     LoggerTypeDef,
+    CreateLoggerDefinitionVersionResponseTypeDef,
+    CreateResourceDefinitionResponseTypeDef,
+    CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobRequestRequestTypeDef,
+    CreateSoftwareUpdateJobResponseTypeDef,
+    CreateSubscriptionDefinitionResponseTypeDef,
     SubscriptionTypeDef,
+    CreateSubscriptionDefinitionVersionResponseTypeDef,
     DefinitionInformationTypeDef,
     DeleteConnectorDefinitionRequestRequestTypeDef,
     DeleteCoreDefinitionRequestRequestTypeDef,
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
+    DisassociateRoleFromGroupResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceAccessPolicyTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
+    GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
+    GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionRequestRequestTypeDef,
+    GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionRequestRequestTypeDef,
     GetDeploymentStatusRequestRequestTypeDef,
     GetDeviceDefinitionRequestRequestTypeDef,
+    GetDeviceDefinitionResponseTypeDef,
     GetDeviceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionRequestRequestTypeDef,
+    GetFunctionDefinitionResponseTypeDef,
     GetFunctionDefinitionVersionRequestRequestTypeDef,
     GetGroupCertificateAuthorityRequestRequestTypeDef,
+    GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
+    GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
+    GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
+    GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
+    GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
+    GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
     GroupOwnerSettingTypeDef,
-    PaginatorConfigTypeDef,
+    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
+    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
+    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
     VersionInformationTypeDef,
+    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
     ListConnectorDefinitionsRequestRequestTypeDef,
+    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     ListCoreDefinitionVersionsRequestRequestTypeDef,
+    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
     ListCoreDefinitionsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     ListDeviceDefinitionVersionsRequestRequestTypeDef,
+    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
     ListDeviceDefinitionsRequestRequestTypeDef,
+    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     ListFunctionDefinitionVersionsRequestRequestTypeDef,
+    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
     ListFunctionDefinitionsRequestRequestTypeDef,
     ListGroupCertificateAuthoritiesRequestRequestTypeDef,
+    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     ListGroupVersionsRequestRequestTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
+    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     ListLoggerDefinitionVersionsRequestRequestTypeDef,
+    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
     ListLoggerDefinitionsRequestRequestTypeDef,
+    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     ListResourceDefinitionVersionsRequestRequestTypeDef,
+    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
     ListResourceDefinitionsRequestRequestTypeDef,
+    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
+    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
+    ResetDeploymentsResponseTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
+    ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
+    StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
     UpdateFunctionDefinitionRequestRequestTypeDef,
     UpdateGroupCertificateConfigurationRequestRequestTypeDef,
+    UpdateGroupCertificateConfigurationResponseTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateLoggerDefinitionRequestRequestTypeDef,
     UpdateResourceDefinitionRequestRequestTypeDef,
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
-    AssociateRoleToGroupResponseTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
-    CreateConnectorDefinitionResponseTypeDef,
-    CreateConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionResponseTypeDef,
-    CreateCoreDefinitionVersionResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateDeviceDefinitionResponseTypeDef,
-    CreateDeviceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionResponseTypeDef,
-    CreateFunctionDefinitionVersionResponseTypeDef,
-    CreateGroupCertificateAuthorityResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateGroupVersionResponseTypeDef,
-    CreateLoggerDefinitionResponseTypeDef,
-    CreateLoggerDefinitionVersionResponseTypeDef,
-    CreateResourceDefinitionResponseTypeDef,
-    CreateResourceDefinitionVersionResponseTypeDef,
-    CreateSoftwareUpdateJobResponseTypeDef,
-    CreateSubscriptionDefinitionResponseTypeDef,
-    CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DisassociateRoleFromGroupResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAssociatedRoleResponseTypeDef,
-    GetConnectorDefinitionResponseTypeDef,
-    GetCoreDefinitionResponseTypeDef,
-    GetDeviceDefinitionResponseTypeDef,
-    GetFunctionDefinitionResponseTypeDef,
-    GetGroupCertificateAuthorityResponseTypeDef,
-    GetGroupCertificateConfigurationResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetLoggerDefinitionResponseTypeDef,
-    GetResourceDefinitionResponseTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
-    GetSubscriptionDefinitionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResetDeploymentsResponseTypeDef,
-    StartBulkDeploymentResponseTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
-    UpdateGroupCertificateConfigurationResponseTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionTypeDef,
@@ -592,33 +611,14 @@
     ListDeploymentsResponseTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
-    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
-    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
-    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
-    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
-    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
-    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
-    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
-    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
@@ -663,42 +663,42 @@
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

### Comparing `mypy-boto3-greengrass-1.26.59/README.md` & `mypy-boto3-greengrass-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrass?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,151 +391,170 @@
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
     ConnectivityInfoTypeDef,
     ConnectorTypeDef,
     CoreTypeDef,
+    CreateConnectorDefinitionResponseTypeDef,
+    CreateConnectorDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionResponseTypeDef,
+    CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateDeviceDefinitionResponseTypeDef,
     DeviceTypeDef,
+    CreateDeviceDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionResponseTypeDef,
+    CreateFunctionDefinitionVersionResponseTypeDef,
     CreateGroupCertificateAuthorityRequestRequestTypeDef,
+    CreateGroupCertificateAuthorityResponseTypeDef,
     GroupVersionTypeDef,
+    CreateGroupResponseTypeDef,
     CreateGroupVersionRequestRequestTypeDef,
+    CreateGroupVersionResponseTypeDef,
+    CreateLoggerDefinitionResponseTypeDef,
     LoggerTypeDef,
+    CreateLoggerDefinitionVersionResponseTypeDef,
+    CreateResourceDefinitionResponseTypeDef,
+    CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobRequestRequestTypeDef,
+    CreateSoftwareUpdateJobResponseTypeDef,
+    CreateSubscriptionDefinitionResponseTypeDef,
     SubscriptionTypeDef,
+    CreateSubscriptionDefinitionVersionResponseTypeDef,
     DefinitionInformationTypeDef,
     DeleteConnectorDefinitionRequestRequestTypeDef,
     DeleteCoreDefinitionRequestRequestTypeDef,
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
+    DisassociateRoleFromGroupResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceAccessPolicyTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
+    GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
+    GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionRequestRequestTypeDef,
+    GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionRequestRequestTypeDef,
     GetDeploymentStatusRequestRequestTypeDef,
     GetDeviceDefinitionRequestRequestTypeDef,
+    GetDeviceDefinitionResponseTypeDef,
     GetDeviceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionRequestRequestTypeDef,
+    GetFunctionDefinitionResponseTypeDef,
     GetFunctionDefinitionVersionRequestRequestTypeDef,
     GetGroupCertificateAuthorityRequestRequestTypeDef,
+    GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
+    GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
+    GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
+    GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
+    GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
+    GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
     GroupOwnerSettingTypeDef,
-    PaginatorConfigTypeDef,
+    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
+    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
+    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
     VersionInformationTypeDef,
+    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
     ListConnectorDefinitionsRequestRequestTypeDef,
+    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     ListCoreDefinitionVersionsRequestRequestTypeDef,
+    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
     ListCoreDefinitionsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     ListDeviceDefinitionVersionsRequestRequestTypeDef,
+    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
     ListDeviceDefinitionsRequestRequestTypeDef,
+    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     ListFunctionDefinitionVersionsRequestRequestTypeDef,
+    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
     ListFunctionDefinitionsRequestRequestTypeDef,
     ListGroupCertificateAuthoritiesRequestRequestTypeDef,
+    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     ListGroupVersionsRequestRequestTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
+    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     ListLoggerDefinitionVersionsRequestRequestTypeDef,
+    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
     ListLoggerDefinitionsRequestRequestTypeDef,
+    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     ListResourceDefinitionVersionsRequestRequestTypeDef,
+    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
     ListResourceDefinitionsRequestRequestTypeDef,
+    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
+    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
+    ResetDeploymentsResponseTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
+    ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
+    StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
     UpdateFunctionDefinitionRequestRequestTypeDef,
     UpdateGroupCertificateConfigurationRequestRequestTypeDef,
+    UpdateGroupCertificateConfigurationResponseTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateLoggerDefinitionRequestRequestTypeDef,
     UpdateResourceDefinitionRequestRequestTypeDef,
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
-    AssociateRoleToGroupResponseTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
-    CreateConnectorDefinitionResponseTypeDef,
-    CreateConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionResponseTypeDef,
-    CreateCoreDefinitionVersionResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateDeviceDefinitionResponseTypeDef,
-    CreateDeviceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionResponseTypeDef,
-    CreateFunctionDefinitionVersionResponseTypeDef,
-    CreateGroupCertificateAuthorityResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateGroupVersionResponseTypeDef,
-    CreateLoggerDefinitionResponseTypeDef,
-    CreateLoggerDefinitionVersionResponseTypeDef,
-    CreateResourceDefinitionResponseTypeDef,
-    CreateResourceDefinitionVersionResponseTypeDef,
-    CreateSoftwareUpdateJobResponseTypeDef,
-    CreateSubscriptionDefinitionResponseTypeDef,
-    CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DisassociateRoleFromGroupResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAssociatedRoleResponseTypeDef,
-    GetConnectorDefinitionResponseTypeDef,
-    GetCoreDefinitionResponseTypeDef,
-    GetDeviceDefinitionResponseTypeDef,
-    GetFunctionDefinitionResponseTypeDef,
-    GetGroupCertificateAuthorityResponseTypeDef,
-    GetGroupCertificateConfigurationResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetLoggerDefinitionResponseTypeDef,
-    GetResourceDefinitionResponseTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
-    GetSubscriptionDefinitionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResetDeploymentsResponseTypeDef,
-    StartBulkDeploymentResponseTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
-    UpdateGroupCertificateConfigurationResponseTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionTypeDef,
@@ -560,33 +579,14 @@
     ListDeploymentsResponseTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
-    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
-    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
-    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
-    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
-    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
-    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
-    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
-    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
@@ -631,42 +631,42 @@
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

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/__init__.py` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/__init__.pyi` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/__main__.py` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Greengrass 1.26.59\nVersion:         1.26.59\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Greengrass 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/client.py` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/client.pyi` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/literals.py` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
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
@@ -151,21 +152,23 @@
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
@@ -244,14 +247,15 @@
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
@@ -262,14 +266,15 @@
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
@@ -305,14 +310,15 @@
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
@@ -331,16 +337,19 @@
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
@@ -420,18 +429,21 @@
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

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/literals.pyi` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
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
@@ -149,21 +150,23 @@
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
@@ -242,14 +245,15 @@
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
@@ -260,14 +264,15 @@
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
@@ -303,14 +308,15 @@
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
@@ -329,16 +335,19 @@
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
@@ -418,18 +427,21 @@
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

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/paginator.py` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,283 +118,283 @@
 class ListBulkDeploymentDetailedReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
     """
 
     def paginate(
-        self, *, BulkDeploymentId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BulkDeploymentId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBulkDeploymentDetailedReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
         """
 
 
 class ListBulkDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBulkDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
         """
 
 
 class ListConnectorDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ConnectorDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ConnectorDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConnectorDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
         """
 
 
 class ListConnectorDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConnectorDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
         """
 
 
 class ListCoreDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, CoreDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CoreDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoreDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
         """
 
 
 class ListCoreDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoreDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
         """
 
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
         """
 
 
 class ListDeviceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, DeviceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DeviceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
         """
 
 
 class ListDeviceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
         """
 
 
 class ListFunctionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, FunctionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
         """
 
 
 class ListFunctionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
         """
 
 
 class ListGroupVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
         """
 
 
 class ListLoggerDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, LoggerDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, LoggerDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLoggerDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
         """
 
 
 class ListLoggerDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLoggerDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
         """
 
 
 class ListResourceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ResourceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
         """
 
 
 class ListResourceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
         """
 
 
 class ListSubscriptionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, SubscriptionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SubscriptionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
         """
 
 
 class ListSubscriptionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
         """
```

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/paginator.pyi` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -115,265 +115,265 @@
 class ListBulkDeploymentDetailedReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
     """
 
     def paginate(
-        self, *, BulkDeploymentId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BulkDeploymentId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBulkDeploymentDetailedReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeploymentDetailedReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentdetailedreportspaginator)
         """
 
 class ListBulkDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBulkDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListBulkDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listbulkdeploymentspaginator)
         """
 
 class ListConnectorDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ConnectorDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ConnectorDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConnectorDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionversionspaginator)
         """
 
 class ListConnectorDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConnectorDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListConnectorDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listconnectordefinitionspaginator)
         """
 
 class ListCoreDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, CoreDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CoreDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoreDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionversionspaginator)
         """
 
 class ListCoreDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoreDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListCoreDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listcoredefinitionspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdeploymentspaginator)
         """
 
 class ListDeviceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, DeviceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DeviceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionversionspaginator)
         """
 
 class ListDeviceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListDeviceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listdevicedefinitionspaginator)
         """
 
 class ListFunctionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, FunctionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionversionspaginator)
         """
 
 class ListFunctionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListFunctionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listfunctiondefinitionspaginator)
         """
 
 class ListGroupVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
     """
 
     def paginate(
-        self, *, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroupVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupversionspaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listgroupspaginator)
         """
 
 class ListLoggerDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, LoggerDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, LoggerDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLoggerDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionversionspaginator)
         """
 
 class ListLoggerDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLoggerDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListLoggerDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listloggerdefinitionspaginator)
         """
 
 class ListResourceDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, ResourceDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionversionspaginator)
         """
 
 class ListResourceDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListResourceDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listresourcedefinitionspaginator)
         """
 
 class ListSubscriptionDefinitionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
     """
 
     def paginate(
-        self, *, SubscriptionDefinitionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SubscriptionDefinitionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionDefinitionVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionversionspaginator)
         """
 
 class ListSubscriptionDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSubscriptionDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Paginator.ListSubscriptionDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/paginators/#listsubscriptiondefinitionspaginator)
         """
```

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/type_defs.py` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,151 +35,170 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateRoleToGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateRoleToGroupResponseTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
     "ConnectivityInfoTypeDef",
     "ConnectorTypeDef",
     "CoreTypeDef",
+    "CreateConnectorDefinitionResponseTypeDef",
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    "CreateCoreDefinitionResponseTypeDef",
+    "CreateCoreDefinitionVersionResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateDeviceDefinitionResponseTypeDef",
     "DeviceTypeDef",
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    "CreateFunctionDefinitionResponseTypeDef",
+    "CreateFunctionDefinitionVersionResponseTypeDef",
     "CreateGroupCertificateAuthorityRequestRequestTypeDef",
+    "CreateGroupCertificateAuthorityResponseTypeDef",
     "GroupVersionTypeDef",
+    "CreateGroupResponseTypeDef",
     "CreateGroupVersionRequestRequestTypeDef",
+    "CreateGroupVersionResponseTypeDef",
+    "CreateLoggerDefinitionResponseTypeDef",
     "LoggerTypeDef",
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    "CreateResourceDefinitionResponseTypeDef",
+    "CreateResourceDefinitionVersionResponseTypeDef",
     "CreateSoftwareUpdateJobRequestRequestTypeDef",
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    "CreateSubscriptionDefinitionResponseTypeDef",
     "SubscriptionTypeDef",
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
     "DefinitionInformationTypeDef",
     "DeleteConnectorDefinitionRequestRequestTypeDef",
     "DeleteCoreDefinitionRequestRequestTypeDef",
     "DeleteDeviceDefinitionRequestRequestTypeDef",
     "DeleteFunctionDefinitionRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteLoggerDefinitionRequestRequestTypeDef",
     "DeleteResourceDefinitionRequestRequestTypeDef",
     "DeleteSubscriptionDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
     "DisassociateRoleFromGroupRequestRequestTypeDef",
+    "DisassociateRoleFromGroupResponseTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ResourceAccessPolicyTypeDef",
     "FunctionRunAsConfigTypeDef",
     "GetAssociatedRoleRequestRequestTypeDef",
+    "GetAssociatedRoleResponseTypeDef",
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetConnectorDefinitionRequestRequestTypeDef",
+    "GetConnectorDefinitionResponseTypeDef",
     "GetConnectorDefinitionVersionRequestRequestTypeDef",
     "GetCoreDefinitionRequestRequestTypeDef",
+    "GetCoreDefinitionResponseTypeDef",
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     "GetDeploymentStatusRequestRequestTypeDef",
     "GetDeviceDefinitionRequestRequestTypeDef",
+    "GetDeviceDefinitionResponseTypeDef",
     "GetDeviceDefinitionVersionRequestRequestTypeDef",
     "GetFunctionDefinitionRequestRequestTypeDef",
+    "GetFunctionDefinitionResponseTypeDef",
     "GetFunctionDefinitionVersionRequestRequestTypeDef",
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
+    "GetGroupCertificateAuthorityResponseTypeDef",
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
+    "GetGroupCertificateConfigurationResponseTypeDef",
     "GetGroupRequestRequestTypeDef",
+    "GetGroupResponseTypeDef",
     "GetGroupVersionRequestRequestTypeDef",
     "GetLoggerDefinitionRequestRequestTypeDef",
+    "GetLoggerDefinitionResponseTypeDef",
     "GetLoggerDefinitionVersionRequestRequestTypeDef",
     "GetResourceDefinitionRequestRequestTypeDef",
+    "GetResourceDefinitionResponseTypeDef",
     "GetResourceDefinitionVersionRequestRequestTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
     "GetSubscriptionDefinitionRequestRequestTypeDef",
+    "GetSubscriptionDefinitionResponseTypeDef",
     "GetSubscriptionDefinitionVersionRequestRequestTypeDef",
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     "GroupCertificateAuthorityPropertiesTypeDef",
     "GroupInformationTypeDef",
     "GroupOwnerSettingTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     "ListBulkDeploymentDetailedReportsRequestRequestTypeDef",
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     "ListBulkDeploymentsRequestRequestTypeDef",
+    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsRequestRequestTypeDef",
     "VersionInformationTypeDef",
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionsRequestRequestTypeDef",
+    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     "ListCoreDefinitionVersionsRequestRequestTypeDef",
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     "ListCoreDefinitionsRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     "ListDeviceDefinitionVersionsRequestRequestTypeDef",
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
     "ListDeviceDefinitionsRequestRequestTypeDef",
+    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
     "ListFunctionDefinitionVersionsRequestRequestTypeDef",
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
     "ListFunctionDefinitionsRequestRequestTypeDef",
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
+    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
     "ListGroupVersionsRequestRequestTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
+    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
     "ListLoggerDefinitionVersionsRequestRequestTypeDef",
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
     "ListLoggerDefinitionsRequestRequestTypeDef",
+    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
     "ListResourceDefinitionVersionsRequestRequestTypeDef",
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
     "ListResourceDefinitionsRequestRequestTypeDef",
+    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
+    "ResetDeploymentsResponseTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
+    "ResponseMetadataTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
+    "StartBulkDeploymentResponseTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
     "UpdateConnectorDefinitionRequestRequestTypeDef",
     "UpdateCoreDefinitionRequestRequestTypeDef",
     "UpdateDeviceDefinitionRequestRequestTypeDef",
     "UpdateFunctionDefinitionRequestRequestTypeDef",
     "UpdateGroupCertificateConfigurationRequestRequestTypeDef",
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateLoggerDefinitionRequestRequestTypeDef",
     "UpdateResourceDefinitionRequestRequestTypeDef",
     "UpdateSubscriptionDefinitionRequestRequestTypeDef",
-    "AssociateRoleToGroupResponseTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    "CreateConnectorDefinitionResponseTypeDef",
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    "CreateCoreDefinitionResponseTypeDef",
-    "CreateCoreDefinitionVersionResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateDeviceDefinitionResponseTypeDef",
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    "CreateFunctionDefinitionResponseTypeDef",
-    "CreateFunctionDefinitionVersionResponseTypeDef",
-    "CreateGroupCertificateAuthorityResponseTypeDef",
-    "CreateGroupResponseTypeDef",
-    "CreateGroupVersionResponseTypeDef",
-    "CreateLoggerDefinitionResponseTypeDef",
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    "CreateResourceDefinitionResponseTypeDef",
-    "CreateResourceDefinitionVersionResponseTypeDef",
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    "CreateSubscriptionDefinitionResponseTypeDef",
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
-    "DisassociateRoleFromGroupResponseTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAssociatedRoleResponseTypeDef",
-    "GetConnectorDefinitionResponseTypeDef",
-    "GetCoreDefinitionResponseTypeDef",
-    "GetDeviceDefinitionResponseTypeDef",
-    "GetFunctionDefinitionResponseTypeDef",
-    "GetGroupCertificateAuthorityResponseTypeDef",
-    "GetGroupCertificateConfigurationResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetLoggerDefinitionResponseTypeDef",
-    "GetResourceDefinitionResponseTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
-    "GetSubscriptionDefinitionResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResetDeploymentsResponseTypeDef",
-    "StartBulkDeploymentResponseTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ConnectorDefinitionVersionTypeDef",
@@ -204,33 +223,14 @@
     "ListDeploymentsResponseTypeDef",
     "FunctionDefaultExecutionConfigTypeDef",
     "FunctionExecutionConfigTypeDef",
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "LocalDeviceResourceDataTypeDef",
     "LocalVolumeResourceDataTypeDef",
-    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
-    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
-    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
-    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
-    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
-    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
-    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsResponseTypeDef",
     "ListCoreDefinitionVersionsResponseTypeDef",
     "ListDeviceDefinitionVersionsResponseTypeDef",
     "ListFunctionDefinitionVersionsResponseTypeDef",
     "ListGroupVersionsResponseTypeDef",
     "ListLoggerDefinitionVersionsResponseTypeDef",
     "ListResourceDefinitionVersionsResponseTypeDef",
@@ -271,32 +271,37 @@
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateRoleToGroupResponseTypeDef = TypedDict(
+    "AssociateRoleToGroupResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AssociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "RoleArn": str,
     },
 )
 
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BulkDeploymentMetricsTypeDef = TypedDict(
     "BulkDeploymentMetricsTypeDef",
     {
         "InvalidInputRecords": int,
         "RecordsProcessed": int,
         "RetryAttempts": int,
     },
@@ -370,14 +375,64 @@
 )
 
 
 class CoreTypeDef(_RequiredCoreTypeDef, _OptionalCoreTypeDef):
     pass
 
 
+CreateConnectorDefinitionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCoreDefinitionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "DeploymentType": DeploymentTypeType,
         "GroupId": str,
     },
 )
@@ -394,14 +449,37 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDeviceDefinitionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -415,14 +493,50 @@
 )
 
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
 
+CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFunctionDefinitionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
@@ -437,28 +551,50 @@
 class CreateGroupCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
 
+CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "CreateGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GroupVersionTypeDef = TypedDict(
     "GroupVersionTypeDef",
     {
         "ConnectorDefinitionVersionArn": str,
         "CoreDefinitionVersionArn": str,
         "DeviceDefinitionVersionArn": str,
         "FunctionDefinitionVersionArn": str,
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateGroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupVersionRequestRequestTypeDef = TypedDict(
@@ -480,14 +616,39 @@
 class CreateGroupVersionRequestRequestTypeDef(
     _RequiredCreateGroupVersionRequestRequestTypeDef,
     _OptionalCreateGroupVersionRequestRequestTypeDef,
 ):
     pass
 
 
+CreateGroupVersionResponseTypeDef = TypedDict(
+    "CreateGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLoggerDefinitionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredLoggerTypeDef = TypedDict(
     "_RequiredLoggerTypeDef",
     {
         "Component": LoggerComponentType,
         "Id": str,
         "Level": LoggerLevelType,
         "Type": LoggerTypeType,
@@ -502,14 +663,50 @@
 )
 
 
 class LoggerTypeDef(_RequiredLoggerTypeDef, _OptionalLoggerTypeDef):
     pass
 
 
+CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateResourceDefinitionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSoftwareUpdateJobRequestRequestTypeDef",
     {
         "S3UrlSignerRole": str,
         "SoftwareToUpdate": SoftwareToUpdateType,
         "UpdateTargets": Sequence[str],
         "UpdateTargetsArchitecture": UpdateTargetsArchitectureType,
@@ -529,24 +726,59 @@
 class CreateSoftwareUpdateJobRequestRequestTypeDef(
     _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef,
     _OptionalCreateSoftwareUpdateJobRequestRequestTypeDef,
 ):
     pass
 
 
+CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    {
+        "IotJobArn": str,
+        "IotJobId": str,
+        "PlatformSoftwareVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Id": str,
         "Source": str,
         "Subject": str,
         "Target": str,
     },
 )
 
+CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DefinitionInformationTypeDef = TypedDict(
     "DefinitionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "LastUpdatedTimestamp": str,
@@ -629,14 +861,37 @@
 DisassociateRoleFromGroupRequestRequestTypeDef = TypedDict(
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+DisassociateRoleFromGroupResponseTypeDef = TypedDict(
+    "DisassociateRoleFromGroupResponseTypeDef",
+    {
+        "DisassociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "DisassociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResourceAccessPolicyTypeDef = TypedDict(
     "_RequiredResourceAccessPolicyTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalResourceAccessPolicyTypeDef = TypedDict(
@@ -666,14 +921,23 @@
 GetAssociatedRoleRequestRequestTypeDef = TypedDict(
     "GetAssociatedRoleRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+GetAssociatedRoleResponseTypeDef = TypedDict(
+    "GetAssociatedRoleResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBulkDeploymentStatusRequestRequestTypeDef = TypedDict(
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -687,14 +951,29 @@
 GetConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "GetConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 
+GetConnectorDefinitionResponseTypeDef = TypedDict(
+    "GetConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
         "ConnectorDefinitionVersionId": str,
     },
 )
@@ -717,14 +996,29 @@
 GetCoreDefinitionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 
+GetCoreDefinitionResponseTypeDef = TypedDict(
+    "GetCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCoreDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
         "CoreDefinitionVersionId": str,
     },
 )
@@ -740,14 +1034,29 @@
 GetDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "GetDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 
+GetDeviceDefinitionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
         "DeviceDefinitionVersionId": str,
     },
 )
@@ -770,14 +1079,29 @@
 GetFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "GetFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 
+GetFunctionDefinitionResponseTypeDef = TypedDict(
+    "GetFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
         "FunctionDefinitionVersionId": str,
     },
 )
@@ -801,28 +1125,63 @@
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityId": str,
         "GroupId": str,
     },
 )
 
+GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "GetGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "GroupCertificateAuthorityId": str,
+        "PemEncodedCertificate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "GetGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupVersionRequestRequestTypeDef = TypedDict(
     "GetGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
         "GroupVersionId": str,
     },
 )
@@ -830,14 +1189,29 @@
 GetLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "GetLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 
+GetLoggerDefinitionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
         "LoggerDefinitionVersionId": str,
     },
 )
@@ -860,29 +1234,68 @@
 GetResourceDefinitionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 
+GetResourceDefinitionResponseTypeDef = TypedDict(
+    "GetResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionVersionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
         "ResourceDefinitionVersionId": str,
     },
 )
 
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 
+GetSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
         "SubscriptionDefinitionVersionId": str,
     },
 )
@@ -937,24 +1350,36 @@
     {
         "AutoAddGroupOwner": bool,
         "GroupOwner": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "BulkDeploymentId": str,
+    },
+)
+_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
+    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
@@ -970,23 +1395,53 @@
 class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef,
 ):
     pass
 
 
+ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBulkDeploymentsRequestRequestTypeDef = TypedDict(
     "ListBulkDeploymentsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    {
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
+    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConnectorDefinitionVersionsRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1013,23 +1468,53 @@
         "CreationTimestamp": str,
         "Id": str,
         "Version": str,
     },
     total=False,
 )
 
+ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConnectorDefinitionsRequestRequestTypeDef = TypedDict(
     "ListConnectorDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    {
+        "CoreDefinitionId": str,
+    },
+)
+_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
+    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCoreDefinitionVersionsRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1045,23 +1530,53 @@
 class ListCoreDefinitionVersionsRequestRequestTypeDef(
     _RequiredListCoreDefinitionVersionsRequestRequestTypeDef,
     _OptionalListCoreDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCoreDefinitionsRequestRequestTypeDef = TypedDict(
     "ListCoreDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1076,14 +1591,36 @@
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    {
+        "DeviceDefinitionId": str,
+    },
+)
+_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
+    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1099,23 +1636,53 @@
 class ListDeviceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeviceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
+    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionDefinitionVersionsRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1131,14 +1698,22 @@
 class ListFunctionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFunctionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1147,14 +1722,36 @@
 ListGroupCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
+    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGroupVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupVersionsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListGroupVersionsRequestRequestTypeDef = TypedDict(
@@ -1169,23 +1766,53 @@
 
 class ListGroupVersionsRequestRequestTypeDef(
     _RequiredListGroupVersionsRequestRequestTypeDef, _OptionalListGroupVersionsRequestRequestTypeDef
 ):
     pass
 
 
+ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "LoggerDefinitionId": str,
+    },
+)
+_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
+    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLoggerDefinitionVersionsRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1201,23 +1828,53 @@
 class ListLoggerDefinitionVersionsRequestRequestTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLoggerDefinitionsRequestRequestTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
+    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceDefinitionVersionsRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1233,23 +1890,53 @@
 class ListResourceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListResourceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListResourceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListResourceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "SubscriptionDefinitionId": str,
+    },
+)
+_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
+    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1265,14 +1952,22 @@
 class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSubscriptionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1281,14 +1976,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 _RequiredResetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredResetDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalResetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1303,14 +2016,23 @@
 
 class ResetDeploymentsRequestRequestTypeDef(
     _RequiredResetDeploymentsRequestRequestTypeDef, _OptionalResetDeploymentsRequestRequestTypeDef
 ):
     pass
 
 
+ResetDeploymentsResponseTypeDef = TypedDict(
+    "ResetDeploymentsResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SecretsManagerSecretResourceDataTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
@@ -1320,14 +2042,25 @@
     "ResourceDownloadOwnerSettingTypeDef",
     {
         "GroupOwner": str,
         "GroupPermission": PermissionType,
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
 _RequiredTelemetryConfigurationTypeDef = TypedDict(
     "_RequiredTelemetryConfigurationTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 _OptionalTelemetryConfigurationTypeDef = TypedDict(
@@ -1365,14 +2098,23 @@
 class StartBulkDeploymentRequestRequestTypeDef(
     _RequiredStartBulkDeploymentRequestRequestTypeDef,
     _OptionalStartBulkDeploymentRequestRequestTypeDef,
 ):
     pass
 
 
+StartBulkDeploymentResponseTypeDef = TypedDict(
+    "StartBulkDeploymentResponseTypeDef",
+    {
+        "BulkDeploymentArn": str,
+        "BulkDeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -1408,14 +2150,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "Message": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
@@ -1518,14 +2269,24 @@
 class UpdateGroupCertificateConfigurationRequestRequestTypeDef(
     _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef,
     _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupRequestRequestTypeDef = TypedDict(
@@ -1605,483 +2366,14 @@
 class UpdateSubscriptionDefinitionRequestRequestTypeDef(
     _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef,
     _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateRoleToGroupResponseTypeDef = TypedDict(
-    "AssociateRoleToGroupResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectorDefinitionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCoreDefinitionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeviceDefinitionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFunctionDefinitionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "CreateGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupVersionResponseTypeDef = TypedDict(
-    "CreateGroupVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLoggerDefinitionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResourceDefinitionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    {
-        "IotJobArn": str,
-        "IotJobId": str,
-        "PlatformSoftwareVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateRoleFromGroupResponseTypeDef = TypedDict(
-    "DisassociateRoleFromGroupResponseTypeDef",
-    {
-        "DisassociatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "DisassociatedAt": str,
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
-GetAssociatedRoleResponseTypeDef = TypedDict(
-    "GetAssociatedRoleResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetConnectorDefinitionResponseTypeDef = TypedDict(
-    "GetConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCoreDefinitionResponseTypeDef = TypedDict(
-    "GetCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeviceDefinitionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionDefinitionResponseTypeDef = TypedDict(
-    "GetFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "GetGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "GroupCertificateAuthorityId": str,
-        "PemEncodedCertificate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "GetGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLoggerDefinitionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourceDefinitionResponseTypeDef = TypedDict(
-    "GetResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
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
-ResetDeploymentsResponseTypeDef = TypedDict(
-    "ResetDeploymentsResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBulkDeploymentResponseTypeDef = TypedDict(
-    "StartBulkDeploymentResponseTypeDef",
-    {
-        "BulkDeploymentArn": str,
-        "BulkDeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "Message": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BulkDeploymentResultTypeDef = TypedDict(
     "BulkDeploymentResultTypeDef",
     {
         "CreatedAt": str,
         "DeploymentArn": str,
         "DeploymentId": str,
         "DeploymentStatus": str,
@@ -2098,45 +2390,45 @@
     {
         "BulkDeploymentMetrics": BulkDeploymentMetricsTypeDef,
         "BulkDeploymentStatus": BulkDeploymentStatusType,
         "CreatedAt": str,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentStatusResponseTypeDef = TypedDict(
     "GetDeploymentStatusResponseTypeDef",
     {
         "DeploymentStatus": str,
         "DeploymentType": DeploymentTypeType,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "UpdatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBulkDeploymentsResponseTypeDef = TypedDict(
     "ListBulkDeploymentsResponseTypeDef",
     {
         "BulkDeployments": List[BulkDeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
         "ConnectivityInfo": List[ConnectivityInfoTypeDef],
         "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ThingName": str,
@@ -2278,15 +2570,15 @@
     "GetGroupVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": GroupVersionTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
@@ -2349,78 +2641,78 @@
 )
 
 ListConnectorDefinitionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCoreDefinitionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceDefinitionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionDefinitionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggerDefinitionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceDefinitionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionDefinitionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionDefaultExecutionConfigTypeDef = TypedDict(
     "FunctionDefaultExecutionConfigTypeDef",
     {
         "IsolationMode": FunctionIsolationModeType,
@@ -2438,24 +2730,24 @@
     total=False,
 )
 
 ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     {
         "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocalDeviceResourceDataTypeDef = TypedDict(
     "LocalDeviceResourceDataTypeDef",
     {
         "GroupOwnerSetting": GroupOwnerSettingTypeDef,
@@ -2470,375 +2762,83 @@
         "DestinationPath": str,
         "GroupOwnerSetting": GroupOwnerSettingTypeDef,
         "SourcePath": str,
     },
     total=False,
 )
 
-_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    {
-        "BulkDeploymentId": str,
-    },
-)
-_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
-    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-):
-    pass
-
-
-ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
-    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "CoreDefinitionId": str,
-    },
-)
-_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
-    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "DeviceDefinitionId": str,
-    },
-)
-_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
-    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
-    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
-    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "LoggerDefinitionId": str,
-    },
-)
-_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
-    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
-    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "SubscriptionDefinitionId": str,
-    },
-)
-_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
-    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListConnectorDefinitionVersionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCoreDefinitionVersionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupVersionsResponseTypeDef = TypedDict(
     "ListGroupVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggerDefinitionVersionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3MachineLearningModelResourceDataTypeDef = TypedDict(
     "S3MachineLearningModelResourceDataTypeDef",
     {
         "DestinationPath": str,
@@ -2889,15 +2889,15 @@
 
 
 ListBulkDeploymentDetailedReportsResponseTypeDef = TypedDict(
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2913,15 +2913,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ConnectorDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2937,15 +2937,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": CoreDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateDeviceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2961,15 +2961,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": DeviceDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "CreateLoggerDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2984,15 +2984,15 @@
     "GetLoggerDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": LoggerDefinitionVersionTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3008,15 +3008,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": SubscriptionDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionDefaultConfigTypeDef = TypedDict(
     "FunctionDefaultConfigTypeDef",
     {
         "Execution": FunctionDefaultExecutionConfigTypeDef,
@@ -3037,25 +3037,27 @@
 
 ResourceDataContainerTypeDef = TypedDict(
     "ResourceDataContainerTypeDef",
     {
         "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
         "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
         "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
-        "SageMakerMachineLearningModelResourceData": SageMakerMachineLearningModelResourceDataTypeDef,
+        "SageMakerMachineLearningModelResourceData": (
+            SageMakerMachineLearningModelResourceDataTypeDef
+        ),
         "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataTypeDef,
     },
     total=False,
 )
 
 GetThingRuntimeConfigurationResponseTypeDef = TypedDict(
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "EncodingType": EncodingTypeType,
@@ -3178,15 +3180,15 @@
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ResourceDefinitionVersionTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateFunctionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3202,10 +3204,10 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": FunctionDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass/type_defs.pyi` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -34,151 +34,170 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateRoleToGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateRoleToGroupResponseTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
     "BulkDeploymentMetricsTypeDef",
     "ErrorDetailTypeDef",
     "BulkDeploymentTypeDef",
     "ConnectivityInfoTypeDef",
     "ConnectorTypeDef",
     "CoreTypeDef",
+    "CreateConnectorDefinitionResponseTypeDef",
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    "CreateCoreDefinitionResponseTypeDef",
+    "CreateCoreDefinitionVersionResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateDeviceDefinitionResponseTypeDef",
     "DeviceTypeDef",
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    "CreateFunctionDefinitionResponseTypeDef",
+    "CreateFunctionDefinitionVersionResponseTypeDef",
     "CreateGroupCertificateAuthorityRequestRequestTypeDef",
+    "CreateGroupCertificateAuthorityResponseTypeDef",
     "GroupVersionTypeDef",
+    "CreateGroupResponseTypeDef",
     "CreateGroupVersionRequestRequestTypeDef",
+    "CreateGroupVersionResponseTypeDef",
+    "CreateLoggerDefinitionResponseTypeDef",
     "LoggerTypeDef",
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    "CreateResourceDefinitionResponseTypeDef",
+    "CreateResourceDefinitionVersionResponseTypeDef",
     "CreateSoftwareUpdateJobRequestRequestTypeDef",
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    "CreateSubscriptionDefinitionResponseTypeDef",
     "SubscriptionTypeDef",
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
     "DefinitionInformationTypeDef",
     "DeleteConnectorDefinitionRequestRequestTypeDef",
     "DeleteCoreDefinitionRequestRequestTypeDef",
     "DeleteDeviceDefinitionRequestRequestTypeDef",
     "DeleteFunctionDefinitionRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteLoggerDefinitionRequestRequestTypeDef",
     "DeleteResourceDefinitionRequestRequestTypeDef",
     "DeleteSubscriptionDefinitionRequestRequestTypeDef",
     "DeploymentTypeDef",
     "DisassociateRoleFromGroupRequestRequestTypeDef",
+    "DisassociateRoleFromGroupResponseTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ResourceAccessPolicyTypeDef",
     "FunctionRunAsConfigTypeDef",
     "GetAssociatedRoleRequestRequestTypeDef",
+    "GetAssociatedRoleResponseTypeDef",
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetConnectorDefinitionRequestRequestTypeDef",
+    "GetConnectorDefinitionResponseTypeDef",
     "GetConnectorDefinitionVersionRequestRequestTypeDef",
     "GetCoreDefinitionRequestRequestTypeDef",
+    "GetCoreDefinitionResponseTypeDef",
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     "GetDeploymentStatusRequestRequestTypeDef",
     "GetDeviceDefinitionRequestRequestTypeDef",
+    "GetDeviceDefinitionResponseTypeDef",
     "GetDeviceDefinitionVersionRequestRequestTypeDef",
     "GetFunctionDefinitionRequestRequestTypeDef",
+    "GetFunctionDefinitionResponseTypeDef",
     "GetFunctionDefinitionVersionRequestRequestTypeDef",
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
+    "GetGroupCertificateAuthorityResponseTypeDef",
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
+    "GetGroupCertificateConfigurationResponseTypeDef",
     "GetGroupRequestRequestTypeDef",
+    "GetGroupResponseTypeDef",
     "GetGroupVersionRequestRequestTypeDef",
     "GetLoggerDefinitionRequestRequestTypeDef",
+    "GetLoggerDefinitionResponseTypeDef",
     "GetLoggerDefinitionVersionRequestRequestTypeDef",
     "GetResourceDefinitionRequestRequestTypeDef",
+    "GetResourceDefinitionResponseTypeDef",
     "GetResourceDefinitionVersionRequestRequestTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
     "GetSubscriptionDefinitionRequestRequestTypeDef",
+    "GetSubscriptionDefinitionResponseTypeDef",
     "GetSubscriptionDefinitionVersionRequestRequestTypeDef",
     "GetThingRuntimeConfigurationRequestRequestTypeDef",
     "GroupCertificateAuthorityPropertiesTypeDef",
     "GroupInformationTypeDef",
     "GroupOwnerSettingTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     "ListBulkDeploymentDetailedReportsRequestRequestTypeDef",
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
     "ListBulkDeploymentsRequestRequestTypeDef",
+    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsRequestRequestTypeDef",
     "VersionInformationTypeDef",
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionsRequestRequestTypeDef",
+    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
     "ListCoreDefinitionVersionsRequestRequestTypeDef",
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
     "ListCoreDefinitionsRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
     "ListDeviceDefinitionVersionsRequestRequestTypeDef",
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
     "ListDeviceDefinitionsRequestRequestTypeDef",
+    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
     "ListFunctionDefinitionVersionsRequestRequestTypeDef",
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
     "ListFunctionDefinitionsRequestRequestTypeDef",
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
+    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
     "ListGroupVersionsRequestRequestTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
+    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
     "ListLoggerDefinitionVersionsRequestRequestTypeDef",
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
     "ListLoggerDefinitionsRequestRequestTypeDef",
+    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
     "ListResourceDefinitionVersionsRequestRequestTypeDef",
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
     "ListResourceDefinitionsRequestRequestTypeDef",
+    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
     "ListSubscriptionDefinitionVersionsRequestRequestTypeDef",
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResetDeploymentsRequestRequestTypeDef",
+    "ResetDeploymentsResponseTypeDef",
     "SecretsManagerSecretResourceDataTypeDef",
     "ResourceDownloadOwnerSettingTypeDef",
+    "ResponseMetadataTypeDef",
     "TelemetryConfigurationTypeDef",
     "StartBulkDeploymentRequestRequestTypeDef",
+    "StartBulkDeploymentResponseTypeDef",
     "StopBulkDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TelemetryConfigurationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
     "UpdateConnectorDefinitionRequestRequestTypeDef",
     "UpdateCoreDefinitionRequestRequestTypeDef",
     "UpdateDeviceDefinitionRequestRequestTypeDef",
     "UpdateFunctionDefinitionRequestRequestTypeDef",
     "UpdateGroupCertificateConfigurationRequestRequestTypeDef",
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateLoggerDefinitionRequestRequestTypeDef",
     "UpdateResourceDefinitionRequestRequestTypeDef",
     "UpdateSubscriptionDefinitionRequestRequestTypeDef",
-    "AssociateRoleToGroupResponseTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    "CreateConnectorDefinitionResponseTypeDef",
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    "CreateCoreDefinitionResponseTypeDef",
-    "CreateCoreDefinitionVersionResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateDeviceDefinitionResponseTypeDef",
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    "CreateFunctionDefinitionResponseTypeDef",
-    "CreateFunctionDefinitionVersionResponseTypeDef",
-    "CreateGroupCertificateAuthorityResponseTypeDef",
-    "CreateGroupResponseTypeDef",
-    "CreateGroupVersionResponseTypeDef",
-    "CreateLoggerDefinitionResponseTypeDef",
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    "CreateResourceDefinitionResponseTypeDef",
-    "CreateResourceDefinitionVersionResponseTypeDef",
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    "CreateSubscriptionDefinitionResponseTypeDef",
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
-    "DisassociateRoleFromGroupResponseTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAssociatedRoleResponseTypeDef",
-    "GetConnectorDefinitionResponseTypeDef",
-    "GetCoreDefinitionResponseTypeDef",
-    "GetDeviceDefinitionResponseTypeDef",
-    "GetFunctionDefinitionResponseTypeDef",
-    "GetGroupCertificateAuthorityResponseTypeDef",
-    "GetGroupCertificateConfigurationResponseTypeDef",
-    "GetGroupResponseTypeDef",
-    "GetLoggerDefinitionResponseTypeDef",
-    "GetResourceDefinitionResponseTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
-    "GetSubscriptionDefinitionResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResetDeploymentsResponseTypeDef",
-    "StartBulkDeploymentResponseTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
     "BulkDeploymentResultTypeDef",
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ConnectorDefinitionVersionTypeDef",
@@ -203,33 +222,14 @@
     "ListDeploymentsResponseTypeDef",
     "FunctionDefaultExecutionConfigTypeDef",
     "FunctionExecutionConfigTypeDef",
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "LocalDeviceResourceDataTypeDef",
     "LocalVolumeResourceDataTypeDef",
-    "ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
-    "ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
-    "ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
-    "ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
-    "ListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    "ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
-    "ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
-    "ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
     "ListConnectorDefinitionVersionsResponseTypeDef",
     "ListCoreDefinitionVersionsResponseTypeDef",
     "ListDeviceDefinitionVersionsResponseTypeDef",
     "ListFunctionDefinitionVersionsResponseTypeDef",
     "ListGroupVersionsResponseTypeDef",
     "ListLoggerDefinitionVersionsResponseTypeDef",
     "ListResourceDefinitionVersionsResponseTypeDef",
@@ -270,32 +270,37 @@
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateRoleToGroupResponseTypeDef = TypedDict(
+    "AssociateRoleToGroupResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AssociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "RoleArn": str,
     },
 )
 
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BulkDeploymentMetricsTypeDef = TypedDict(
     "BulkDeploymentMetricsTypeDef",
     {
         "InvalidInputRecords": int,
         "RecordsProcessed": int,
         "RetryAttempts": int,
     },
@@ -365,14 +370,64 @@
     },
     total=False,
 )
 
 class CoreTypeDef(_RequiredCoreTypeDef, _OptionalCoreTypeDef):
     pass
 
+CreateConnectorDefinitionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateConnectorDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCoreDefinitionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateCoreDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "DeploymentType": DeploymentTypeType,
         "GroupId": str,
     },
 )
@@ -387,14 +442,37 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDeviceDefinitionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "CertificateArn": str,
         "Id": str,
         "ThingArn": str,
     },
@@ -406,14 +484,50 @@
     },
     total=False,
 )
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
+CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateDeviceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFunctionDefinitionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateFunctionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef = TypedDict(
@@ -426,28 +540,50 @@
 
 class CreateGroupCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateGroupCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateGroupCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "CreateGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GroupVersionTypeDef = TypedDict(
     "GroupVersionTypeDef",
     {
         "ConnectorDefinitionVersionArn": str,
         "CoreDefinitionVersionArn": str,
         "DeviceDefinitionVersionArn": str,
         "FunctionDefinitionVersionArn": str,
         "LoggerDefinitionVersionArn": str,
         "ResourceDefinitionVersionArn": str,
         "SubscriptionDefinitionVersionArn": str,
     },
     total=False,
 )
 
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateGroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalCreateGroupVersionRequestRequestTypeDef = TypedDict(
@@ -467,14 +603,39 @@
 
 class CreateGroupVersionRequestRequestTypeDef(
     _RequiredCreateGroupVersionRequestRequestTypeDef,
     _OptionalCreateGroupVersionRequestRequestTypeDef,
 ):
     pass
 
+CreateGroupVersionResponseTypeDef = TypedDict(
+    "CreateGroupVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateLoggerDefinitionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredLoggerTypeDef = TypedDict(
     "_RequiredLoggerTypeDef",
     {
         "Component": LoggerComponentType,
         "Id": str,
         "Level": LoggerLevelType,
         "Type": LoggerTypeType,
@@ -487,14 +648,50 @@
     },
     total=False,
 )
 
 class LoggerTypeDef(_RequiredLoggerTypeDef, _OptionalLoggerTypeDef):
     pass
 
+CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateLoggerDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateResourceDefinitionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateResourceDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSoftwareUpdateJobRequestRequestTypeDef",
     {
         "S3UrlSignerRole": str,
         "SoftwareToUpdate": SoftwareToUpdateType,
         "UpdateTargets": Sequence[str],
         "UpdateTargetsArchitecture": UpdateTargetsArchitectureType,
@@ -512,24 +709,59 @@
 
 class CreateSoftwareUpdateJobRequestRequestTypeDef(
     _RequiredCreateSoftwareUpdateJobRequestRequestTypeDef,
     _OptionalCreateSoftwareUpdateJobRequestRequestTypeDef,
 ):
     pass
 
+CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
+    "CreateSoftwareUpdateJobResponseTypeDef",
+    {
+        "IotJobArn": str,
+        "IotJobId": str,
+        "PlatformSoftwareVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "Id": str,
         "Source": str,
         "Subject": str,
         "Target": str,
     },
 )
 
+CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
+    "CreateSubscriptionDefinitionVersionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DefinitionInformationTypeDef = TypedDict(
     "DefinitionInformationTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Id": str,
         "LastUpdatedTimestamp": str,
@@ -612,14 +844,37 @@
 DisassociateRoleFromGroupRequestRequestTypeDef = TypedDict(
     "DisassociateRoleFromGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+DisassociateRoleFromGroupResponseTypeDef = TypedDict(
+    "DisassociateRoleFromGroupResponseTypeDef",
+    {
+        "DisassociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "DisassociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResourceAccessPolicyTypeDef = TypedDict(
     "_RequiredResourceAccessPolicyTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalResourceAccessPolicyTypeDef = TypedDict(
@@ -647,14 +902,23 @@
 GetAssociatedRoleRequestRequestTypeDef = TypedDict(
     "GetAssociatedRoleRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+GetAssociatedRoleResponseTypeDef = TypedDict(
+    "GetAssociatedRoleResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBulkDeploymentStatusRequestRequestTypeDef = TypedDict(
     "GetBulkDeploymentStatusRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -668,14 +932,29 @@
 GetConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "GetConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 
+GetConnectorDefinitionResponseTypeDef = TypedDict(
+    "GetConnectorDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectorDefinitionVersionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
         "ConnectorDefinitionVersionId": str,
     },
 )
@@ -696,14 +975,29 @@
 GetCoreDefinitionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 
+GetCoreDefinitionResponseTypeDef = TypedDict(
+    "GetCoreDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCoreDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetCoreDefinitionVersionRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
         "CoreDefinitionVersionId": str,
     },
 )
@@ -719,14 +1013,29 @@
 GetDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "GetDeviceDefinitionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 
+GetDeviceDefinitionResponseTypeDef = TypedDict(
+    "GetDeviceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDeviceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceDefinitionVersionRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
         "DeviceDefinitionVersionId": str,
     },
 )
@@ -747,14 +1056,29 @@
 GetFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "GetFunctionDefinitionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 
+GetFunctionDefinitionResponseTypeDef = TypedDict(
+    "GetFunctionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFunctionDefinitionVersionRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
         "FunctionDefinitionVersionId": str,
     },
 )
@@ -776,28 +1100,63 @@
     "GetGroupCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityId": str,
         "GroupId": str,
     },
 )
 
+GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
+    "GetGroupCertificateAuthorityResponseTypeDef",
+    {
+        "GroupCertificateAuthorityArn": str,
+        "GroupCertificateAuthorityId": str,
+        "PemEncodedCertificate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupCertificateConfigurationRequestRequestTypeDef = TypedDict(
     "GetGroupCertificateConfigurationRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "GetGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupVersionRequestRequestTypeDef = TypedDict(
     "GetGroupVersionRequestRequestTypeDef",
     {
         "GroupId": str,
         "GroupVersionId": str,
     },
 )
@@ -805,14 +1164,29 @@
 GetLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "GetLoggerDefinitionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 
+GetLoggerDefinitionResponseTypeDef = TypedDict(
+    "GetLoggerDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
         "LoggerDefinitionVersionId": str,
     },
 )
@@ -833,29 +1207,68 @@
 GetResourceDefinitionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 
+GetResourceDefinitionResponseTypeDef = TypedDict(
+    "GetResourceDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
     "GetResourceDefinitionVersionRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
         "ResourceDefinitionVersionId": str,
     },
 )
 
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "AssociatedAt": str,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionDefinitionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 
+GetSubscriptionDefinitionResponseTypeDef = TypedDict(
+    "GetSubscriptionDefinitionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTimestamp": str,
+        "Id": str,
+        "LastUpdatedTimestamp": str,
+        "LatestVersion": str,
+        "LatestVersionArn": str,
+        "Name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSubscriptionDefinitionVersionRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
         "SubscriptionDefinitionVersionId": str,
     },
 )
@@ -908,24 +1321,34 @@
     {
         "AutoAddGroupOwner": bool,
         "GroupOwner": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "BulkDeploymentId": str,
+    },
+)
+_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
+    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
+    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef = TypedDict(
@@ -939,23 +1362,51 @@
 
 class ListBulkDeploymentDetailedReportsRequestRequestTypeDef(
     _RequiredListBulkDeploymentDetailedReportsRequestRequestTypeDef,
     _OptionalListBulkDeploymentDetailedReportsRequestRequestTypeDef,
 ):
     pass
 
+ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
+    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBulkDeploymentsRequestRequestTypeDef = TypedDict(
     "ListBulkDeploymentsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    {
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
+    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConnectorDefinitionVersionsRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalListConnectorDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -980,23 +1431,51 @@
         "CreationTimestamp": str,
         "Id": str,
         "Version": str,
     },
     total=False,
 )
 
+ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
+    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConnectorDefinitionsRequestRequestTypeDef = TypedDict(
     "ListConnectorDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    {
+        "CoreDefinitionId": str,
+    },
+)
+_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
+    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCoreDefinitionVersionsRequestRequestTypeDef",
     {
         "CoreDefinitionId": str,
     },
 )
 _OptionalListCoreDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1010,23 +1489,51 @@
 
 class ListCoreDefinitionVersionsRequestRequestTypeDef(
     _RequiredListCoreDefinitionVersionsRequestRequestTypeDef,
     _OptionalListCoreDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
+    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCoreDefinitionsRequestRequestTypeDef = TypedDict(
     "ListCoreDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1039,14 +1546,34 @@
 )
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    {
+        "DeviceDefinitionId": str,
+    },
+)
+_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
+    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceDefinitionVersionsRequestRequestTypeDef",
     {
         "DeviceDefinitionId": str,
     },
 )
 _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1060,23 +1587,51 @@
 
 class ListDeviceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListDeviceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListDeviceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
+    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeviceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListDeviceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
+    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionDefinitionVersionsRequestRequestTypeDef",
     {
         "FunctionDefinitionId": str,
     },
 )
 _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1090,14 +1645,22 @@
 
 class ListFunctionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListFunctionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListFunctionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
+    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFunctionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListFunctionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1106,14 +1669,34 @@
 ListGroupCertificateAuthoritiesRequestRequestTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 
+_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
+    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListGroupVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupVersionsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalListGroupVersionsRequestRequestTypeDef = TypedDict(
@@ -1126,23 +1709,51 @@
 )
 
 class ListGroupVersionsRequestRequestTypeDef(
     _RequiredListGroupVersionsRequestRequestTypeDef, _OptionalListGroupVersionsRequestRequestTypeDef
 ):
     pass
 
+ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "LoggerDefinitionId": str,
+    },
+)
+_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
+    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLoggerDefinitionVersionsRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
     },
 )
 _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1156,23 +1767,51 @@
 
 class ListLoggerDefinitionVersionsRequestRequestTypeDef(
     _RequiredListLoggerDefinitionVersionsRequestRequestTypeDef,
     _OptionalListLoggerDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
+    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLoggerDefinitionsRequestRequestTypeDef = TypedDict(
     "ListLoggerDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
+    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceDefinitionVersionsRequestRequestTypeDef",
     {
         "ResourceDefinitionId": str,
     },
 )
 _OptionalListResourceDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1186,23 +1825,51 @@
 
 class ListResourceDefinitionVersionsRequestRequestTypeDef(
     _RequiredListResourceDefinitionVersionsRequestRequestTypeDef,
     _OptionalListResourceDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
+    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResourceDefinitionsRequestRequestTypeDef = TypedDict(
     "ListResourceDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "SubscriptionDefinitionId": str,
+    },
+)
+_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
+    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef",
     {
         "SubscriptionDefinitionId": str,
     },
 )
 _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef = TypedDict(
@@ -1216,14 +1883,22 @@
 
 class ListSubscriptionDefinitionVersionsRequestRequestTypeDef(
     _RequiredListSubscriptionDefinitionVersionsRequestRequestTypeDef,
     _OptionalListSubscriptionDefinitionVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSubscriptionDefinitionsRequestRequestTypeDef = TypedDict(
     "ListSubscriptionDefinitionsRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1232,14 +1907,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 _RequiredResetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredResetDeploymentsRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalResetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1252,14 +1945,23 @@
 )
 
 class ResetDeploymentsRequestRequestTypeDef(
     _RequiredResetDeploymentsRequestRequestTypeDef, _OptionalResetDeploymentsRequestRequestTypeDef
 ):
     pass
 
+ResetDeploymentsResponseTypeDef = TypedDict(
+    "ResetDeploymentsResponseTypeDef",
+    {
+        "DeploymentArn": str,
+        "DeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SecretsManagerSecretResourceDataTypeDef = TypedDict(
     "SecretsManagerSecretResourceDataTypeDef",
     {
         "ARN": str,
         "AdditionalStagingLabelsToDownload": Sequence[str],
     },
     total=False,
@@ -1269,14 +1971,25 @@
     "ResourceDownloadOwnerSettingTypeDef",
     {
         "GroupOwner": str,
         "GroupPermission": PermissionType,
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
 _RequiredTelemetryConfigurationTypeDef = TypedDict(
     "_RequiredTelemetryConfigurationTypeDef",
     {
         "Telemetry": TelemetryType,
     },
 )
 _OptionalTelemetryConfigurationTypeDef = TypedDict(
@@ -1310,14 +2023,23 @@
 
 class StartBulkDeploymentRequestRequestTypeDef(
     _RequiredStartBulkDeploymentRequestRequestTypeDef,
     _OptionalStartBulkDeploymentRequestRequestTypeDef,
 ):
     pass
 
+StartBulkDeploymentResponseTypeDef = TypedDict(
+    "StartBulkDeploymentResponseTypeDef",
+    {
+        "BulkDeploymentArn": str,
+        "BulkDeploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopBulkDeploymentRequestRequestTypeDef = TypedDict(
     "StopBulkDeploymentRequestRequestTypeDef",
     {
         "BulkDeploymentId": str,
     },
 )
 
@@ -1351,14 +2073,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "Message": str,
+        "Version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorDefinitionRequestRequestTypeDef",
     {
         "ConnectorDefinitionId": str,
     },
 )
 _OptionalUpdateConnectorDefinitionRequestRequestTypeDef = TypedDict(
@@ -1451,14 +2182,24 @@
 
 class UpdateGroupCertificateConfigurationRequestRequestTypeDef(
     _RequiredUpdateGroupCertificateConfigurationRequestRequestTypeDef,
     _OptionalUpdateGroupCertificateConfigurationRequestRequestTypeDef,
 ):
     pass
 
+UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
+    "UpdateGroupCertificateConfigurationResponseTypeDef",
+    {
+        "CertificateAuthorityExpiryInMilliseconds": str,
+        "CertificateExpiryInMilliseconds": str,
+        "GroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupId": str,
     },
 )
 _OptionalUpdateGroupRequestRequestTypeDef = TypedDict(
@@ -1530,483 +2271,14 @@
 
 class UpdateSubscriptionDefinitionRequestRequestTypeDef(
     _RequiredUpdateSubscriptionDefinitionRequestRequestTypeDef,
     _OptionalUpdateSubscriptionDefinitionRequestRequestTypeDef,
 ):
     pass
 
-AssociateRoleToGroupResponseTypeDef = TypedDict(
-    "AssociateRoleToGroupResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectorDefinitionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectorDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateConnectorDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCoreDefinitionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCoreDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateCoreDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeviceDefinitionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeviceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateDeviceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFunctionDefinitionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFunctionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateFunctionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "CreateGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupVersionResponseTypeDef = TypedDict(
-    "CreateGroupVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLoggerDefinitionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLoggerDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateLoggerDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResourceDefinitionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResourceDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateResourceDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSoftwareUpdateJobResponseTypeDef = TypedDict(
-    "CreateSoftwareUpdateJobResponseTypeDef",
-    {
-        "IotJobArn": str,
-        "IotJobId": str,
-        "PlatformSoftwareVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
-    "CreateSubscriptionDefinitionVersionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateRoleFromGroupResponseTypeDef = TypedDict(
-    "DisassociateRoleFromGroupResponseTypeDef",
-    {
-        "DisassociatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "DisassociatedAt": str,
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
-GetAssociatedRoleResponseTypeDef = TypedDict(
-    "GetAssociatedRoleResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetConnectorDefinitionResponseTypeDef = TypedDict(
-    "GetConnectorDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCoreDefinitionResponseTypeDef = TypedDict(
-    "GetCoreDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeviceDefinitionResponseTypeDef = TypedDict(
-    "GetDeviceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionDefinitionResponseTypeDef = TypedDict(
-    "GetFunctionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupCertificateAuthorityResponseTypeDef = TypedDict(
-    "GetGroupCertificateAuthorityResponseTypeDef",
-    {
-        "GroupCertificateAuthorityArn": str,
-        "GroupCertificateAuthorityId": str,
-        "PemEncodedCertificate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "GetGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupResponseTypeDef = TypedDict(
-    "GetGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLoggerDefinitionResponseTypeDef = TypedDict(
-    "GetLoggerDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourceDefinitionResponseTypeDef = TypedDict(
-    "GetResourceDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "AssociatedAt": str,
-        "RoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSubscriptionDefinitionResponseTypeDef = TypedDict(
-    "GetSubscriptionDefinitionResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTimestamp": str,
-        "Id": str,
-        "LastUpdatedTimestamp": str,
-        "LatestVersion": str,
-        "LatestVersionArn": str,
-        "Name": str,
-        "tags": Dict[str, str],
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
-ResetDeploymentsResponseTypeDef = TypedDict(
-    "ResetDeploymentsResponseTypeDef",
-    {
-        "DeploymentArn": str,
-        "DeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBulkDeploymentResponseTypeDef = TypedDict(
-    "StartBulkDeploymentResponseTypeDef",
-    {
-        "BulkDeploymentArn": str,
-        "BulkDeploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "Message": str,
-        "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGroupCertificateConfigurationResponseTypeDef = TypedDict(
-    "UpdateGroupCertificateConfigurationResponseTypeDef",
-    {
-        "CertificateAuthorityExpiryInMilliseconds": str,
-        "CertificateExpiryInMilliseconds": str,
-        "GroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BulkDeploymentResultTypeDef = TypedDict(
     "BulkDeploymentResultTypeDef",
     {
         "CreatedAt": str,
         "DeploymentArn": str,
         "DeploymentId": str,
         "DeploymentStatus": str,
@@ -2023,45 +2295,45 @@
     {
         "BulkDeploymentMetrics": BulkDeploymentMetricsTypeDef,
         "BulkDeploymentStatus": BulkDeploymentStatusType,
         "CreatedAt": str,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeploymentStatusResponseTypeDef = TypedDict(
     "GetDeploymentStatusResponseTypeDef",
     {
         "DeploymentStatus": str,
         "DeploymentType": DeploymentTypeType,
         "ErrorDetails": List[ErrorDetailTypeDef],
         "ErrorMessage": str,
         "UpdatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBulkDeploymentsResponseTypeDef = TypedDict(
     "ListBulkDeploymentsResponseTypeDef",
     {
         "BulkDeployments": List[BulkDeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
         "ConnectivityInfo": List[ConnectivityInfoTypeDef],
         "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectivityInfoRequestRequestTypeDef",
     {
         "ThingName": str,
@@ -2193,15 +2465,15 @@
     "GetGroupVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": GroupVersionTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoggerDefinitionVersionRequestRequestTypeDef",
     {
         "LoggerDefinitionId": str,
@@ -2260,78 +2532,78 @@
 )
 
 ListConnectorDefinitionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCoreDefinitionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceDefinitionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionDefinitionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggerDefinitionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceDefinitionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionDefinitionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionsResponseTypeDef",
     {
         "Definitions": List[DefinitionInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionDefaultExecutionConfigTypeDef = TypedDict(
     "FunctionDefaultExecutionConfigTypeDef",
     {
         "IsolationMode": FunctionIsolationModeType,
@@ -2349,24 +2621,24 @@
     total=False,
 )
 
 ListGroupCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListGroupCertificateAuthoritiesResponseTypeDef",
     {
         "GroupCertificateAuthorities": List[GroupCertificateAuthorityPropertiesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocalDeviceResourceDataTypeDef = TypedDict(
     "LocalDeviceResourceDataTypeDef",
     {
         "GroupOwnerSetting": GroupOwnerSettingTypeDef,
@@ -2381,355 +2653,83 @@
         "DestinationPath": str,
         "GroupOwnerSetting": GroupOwnerSettingTypeDef,
         "SourcePath": str,
     },
     total=False,
 )
 
-_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    {
-        "BulkDeploymentId": str,
-    },
-)
-_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef = TypedDict(
-    "_OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef(
-    _RequiredListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    _OptionalListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-):
-    pass
-
-ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef = TypedDict(
-    "ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef(
-    _RequiredListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    _OptionalListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef = TypedDict(
-    "ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "CoreDefinitionId": str,
-    },
-)
-_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef(
-    _RequiredListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    _OptionalListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef = TypedDict(
-    "ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "DeviceDefinitionId": str,
-    },
-)
-_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef(
-    _RequiredListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    _OptionalListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef = TypedDict(
-    "ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef(
-    _RequiredListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    _OptionalListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef = TypedDict(
-    "ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListGroupVersionsRequestListGroupVersionsPaginateTypeDef(
-    _RequiredListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    _OptionalListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-):
-    pass
-
-ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "LoggerDefinitionId": str,
-    },
-)
-_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef(
-    _RequiredListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    _OptionalListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef = TypedDict(
-    "ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef(
-    _RequiredListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    _OptionalListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef = TypedDict(
-    "ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "SubscriptionDefinitionId": str,
-    },
-)
-_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef(
-    _RequiredListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    _OptionalListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-):
-    pass
-
-ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListConnectorDefinitionVersionsResponseTypeDef = TypedDict(
     "ListConnectorDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCoreDefinitionVersionsResponseTypeDef = TypedDict(
     "ListCoreDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeviceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListDeviceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListFunctionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupVersionsResponseTypeDef = TypedDict(
     "ListGroupVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLoggerDefinitionVersionsResponseTypeDef = TypedDict(
     "ListLoggerDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceDefinitionVersionsResponseTypeDef = TypedDict(
     "ListResourceDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSubscriptionDefinitionVersionsResponseTypeDef = TypedDict(
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3MachineLearningModelResourceDataTypeDef = TypedDict(
     "S3MachineLearningModelResourceDataTypeDef",
     {
         "DestinationPath": str,
@@ -2778,15 +2778,15 @@
     pass
 
 ListBulkDeploymentDetailedReportsResponseTypeDef = TypedDict(
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     {
         "Deployments": List[BulkDeploymentResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2802,15 +2802,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ConnectorDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2826,15 +2826,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": CoreDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDeviceDefinitionRequestRequestTypeDef = TypedDict(
     "CreateDeviceDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2850,15 +2850,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": DeviceDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoggerDefinitionRequestRequestTypeDef = TypedDict(
     "CreateLoggerDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2873,15 +2873,15 @@
     "GetLoggerDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": LoggerDefinitionVersionTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSubscriptionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -2897,15 +2897,15 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": SubscriptionDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionDefaultConfigTypeDef = TypedDict(
     "FunctionDefaultConfigTypeDef",
     {
         "Execution": FunctionDefaultExecutionConfigTypeDef,
@@ -2926,25 +2926,27 @@
 
 ResourceDataContainerTypeDef = TypedDict(
     "ResourceDataContainerTypeDef",
     {
         "LocalDeviceResourceData": LocalDeviceResourceDataTypeDef,
         "LocalVolumeResourceData": LocalVolumeResourceDataTypeDef,
         "S3MachineLearningModelResourceData": S3MachineLearningModelResourceDataTypeDef,
-        "SageMakerMachineLearningModelResourceData": SageMakerMachineLearningModelResourceDataTypeDef,
+        "SageMakerMachineLearningModelResourceData": (
+            SageMakerMachineLearningModelResourceDataTypeDef
+        ),
         "SecretsManagerSecretResourceData": SecretsManagerSecretResourceDataTypeDef,
     },
     total=False,
 )
 
 GetThingRuntimeConfigurationResponseTypeDef = TypedDict(
     "GetThingRuntimeConfigurationResponseTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "EncodingType": EncodingTypeType,
@@ -3061,15 +3063,15 @@
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ResourceDefinitionVersionTypeDef,
         "Id": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFunctionDefinitionRequestRequestTypeDef = TypedDict(
     "CreateFunctionDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
@@ -3085,10 +3087,10 @@
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": FunctionDefinitionVersionTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/PKG-INFO` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.26.59
-Summary: Type annotations for boto3.Greengrass 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Greengrass 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrass?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,151 +423,170 @@
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     BulkDeploymentMetricsTypeDef,
     ErrorDetailTypeDef,
     BulkDeploymentTypeDef,
     ConnectivityInfoTypeDef,
     ConnectorTypeDef,
     CoreTypeDef,
+    CreateConnectorDefinitionResponseTypeDef,
+    CreateConnectorDefinitionVersionResponseTypeDef,
+    CreateCoreDefinitionResponseTypeDef,
+    CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateDeviceDefinitionResponseTypeDef,
     DeviceTypeDef,
+    CreateDeviceDefinitionVersionResponseTypeDef,
+    CreateFunctionDefinitionResponseTypeDef,
+    CreateFunctionDefinitionVersionResponseTypeDef,
     CreateGroupCertificateAuthorityRequestRequestTypeDef,
+    CreateGroupCertificateAuthorityResponseTypeDef,
     GroupVersionTypeDef,
+    CreateGroupResponseTypeDef,
     CreateGroupVersionRequestRequestTypeDef,
+    CreateGroupVersionResponseTypeDef,
+    CreateLoggerDefinitionResponseTypeDef,
     LoggerTypeDef,
+    CreateLoggerDefinitionVersionResponseTypeDef,
+    CreateResourceDefinitionResponseTypeDef,
+    CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobRequestRequestTypeDef,
+    CreateSoftwareUpdateJobResponseTypeDef,
+    CreateSubscriptionDefinitionResponseTypeDef,
     SubscriptionTypeDef,
+    CreateSubscriptionDefinitionVersionResponseTypeDef,
     DefinitionInformationTypeDef,
     DeleteConnectorDefinitionRequestRequestTypeDef,
     DeleteCoreDefinitionRequestRequestTypeDef,
     DeleteDeviceDefinitionRequestRequestTypeDef,
     DeleteFunctionDefinitionRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteLoggerDefinitionRequestRequestTypeDef,
     DeleteResourceDefinitionRequestRequestTypeDef,
     DeleteSubscriptionDefinitionRequestRequestTypeDef,
     DeploymentTypeDef,
     DisassociateRoleFromGroupRequestRequestTypeDef,
+    DisassociateRoleFromGroupResponseTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceAccessPolicyTypeDef,
     FunctionRunAsConfigTypeDef,
     GetAssociatedRoleRequestRequestTypeDef,
+    GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusRequestRequestTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetConnectorDefinitionRequestRequestTypeDef,
+    GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionRequestRequestTypeDef,
+    GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionRequestRequestTypeDef,
     GetDeploymentStatusRequestRequestTypeDef,
     GetDeviceDefinitionRequestRequestTypeDef,
+    GetDeviceDefinitionResponseTypeDef,
     GetDeviceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionRequestRequestTypeDef,
+    GetFunctionDefinitionResponseTypeDef,
     GetFunctionDefinitionVersionRequestRequestTypeDef,
     GetGroupCertificateAuthorityRequestRequestTypeDef,
+    GetGroupCertificateAuthorityResponseTypeDef,
     GetGroupCertificateConfigurationRequestRequestTypeDef,
+    GetGroupCertificateConfigurationResponseTypeDef,
     GetGroupRequestRequestTypeDef,
+    GetGroupResponseTypeDef,
     GetGroupVersionRequestRequestTypeDef,
     GetLoggerDefinitionRequestRequestTypeDef,
+    GetLoggerDefinitionResponseTypeDef,
     GetLoggerDefinitionVersionRequestRequestTypeDef,
     GetResourceDefinitionRequestRequestTypeDef,
+    GetResourceDefinitionResponseTypeDef,
     GetResourceDefinitionVersionRequestRequestTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
     GetSubscriptionDefinitionRequestRequestTypeDef,
+    GetSubscriptionDefinitionResponseTypeDef,
     GetSubscriptionDefinitionVersionRequestRequestTypeDef,
     GetThingRuntimeConfigurationRequestRequestTypeDef,
     GroupCertificateAuthorityPropertiesTypeDef,
     GroupInformationTypeDef,
     GroupOwnerSettingTypeDef,
-    PaginatorConfigTypeDef,
+    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
     ListBulkDeploymentDetailedReportsRequestRequestTypeDef,
+    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
     ListBulkDeploymentsRequestRequestTypeDef,
+    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
     ListConnectorDefinitionVersionsRequestRequestTypeDef,
     VersionInformationTypeDef,
+    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
     ListConnectorDefinitionsRequestRequestTypeDef,
+    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
     ListCoreDefinitionVersionsRequestRequestTypeDef,
+    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
     ListCoreDefinitionsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
     ListDeviceDefinitionVersionsRequestRequestTypeDef,
+    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
     ListDeviceDefinitionsRequestRequestTypeDef,
+    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
     ListFunctionDefinitionVersionsRequestRequestTypeDef,
+    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
     ListFunctionDefinitionsRequestRequestTypeDef,
     ListGroupCertificateAuthoritiesRequestRequestTypeDef,
+    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
     ListGroupVersionsRequestRequestTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
+    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
     ListLoggerDefinitionVersionsRequestRequestTypeDef,
+    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
     ListLoggerDefinitionsRequestRequestTypeDef,
+    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
     ListResourceDefinitionVersionsRequestRequestTypeDef,
+    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
     ListResourceDefinitionsRequestRequestTypeDef,
+    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
     ListSubscriptionDefinitionVersionsRequestRequestTypeDef,
+    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListSubscriptionDefinitionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResetDeploymentsRequestRequestTypeDef,
+    ResetDeploymentsResponseTypeDef,
     SecretsManagerSecretResourceDataTypeDef,
     ResourceDownloadOwnerSettingTypeDef,
+    ResponseMetadataTypeDef,
     TelemetryConfigurationTypeDef,
     StartBulkDeploymentRequestRequestTypeDef,
+    StartBulkDeploymentResponseTypeDef,
     StopBulkDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     UpdateConnectorDefinitionRequestRequestTypeDef,
     UpdateCoreDefinitionRequestRequestTypeDef,
     UpdateDeviceDefinitionRequestRequestTypeDef,
     UpdateFunctionDefinitionRequestRequestTypeDef,
     UpdateGroupCertificateConfigurationRequestRequestTypeDef,
+    UpdateGroupCertificateConfigurationResponseTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateLoggerDefinitionRequestRequestTypeDef,
     UpdateResourceDefinitionRequestRequestTypeDef,
     UpdateSubscriptionDefinitionRequestRequestTypeDef,
-    AssociateRoleToGroupResponseTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
-    CreateConnectorDefinitionResponseTypeDef,
-    CreateConnectorDefinitionVersionResponseTypeDef,
-    CreateCoreDefinitionResponseTypeDef,
-    CreateCoreDefinitionVersionResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateDeviceDefinitionResponseTypeDef,
-    CreateDeviceDefinitionVersionResponseTypeDef,
-    CreateFunctionDefinitionResponseTypeDef,
-    CreateFunctionDefinitionVersionResponseTypeDef,
-    CreateGroupCertificateAuthorityResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateGroupVersionResponseTypeDef,
-    CreateLoggerDefinitionResponseTypeDef,
-    CreateLoggerDefinitionVersionResponseTypeDef,
-    CreateResourceDefinitionResponseTypeDef,
-    CreateResourceDefinitionVersionResponseTypeDef,
-    CreateSoftwareUpdateJobResponseTypeDef,
-    CreateSubscriptionDefinitionResponseTypeDef,
-    CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DisassociateRoleFromGroupResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAssociatedRoleResponseTypeDef,
-    GetConnectorDefinitionResponseTypeDef,
-    GetCoreDefinitionResponseTypeDef,
-    GetDeviceDefinitionResponseTypeDef,
-    GetFunctionDefinitionResponseTypeDef,
-    GetGroupCertificateAuthorityResponseTypeDef,
-    GetGroupCertificateConfigurationResponseTypeDef,
-    GetGroupResponseTypeDef,
-    GetLoggerDefinitionResponseTypeDef,
-    GetResourceDefinitionResponseTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
-    GetSubscriptionDefinitionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResetDeploymentsResponseTypeDef,
-    StartBulkDeploymentResponseTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
-    UpdateGroupCertificateConfigurationResponseTypeDef,
     BulkDeploymentResultTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionTypeDef,
@@ -592,33 +611,14 @@
     ListDeploymentsResponseTypeDef,
     FunctionDefaultExecutionConfigTypeDef,
     FunctionExecutionConfigTypeDef,
     ListGroupCertificateAuthoritiesResponseTypeDef,
     ListGroupsResponseTypeDef,
     LocalDeviceResourceDataTypeDef,
     LocalVolumeResourceDataTypeDef,
-    ListBulkDeploymentDetailedReportsRequestListBulkDeploymentDetailedReportsPaginateTypeDef,
-    ListBulkDeploymentsRequestListBulkDeploymentsPaginateTypeDef,
-    ListConnectorDefinitionVersionsRequestListConnectorDefinitionVersionsPaginateTypeDef,
-    ListConnectorDefinitionsRequestListConnectorDefinitionsPaginateTypeDef,
-    ListCoreDefinitionVersionsRequestListCoreDefinitionVersionsPaginateTypeDef,
-    ListCoreDefinitionsRequestListCoreDefinitionsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListDeviceDefinitionVersionsRequestListDeviceDefinitionVersionsPaginateTypeDef,
-    ListDeviceDefinitionsRequestListDeviceDefinitionsPaginateTypeDef,
-    ListFunctionDefinitionVersionsRequestListFunctionDefinitionVersionsPaginateTypeDef,
-    ListFunctionDefinitionsRequestListFunctionDefinitionsPaginateTypeDef,
-    ListGroupVersionsRequestListGroupVersionsPaginateTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
-    ListLoggerDefinitionVersionsRequestListLoggerDefinitionVersionsPaginateTypeDef,
-    ListLoggerDefinitionsRequestListLoggerDefinitionsPaginateTypeDef,
-    ListResourceDefinitionVersionsRequestListResourceDefinitionVersionsPaginateTypeDef,
-    ListResourceDefinitionsRequestListResourceDefinitionsPaginateTypeDef,
-    ListSubscriptionDefinitionVersionsRequestListSubscriptionDefinitionVersionsPaginateTypeDef,
-    ListSubscriptionDefinitionsRequestListSubscriptionDefinitionsPaginateTypeDef,
     ListConnectorDefinitionVersionsResponseTypeDef,
     ListCoreDefinitionVersionsResponseTypeDef,
     ListDeviceDefinitionVersionsResponseTypeDef,
     ListFunctionDefinitionVersionsResponseTypeDef,
     ListGroupVersionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
@@ -663,42 +663,42 @@
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

### Comparing `mypy-boto3-greengrass-1.26.59/mypy_boto3_greengrass.egg-info/SOURCES.txt` & `mypy-boto3-greengrass-1.27.0/mypy_boto3_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.26.59/setup.py` & `mypy-boto3-greengrass-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-greengrass.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrass",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Greengrass 1.26.59 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Greengrass 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/",
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


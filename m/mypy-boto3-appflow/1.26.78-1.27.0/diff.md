# Comparing `tmp/mypy-boto3-appflow-1.26.78.tar.gz` & `tmp/mypy-boto3-appflow-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.26.78.tar` & `mypy-boto3-appflow-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68382 2023-02-23 20:34:22.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68286 2023-02-23 20:34:21.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.318818 mypy-boto3-appflow-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-07-03 19:50:22.318818 mypy-boto3-appflow-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.314818 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19559 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18359 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71155 2023-07-03 19:32:29.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71053 2023-07-03 19:32:28.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.314818 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-07-03 19:50:22.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-03 19:50:22.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:22.000000 mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.318818 mypy-boto3-appflow-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:32:27.000000 mypy-boto3-appflow-1.27.0/setup.py
```

### Comparing `mypy-boto3-appflow-1.26.78/LICENSE` & `mypy-boto3-appflow-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-appflow-1.26.78/PKG-INFO` & `mypy-boto3-appflow-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.26.78
-Summary: Type annotations for boto3.Appflow 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.Appflow 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appflow"></a>
 
 # mypy-boto3-appflow
 
 [![PyPI - mypy-boto3-appflow](https://img.shields.io/pypi/v/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,15 @@
     AmplitudeConnectorOperatorType,
     AuthenticationTypeType,
     CatalogTypeType,
     ConnectionModeType,
     ConnectorProvisioningTypeType,
     ConnectorTypeType,
     DataPullModeType,
+    DataTransferApiTypeType,
     DatadogConnectorOperatorType,
     DynatraceConnectorOperatorType,
     ExecutionStatusType,
     FileTypeType,
     FlowStatusType,
     GoogleAnalyticsConnectorOperatorType,
     InforNexusConnectorOperatorType,
@@ -311,14 +312,15 @@
     SAPODataConnectorOperatorType,
     SalesforceConnectorOperatorType,
     SalesforceDataTransferApiType,
     ScheduleFrequencyTypeType,
     ServiceNowConnectorOperatorType,
     SingularConnectorOperatorType,
     SlackConnectorOperatorType,
+    SupportedDataTransferTypeType,
     TaskTypeType,
     TrendmicroConnectorOperatorType,
     TriggerTypeType,
     VeevaConnectorOperatorType,
     WriteOperationTypeType,
     ZendeskConnectorOperatorType,
     AppflowServiceName,
@@ -343,15 +345,18 @@
 from mypy_boto3_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
+    CancelFlowExecutionsRequestRequestTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
     ConnectorRuntimeSettingTypeDef,
+    DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
@@ -379,19 +384,19 @@
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    ResponseMetadataTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
     ErrorHandlingConfigTypeDef,
     OAuth2PropertiesTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -406,60 +411,61 @@
     GoogleAnalyticsSourcePropertiesTypeDef,
     IncrementalPullConfigTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
     OAuthPropertiesTypeDef,
     PardotSourcePropertiesTypeDef,
     PrefixConfigTypeDef,
+    RegisterConnectorResponseTypeDef,
+    ResetConnectorMetadataCacheRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
+    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
+    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectorProfileResponseTypeDef,
+    UpdateConnectorRegistrationResponseTypeDef,
+    UpdateFlowResponseTypeDef,
     CustomAuthConfigTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
+    ListConnectorsResponseTypeDef,
+    ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
     TaskTypeDef,
     ConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
-    ListConnectorEntitiesResponseTypeDef,
-    ListConnectorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterConnectorResponseTypeDef,
-    StartFlowResponseTypeDef,
-    StopFlowResponseTypeDef,
-    UpdateConnectorProfileResponseTypeDef,
-    UpdateConnectorRegistrationResponseTypeDef,
-    UpdateFlowResponseTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
@@ -518,42 +524,42 @@
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

### Comparing `mypy-boto3-appflow-1.26.78/README.md` & `mypy-boto3-appflow-1.27.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appflow"></a>
 
 # mypy-boto3-appflow
 
 [![PyPI - mypy-boto3-appflow](https://img.shields.io/pypi/v/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -251,14 +251,15 @@
     AmplitudeConnectorOperatorType,
     AuthenticationTypeType,
     CatalogTypeType,
     ConnectionModeType,
     ConnectorProvisioningTypeType,
     ConnectorTypeType,
     DataPullModeType,
+    DataTransferApiTypeType,
     DatadogConnectorOperatorType,
     DynatraceConnectorOperatorType,
     ExecutionStatusType,
     FileTypeType,
     FlowStatusType,
     GoogleAnalyticsConnectorOperatorType,
     InforNexusConnectorOperatorType,
@@ -279,14 +280,15 @@
     SAPODataConnectorOperatorType,
     SalesforceConnectorOperatorType,
     SalesforceDataTransferApiType,
     ScheduleFrequencyTypeType,
     ServiceNowConnectorOperatorType,
     SingularConnectorOperatorType,
     SlackConnectorOperatorType,
+    SupportedDataTransferTypeType,
     TaskTypeType,
     TrendmicroConnectorOperatorType,
     TriggerTypeType,
     VeevaConnectorOperatorType,
     WriteOperationTypeType,
     ZendeskConnectorOperatorType,
     AppflowServiceName,
@@ -311,15 +313,18 @@
 from mypy_boto3_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
+    CancelFlowExecutionsRequestRequestTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
     ConnectorRuntimeSettingTypeDef,
+    DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
@@ -347,19 +352,19 @@
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    ResponseMetadataTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
     ErrorHandlingConfigTypeDef,
     OAuth2PropertiesTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -374,60 +379,61 @@
     GoogleAnalyticsSourcePropertiesTypeDef,
     IncrementalPullConfigTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
     OAuthPropertiesTypeDef,
     PardotSourcePropertiesTypeDef,
     PrefixConfigTypeDef,
+    RegisterConnectorResponseTypeDef,
+    ResetConnectorMetadataCacheRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
+    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
+    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectorProfileResponseTypeDef,
+    UpdateConnectorRegistrationResponseTypeDef,
+    UpdateFlowResponseTypeDef,
     CustomAuthConfigTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
+    ListConnectorsResponseTypeDef,
+    ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
     TaskTypeDef,
     ConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
-    ListConnectorEntitiesResponseTypeDef,
-    ListConnectorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterConnectorResponseTypeDef,
-    StartFlowResponseTypeDef,
-    StopFlowResponseTypeDef,
-    UpdateConnectorProfileResponseTypeDef,
-    UpdateConnectorRegistrationResponseTypeDef,
-    UpdateFlowResponseTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
@@ -486,42 +492,42 @@
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

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.26.78\nVersion:         1.26.78\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.Appflow 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.78")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConnectionModeType, ConnectorTypeType
 from .type_defs import (
+    CancelFlowExecutionsResponseTypeDef,
     ConnectorProfileConfigTypeDef,
     ConnectorProvisioningConfigTypeDef,
     CreateConnectorProfileResponseTypeDef,
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
@@ -48,40 +49,36 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppflowClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ConnectorAuthenticationException: Type[BotocoreClientError]
     ConnectorServerException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class AppflowClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/)
     """
 
     meta: ClientMeta
@@ -90,98 +87,101 @@
     def exceptions(self) -> Exceptions:
         """
         AppflowClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#can_paginate)
         """
+    def cancel_flow_executions(
+        self, *, flowName: str, executionIds: Sequence[str] = ...
+    ) -> CancelFlowExecutionsResponseTypeDef:
+        """
+        Cancels active runs for a flow.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#cancel_flow_executions)
+        """
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#close)
         """
-
     def create_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         kmsArn: str = ...,
-        connectorLabel: str = ...
+        connectorLabel: str = ...,
+        clientToken: str = ...
     ) -> CreateConnectorProfileResponseTypeDef:
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_connector_profile)
         """
-
     def create_flow(
         self,
         *,
         flowName: str,
         triggerConfig: TriggerConfigTypeDef,
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
-        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...
+        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_flow)
         """
-
     def delete_connector_profile(
         self, *, connectorProfileName: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables you to delete an existing connector profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_connector_profile)
         """
-
     def delete_flow(self, *, flowName: str, forceDelete: bool = ...) -> Dict[str, Any]:
         """
         Enables your application to delete an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_flow)
         """
-
     def describe_connector(
         self, *, connectorType: ConnectorTypeType, connectorLabel: str = ...
     ) -> DescribeConnectorResponseTypeDef:
         """
         Describes the given custom connector registered in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector)
         """
-
     def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
         apiVersion: str = ...
@@ -189,15 +189,14 @@
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_entity)
         """
-
     def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
@@ -206,61 +205,56 @@
         """
         Returns a list of `connector-profile` details matching the provided `connector-
         profile` names and `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_profiles)
         """
-
     def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connectors)
         """
-
     def describe_flow(self, *, flowName: str) -> DescribeFlowResponseTypeDef:
         """
         Provides a description of the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow)
         """
-
     def describe_flow_execution_records(
         self, *, flowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeFlowExecutionRecordsResponseTypeDef:
         """
         Fetches the execution history of the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow_execution_records)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#generate_presigned_url)
         """
-
     def list_connector_entities(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
@@ -269,140 +263,148 @@
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connector_entities)
         """
-
     def list_connectors(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Returns the list of all registered custom connectors in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connectors)
         """
-
     def list_flows(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListFlowsResponseTypeDef:
         """
         Lists all of the flows associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_flows)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags that are associated with a specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_tags_for_resource)
         """
-
     def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
-        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...
+        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#register_connector)
         """
+    def reset_connector_metadata_cache(
+        self,
+        *,
+        connectorProfileName: str = ...,
+        connectorType: ConnectorTypeType = ...,
+        connectorEntityName: str = ...,
+        entitiesPath: str = ...,
+        apiVersion: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Resets metadata about your connector entities that Amazon AppFlow stored in its
+        cache.
 
-    def start_flow(self, *, flowName: str) -> StartFlowResponseTypeDef:
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#reset_connector_metadata_cache)
+        """
+    def start_flow(self, *, flowName: str, clientToken: str = ...) -> StartFlowResponseTypeDef:
         """
         Activates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#start_flow)
         """
-
     def stop_flow(self, *, flowName: str) -> StopFlowResponseTypeDef:
         """
         Deactivates the existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#stop_flow)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies a tag to the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#tag_resource)
         """
-
     def unregister_connector(
         self, *, connectorLabel: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Unregisters the custom connector registered in your account that matches the
         connector label provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#unregister_connector)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#untag_resource)
         """
-
     def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
-        connectorProfileConfig: ConnectorProfileConfigTypeDef
+        connectorProfileConfig: ConnectorProfileConfigTypeDef,
+        clientToken: str = ...
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_profile)
         """
-
     def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
-        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...
+        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_registration)
         """
-
     def update_flow(
         self,
         *,
         flowName: str,
         triggerConfig: TriggerConfigTypeDef,
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
-        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...
+        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_flow)
         """
```

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConnectionModeType, ConnectorTypeType
 from .type_defs import (
+    CancelFlowExecutionsResponseTypeDef,
     ConnectorProfileConfigTypeDef,
     ConnectorProvisioningConfigTypeDef,
     CreateConnectorProfileResponseTypeDef,
     CreateFlowResponseTypeDef,
     DescribeConnectorEntityResponseTypeDef,
     DescribeConnectorProfilesResponseTypeDef,
     DescribeConnectorResponseTypeDef,
@@ -48,36 +49,40 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AppflowClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ConnectorAuthenticationException: Type[BotocoreClientError]
     ConnectorServerException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class AppflowClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/)
     """
 
     meta: ClientMeta
@@ -86,90 +91,110 @@
     def exceptions(self) -> Exceptions:
         """
         AppflowClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#can_paginate)
         """
+
+    def cancel_flow_executions(
+        self, *, flowName: str, executionIds: Sequence[str] = ...
+    ) -> CancelFlowExecutionsResponseTypeDef:
+        """
+        Cancels active runs for a flow.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.cancel_flow_executions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#cancel_flow_executions)
+        """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#close)
         """
+
     def create_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         kmsArn: str = ...,
-        connectorLabel: str = ...
+        connectorLabel: str = ...,
+        clientToken: str = ...
     ) -> CreateConnectorProfileResponseTypeDef:
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_connector_profile)
         """
+
     def create_flow(
         self,
         *,
         flowName: str,
         triggerConfig: TriggerConfigTypeDef,
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
-        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...
+        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#create_flow)
         """
+
     def delete_connector_profile(
         self, *, connectorProfileName: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables you to delete an existing connector profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_connector_profile)
         """
+
     def delete_flow(self, *, flowName: str, forceDelete: bool = ...) -> Dict[str, Any]:
         """
         Enables your application to delete an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.delete_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#delete_flow)
         """
+
     def describe_connector(
         self, *, connectorType: ConnectorTypeType, connectorLabel: str = ...
     ) -> DescribeConnectorResponseTypeDef:
         """
         Describes the given custom connector registered in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector)
         """
+
     def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
         apiVersion: str = ...
@@ -177,14 +202,15 @@
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_entity)
         """
+
     def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
@@ -193,56 +219,61 @@
         """
         Returns a list of `connector-profile` details matching the provided `connector-
         profile` names and `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connector_profiles)
         """
+
     def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_connectors)
         """
+
     def describe_flow(self, *, flowName: str) -> DescribeFlowResponseTypeDef:
         """
         Provides a description of the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow)
         """
+
     def describe_flow_execution_records(
         self, *, flowName: str, maxResults: int = ..., nextToken: str = ...
     ) -> DescribeFlowExecutionRecordsResponseTypeDef:
         """
         Fetches the execution history of the flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_flow_execution_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#describe_flow_execution_records)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#generate_presigned_url)
         """
+
     def list_connector_entities(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
@@ -251,128 +282,161 @@
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connector_entities)
         """
+
     def list_connectors(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Returns the list of all registered custom connectors in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_connectors)
         """
+
     def list_flows(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListFlowsResponseTypeDef:
         """
         Lists all of the flows associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_flows)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieves the tags that are associated with a specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#list_tags_for_resource)
         """
+
     def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
-        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...
+        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#register_connector)
         """
-    def start_flow(self, *, flowName: str) -> StartFlowResponseTypeDef:
+
+    def reset_connector_metadata_cache(
+        self,
+        *,
+        connectorProfileName: str = ...,
+        connectorType: ConnectorTypeType = ...,
+        connectorEntityName: str = ...,
+        entitiesPath: str = ...,
+        apiVersion: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Resets metadata about your connector entities that Amazon AppFlow stored in its
+        cache.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#reset_connector_metadata_cache)
+        """
+
+    def start_flow(self, *, flowName: str, clientToken: str = ...) -> StartFlowResponseTypeDef:
         """
         Activates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.start_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#start_flow)
         """
+
     def stop_flow(self, *, flowName: str) -> StopFlowResponseTypeDef:
         """
         Deactivates the existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.stop_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#stop_flow)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Applies a tag to the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#tag_resource)
         """
+
     def unregister_connector(
         self, *, connectorLabel: str, forceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Unregisters the custom connector registered in your account that matches the
         connector label provided in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.unregister_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#unregister_connector)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from the specified flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#untag_resource)
         """
+
     def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
-        connectorProfileConfig: ConnectorProfileConfigTypeDef
+        connectorProfileConfig: ConnectorProfileConfigTypeDef,
+        clientToken: str = ...
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_profile)
         """
+
     def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
-        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...
+        connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_connector_registration)
         """
+
     def update_flow(
         self,
         *,
         flowName: str,
         triggerConfig: TriggerConfigTypeDef,
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
-        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...
+        metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
+        clientToken: str = ...
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/client/#update_flow)
         """
```

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AggregationTypeType",
     "AmplitudeConnectorOperatorType",
     "AuthenticationTypeType",
     "CatalogTypeType",
     "ConnectionModeType",
     "ConnectorProvisioningTypeType",
     "ConnectorTypeType",
     "DataPullModeType",
+    "DataTransferApiTypeType",
     "DatadogConnectorOperatorType",
     "DynatraceConnectorOperatorType",
     "ExecutionStatusType",
     "FileTypeType",
     "FlowStatusType",
     "GoogleAnalyticsConnectorOperatorType",
     "InforNexusConnectorOperatorType",
@@ -52,27 +52,27 @@
     "SAPODataConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "SalesforceDataTransferApiType",
     "ScheduleFrequencyTypeType",
     "ServiceNowConnectorOperatorType",
     "SingularConnectorOperatorType",
     "SlackConnectorOperatorType",
+    "SupportedDataTransferTypeType",
     "TaskTypeType",
     "TrendmicroConnectorOperatorType",
     "TriggerTypeType",
     "VeevaConnectorOperatorType",
     "WriteOperationTypeType",
     "ZendeskConnectorOperatorType",
     "AppflowServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AggregationTypeType = Literal["None", "SingleFile"]
 AmplitudeConnectorOperatorType = Literal["BETWEEN"]
 AuthenticationTypeType = Literal["APIKEY", "BASIC", "CUSTOM", "OAUTH2"]
 CatalogTypeType = Literal["GLUE"]
 ConnectionModeType = Literal["Private", "Public"]
 ConnectorProvisioningTypeType = Literal["LAMBDA"]
 ConnectorTypeType = Literal[
@@ -98,14 +98,15 @@
     "Snowflake",
     "Trendmicro",
     "Upsolver",
     "Veeva",
     "Zendesk",
 ]
 DataPullModeType = Literal["Complete", "Incremental"]
+DataTransferApiTypeType = Literal["ASYNC", "AUTOMATIC", "SYNC"]
 DatadogConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "MASK_ALL",
     "MASK_FIRST_N",
@@ -132,15 +133,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
-ExecutionStatusType = Literal["Error", "InProgress", "Successful"]
+ExecutionStatusType = Literal["CancelStarted", "Canceled", "Error", "InProgress", "Successful"]
 FileTypeType = Literal["CSV", "JSON", "PARQUET"]
 FlowStatusType = Literal["Active", "Deleted", "Deprecated", "Draft", "Errored", "Suspended"]
 GoogleAnalyticsConnectorOperatorType = Literal["BETWEEN", "PROJECTION"]
 InforNexusConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
@@ -172,15 +173,15 @@
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
 OAuth2CustomPropTypeType = Literal["AUTH_URL", "TOKEN_URL"]
-OAuth2GrantTypeType = Literal["AUTHORIZATION_CODE", "CLIENT_CREDENTIALS"]
+OAuth2GrantTypeType = Literal["AUTHORIZATION_CODE", "CLIENT_CREDENTIALS", "JWT_BEARER"]
 OperatorPropertiesKeysType = Literal[
     "CONCAT_FORMAT",
     "DATA_TYPE",
     "DESTINATION_DATA_TYPE",
     "EXCLUDE_SOURCE_FIELDS_LIST",
     "INCLUDE_NEW_FIELDS",
     "LOWER_BOUND",
@@ -392,14 +393,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
+SupportedDataTransferTypeType = Literal["FILE", "RECORD"]
 TaskTypeType = Literal[
     "Arithmetic",
     "Filter",
     "Map",
     "Map_all",
     "Mask",
     "Merge",
@@ -477,14 +479,15 @@
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
@@ -524,14 +527,15 @@
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
@@ -610,14 +614,15 @@
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
@@ -628,14 +633,15 @@
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
@@ -671,14 +677,15 @@
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
@@ -697,16 +704,19 @@
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
@@ -790,15 +800,17 @@
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

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AggregationTypeType",
     "AmplitudeConnectorOperatorType",
     "AuthenticationTypeType",
     "CatalogTypeType",
     "ConnectionModeType",
     "ConnectorProvisioningTypeType",
     "ConnectorTypeType",
     "DataPullModeType",
+    "DataTransferApiTypeType",
     "DatadogConnectorOperatorType",
     "DynatraceConnectorOperatorType",
     "ExecutionStatusType",
     "FileTypeType",
     "FlowStatusType",
     "GoogleAnalyticsConnectorOperatorType",
     "InforNexusConnectorOperatorType",
@@ -51,26 +53,28 @@
     "SAPODataConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "SalesforceDataTransferApiType",
     "ScheduleFrequencyTypeType",
     "ServiceNowConnectorOperatorType",
     "SingularConnectorOperatorType",
     "SlackConnectorOperatorType",
+    "SupportedDataTransferTypeType",
     "TaskTypeType",
     "TrendmicroConnectorOperatorType",
     "TriggerTypeType",
     "VeevaConnectorOperatorType",
     "WriteOperationTypeType",
     "ZendeskConnectorOperatorType",
     "AppflowServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AggregationTypeType = Literal["None", "SingleFile"]
 AmplitudeConnectorOperatorType = Literal["BETWEEN"]
 AuthenticationTypeType = Literal["APIKEY", "BASIC", "CUSTOM", "OAUTH2"]
 CatalogTypeType = Literal["GLUE"]
 ConnectionModeType = Literal["Private", "Public"]
 ConnectorProvisioningTypeType = Literal["LAMBDA"]
 ConnectorTypeType = Literal[
@@ -96,14 +100,15 @@
     "Snowflake",
     "Trendmicro",
     "Upsolver",
     "Veeva",
     "Zendesk",
 ]
 DataPullModeType = Literal["Complete", "Incremental"]
+DataTransferApiTypeType = Literal["ASYNC", "AUTOMATIC", "SYNC"]
 DatadogConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "MASK_ALL",
     "MASK_FIRST_N",
@@ -130,15 +135,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
-ExecutionStatusType = Literal["Error", "InProgress", "Successful"]
+ExecutionStatusType = Literal["CancelStarted", "Canceled", "Error", "InProgress", "Successful"]
 FileTypeType = Literal["CSV", "JSON", "PARQUET"]
 FlowStatusType = Literal["Active", "Deleted", "Deprecated", "Draft", "Errored", "Suspended"]
 GoogleAnalyticsConnectorOperatorType = Literal["BETWEEN", "PROJECTION"]
 InforNexusConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
@@ -170,15 +175,15 @@
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
 OAuth2CustomPropTypeType = Literal["AUTH_URL", "TOKEN_URL"]
-OAuth2GrantTypeType = Literal["AUTHORIZATION_CODE", "CLIENT_CREDENTIALS"]
+OAuth2GrantTypeType = Literal["AUTHORIZATION_CODE", "CLIENT_CREDENTIALS", "JWT_BEARER"]
 OperatorPropertiesKeysType = Literal[
     "CONCAT_FORMAT",
     "DATA_TYPE",
     "DESTINATION_DATA_TYPE",
     "EXCLUDE_SOURCE_FIELDS_LIST",
     "INCLUDE_NEW_FIELDS",
     "LOWER_BOUND",
@@ -390,14 +395,15 @@
     "PROJECTION",
     "SUBTRACTION",
     "VALIDATE_NON_NEGATIVE",
     "VALIDATE_NON_NULL",
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
+SupportedDataTransferTypeType = Literal["FILE", "RECORD"]
 TaskTypeType = Literal[
     "Arithmetic",
     "Filter",
     "Map",
     "Map_all",
     "Mask",
     "Merge",
@@ -475,14 +481,15 @@
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
@@ -522,14 +529,15 @@
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
@@ -608,14 +616,15 @@
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
@@ -626,14 +635,15 @@
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
@@ -669,14 +679,15 @@
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
@@ -695,16 +706,19 @@
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
@@ -788,15 +802,17 @@
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

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .literals import (
     AggregationTypeType,
     AuthenticationTypeType,
     ConnectionModeType,
     ConnectorTypeType,
     DatadogConnectorOperatorType,
     DataPullModeType,
+    DataTransferApiTypeType,
     DynatraceConnectorOperatorType,
     ExecutionStatusType,
     FileTypeType,
     FlowStatusType,
     GoogleAnalyticsConnectorOperatorType,
     InforNexusConnectorOperatorType,
     MarketoConnectorOperatorType,
@@ -45,14 +46,15 @@
     SalesforceConnectorOperatorType,
     SalesforceDataTransferApiType,
     SAPODataConnectorOperatorType,
     ScheduleFrequencyTypeType,
     ServiceNowConnectorOperatorType,
     SingularConnectorOperatorType,
     SlackConnectorOperatorType,
+    SupportedDataTransferTypeType,
     TaskTypeType,
     TrendmicroConnectorOperatorType,
     TriggerTypeType,
     VeevaConnectorOperatorType,
     WriteOperationTypeType,
     ZendeskConnectorOperatorType,
 )
@@ -62,23 +64,25 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
+    "CancelFlowExecutionsRequestRequestTypeDef",
+    "CancelFlowExecutionsResponseTypeDef",
     "ConnectorRuntimeSettingTypeDef",
+    "DataTransferApiTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
     "HoneycodeMetadataTypeDef",
     "SalesforceMetadataTypeDef",
@@ -106,19 +110,19 @@
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateConnectorProfileResponseTypeDef",
+    "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
     "ErrorHandlingConfigTypeDef",
     "OAuth2PropertiesTypeDef",
-    "CustomConnectorSourcePropertiesTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
@@ -133,60 +137,61 @@
     "GoogleAnalyticsSourcePropertiesTypeDef",
     "IncrementalPullConfigTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
     "OAuthPropertiesTypeDef",
     "PardotSourcePropertiesTypeDef",
     "PrefixConfigTypeDef",
+    "RegisterConnectorResponseTypeDef",
+    "ResetConnectorMetadataCacheRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
+    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
+    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateConnectorProfileResponseTypeDef",
+    "UpdateConnectorRegistrationResponseTypeDef",
+    "UpdateFlowResponseTypeDef",
     "CustomAuthConfigTypeDef",
+    "CustomConnectorSourcePropertiesTypeDef",
+    "ListConnectorsResponseTypeDef",
+    "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
     "TaskTypeDef",
     "ConnectorProvisioningConfigTypeDef",
-    "CreateConnectorProfileResponseTypeDef",
-    "CreateFlowResponseTypeDef",
-    "ListConnectorEntitiesResponseTypeDef",
-    "ListConnectorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterConnectorResponseTypeDef",
-    "StartFlowResponseTypeDef",
-    "StopFlowResponseTypeDef",
-    "UpdateConnectorProfileResponseTypeDef",
-    "UpdateConnectorRegistrationResponseTypeDef",
-    "UpdateFlowResponseTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
@@ -271,21 +276,19 @@
     "_OptionalApiKeyCredentialsTypeDef",
     {
         "apiSecretKey": str,
     },
     total=False,
 )
 
-
 class ApiKeyCredentialsTypeDef(
     _RequiredApiKeyCredentialsTypeDef, _OptionalApiKeyCredentialsTypeDef
 ):
     pass
 
-
 AuthParameterTypeDef = TypedDict(
     "AuthParameterTypeDef",
     {
         "key": str,
         "isRequired": bool,
         "label": str,
         "description": str,
@@ -299,42 +302,80 @@
     "BasicAuthCredentialsTypeDef",
     {
         "username": str,
         "password": str,
     },
 )
 
+_RequiredCancelFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredCancelFlowExecutionsRequestRequestTypeDef",
+    {
+        "flowName": str,
+    },
+)
+_OptionalCancelFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalCancelFlowExecutionsRequestRequestTypeDef",
+    {
+        "executionIds": Sequence[str],
+    },
+    total=False,
+)
+
+class CancelFlowExecutionsRequestRequestTypeDef(
+    _RequiredCancelFlowExecutionsRequestRequestTypeDef,
+    _OptionalCancelFlowExecutionsRequestRequestTypeDef,
+):
+    pass
+
+CancelFlowExecutionsResponseTypeDef = TypedDict(
+    "CancelFlowExecutionsResponseTypeDef",
+    {
+        "invalidExecutions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConnectorRuntimeSettingTypeDef = TypedDict(
     "ConnectorRuntimeSettingTypeDef",
     {
         "key": str,
         "dataType": str,
         "isRequired": bool,
         "label": str,
         "description": str,
         "scope": str,
         "connectorSuppliedValueOptions": List[str],
     },
     total=False,
 )
 
+DataTransferApiTypeDef = TypedDict(
+    "DataTransferApiTypeDef",
+    {
+        "Name": str,
+        "Type": DataTransferApiTypeType,
+    },
+    total=False,
+)
+
 ConnectorDetailTypeDef = TypedDict(
     "ConnectorDetailTypeDef",
     {
         "connectorDescription": str,
         "connectorName": str,
         "connectorOwner": str,
         "connectorVersion": str,
         "applicationType": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "registeredAt": datetime,
         "registeredBy": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorModes": List[str],
+        "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
     },
     total=False,
 )
 
 DestinationFieldPropertiesTypeDef = TypedDict(
     "DestinationFieldPropertiesTypeDef",
     {
@@ -369,19 +410,17 @@
     {
         "label": str,
         "hasNestedEntities": bool,
     },
     total=False,
 )
 
-
 class ConnectorEntityTypeDef(_RequiredConnectorEntityTypeDef, _OptionalConnectorEntityTypeDef):
     pass
 
-
 GoogleAnalyticsMetadataTypeDef = TypedDict(
     "GoogleAnalyticsMetadataTypeDef",
     {
         "oAuthScopes": List[str],
     },
     total=False,
 )
@@ -395,14 +434,15 @@
 )
 
 SalesforceMetadataTypeDef = TypedDict(
     "SalesforceMetadataTypeDef",
     {
         "oAuthScopes": List[str],
         "dataTransferApis": List[SalesforceDataTransferApiType],
+        "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
     },
     total=False,
 )
 
 SlackMetadataTypeDef = TypedDict(
     "SlackMetadataTypeDef",
     {
@@ -587,22 +627,20 @@
         "clusterIdentifier": str,
         "workgroupName": str,
         "databaseName": str,
     },
     total=False,
 )
 
-
 class RedshiftConnectorProfilePropertiesTypeDef(
     _RequiredRedshiftConnectorProfilePropertiesTypeDef,
     _OptionalRedshiftConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
         "usePrivateLinkForMetadataAndAuthorization": bool,
     },
@@ -638,22 +676,20 @@
         "privateLinkServiceName": str,
         "accountName": str,
         "region": str,
     },
     total=False,
 )
 
-
 class SnowflakeConnectorProfilePropertiesTypeDef(
     _RequiredSnowflakeConnectorProfilePropertiesTypeDef,
     _OptionalSnowflakeConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 VeevaConnectorProfilePropertiesTypeDef = TypedDict(
     "VeevaConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -677,22 +713,28 @@
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateConnectorProfileResponseTypeDef = TypedDict(
+    "CreateConnectorProfileResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "connectorProfileArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFlowResponseTypeDef = TypedDict(
+    "CreateFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCustomAuthCredentialsTypeDef = TypedDict(
     "_RequiredCustomAuthCredentialsTypeDef",
     {
         "customAuthenticationType": str,
@@ -702,21 +744,19 @@
     "_OptionalCustomAuthCredentialsTypeDef",
     {
         "credentialsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
-
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
@@ -734,62 +774,37 @@
     "_OptionalOAuth2PropertiesTypeDef",
     {
         "tokenUrlCustomProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
-
-_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesTypeDef",
-    {
-        "customProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CustomConnectorSourcePropertiesTypeDef(
-    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
-):
-    pass
-
-
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_OptionalCustomerProfilesDestinationPropertiesTypeDef",
     {
         "objectTypeName": str,
     },
     total=False,
 )
 
-
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
-
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -803,43 +818,39 @@
     "_OptionalDeleteConnectorProfileRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteConnectorProfileRequestRequestTypeDef(
     _RequiredDeleteConnectorProfileRequestRequestTypeDef,
     _OptionalDeleteConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFlowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 _OptionalDeleteFlowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFlowRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class DeleteFlowRequestRequestTypeDef(
     _RequiredDeleteFlowRequestRequestTypeDef, _OptionalDeleteFlowRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectorEntityRequestRequestTypeDef",
     {
         "connectorEntityName": str,
     },
 )
 _OptionalDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
@@ -848,22 +859,20 @@
         "connectorType": ConnectorTypeType,
         "connectorProfileName": str,
         "apiVersion": str,
     },
     total=False,
 )
 
-
 class DescribeConnectorEntityRequestRequestTypeDef(
     _RequiredDescribeConnectorEntityRequestRequestTypeDef,
     _OptionalDescribeConnectorEntityRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeConnectorProfilesRequestRequestTypeDef = TypedDict(
     "DescribeConnectorProfilesRequestRequestTypeDef",
     {
         "connectorProfileNames": Sequence[str],
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "maxResults": int,
@@ -882,21 +891,19 @@
     "_OptionalDescribeConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
     },
     total=False,
 )
 
-
 class DescribeConnectorRequestRequestTypeDef(
     _RequiredDescribeConnectorRequestRequestTypeDef, _OptionalDescribeConnectorRequestRequestTypeDef
 ):
     pass
 
-
 DescribeConnectorsRequestRequestTypeDef = TypedDict(
     "DescribeConnectorsRequestRequestTypeDef",
     {
         "connectorTypes": Sequence[ConnectorTypeType],
         "maxResults": int,
         "nextToken": str,
     },
@@ -914,22 +921,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class DescribeFlowExecutionRecordsRequestRequestTypeDef(
     _RequiredDescribeFlowExecutionRecordsRequestRequestTypeDef,
     _OptionalDescribeFlowExecutionRecordsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFlowRequestRequestTypeDef = TypedDict(
     "DescribeFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
@@ -1033,14 +1038,22 @@
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
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1090,14 +1103,45 @@
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
     total=False,
 )
 
+RegisterConnectorResponseTypeDef = TypedDict(
+    "RegisterConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResetConnectorMetadataCacheRequestRequestTypeDef = TypedDict(
+    "ResetConnectorMetadataCacheRequestRequestTypeDef",
+    {
+        "connectorProfileName": str,
+        "connectorType": ConnectorTypeType,
+        "connectorEntityName": str,
+        "entitiesPath": str,
+        "apiVersion": str,
+    },
+    total=False,
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
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
@@ -1131,21 +1175,19 @@
         "enableDynamicFieldUpdate": bool,
         "includeDeletedRecords": bool,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
-
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
-
 _RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
     "_RequiredScheduledTriggerPropertiesTypeDef",
     {
         "scheduleExpression": str,
     },
 )
 _OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
@@ -1158,21 +1200,19 @@
         "scheduleOffset": int,
         "firstExecutionFrom": Union[datetime, str],
         "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
-
 class ScheduledTriggerPropertiesTypeDef(
     _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
 ):
     pass
 
-
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1210,42 +1250,71 @@
         "includeSourceFiles": bool,
         "includeRenditions": bool,
         "includeAllVersions": bool,
     },
     total=False,
 )
 
-
 class VeevaSourcePropertiesTypeDef(
     _RequiredVeevaSourcePropertiesTypeDef, _OptionalVeevaSourcePropertiesTypeDef
 ):
     pass
 
-
 ZendeskSourcePropertiesTypeDef = TypedDict(
     "ZendeskSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-StartFlowRequestRequestTypeDef = TypedDict(
-    "StartFlowRequestRequestTypeDef",
+_RequiredStartFlowRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
+_OptionalStartFlowRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlowRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class StartFlowRequestRequestTypeDef(
+    _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
+):
+    pass
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "executionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1260,39 +1329,99 @@
     "_OptionalUnregisterConnectorRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
-
 class UnregisterConnectorRequestRequestTypeDef(
     _RequiredUnregisterConnectorRequestRequestTypeDef,
     _OptionalUnregisterConnectorRequestRequestTypeDef,
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateConnectorProfileResponseTypeDef = TypedDict(
+    "UpdateConnectorProfileResponseTypeDef",
+    {
+        "connectorProfileArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateConnectorRegistrationResponseTypeDef = TypedDict(
+    "UpdateConnectorRegistrationResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFlowResponseTypeDef = TypedDict(
+    "UpdateFlowResponseTypeDef",
+    {
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomAuthConfigTypeDef = TypedDict(
     "CustomAuthConfigTypeDef",
     {
         "customAuthenticationType": str,
         "authParameters": List[AuthParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+    {
+        "customProperties": Mapping[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
+    },
+    total=False,
+)
+
+class CustomConnectorSourcePropertiesTypeDef(
+    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+):
+    pass
+
+ListConnectorsResponseTypeDef = TypedDict(
+    "ListConnectorsResponseTypeDef",
+    {
+        "connectors": List[ConnectorDetailTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListConnectorEntitiesResponseTypeDef = TypedDict(
+    "ListConnectorEntitiesResponseTypeDef",
+    {
+        "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConnectorMetadataTypeDef = TypedDict(
     "ConnectorMetadataTypeDef",
     {
         "Amplitude": Dict[str, Any],
         "Datadog": Dict[str, Any],
         "Dynatrace": Dict[str, Any],
         "GoogleAnalytics": GoogleAnalyticsMetadataTypeDef,
@@ -1331,22 +1460,20 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class GoogleAnalyticsConnectorProfileCredentialsTypeDef(
     _RequiredGoogleAnalyticsConnectorProfileCredentialsTypeDef,
     _OptionalGoogleAnalyticsConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 HoneycodeConnectorProfileCredentialsTypeDef = TypedDict(
     "HoneycodeConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
@@ -1365,22 +1492,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class MarketoConnectorProfileCredentialsTypeDef(
     _RequiredMarketoConnectorProfileCredentialsTypeDef,
     _OptionalMarketoConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 OAuth2CredentialsTypeDef = TypedDict(
     "OAuth2CredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
         "accessToken": str,
         "refreshToken": str,
@@ -1402,19 +1527,17 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class OAuthCredentialsTypeDef(_RequiredOAuthCredentialsTypeDef, _OptionalOAuthCredentialsTypeDef):
     pass
 
-
 PardotConnectorProfileCredentialsTypeDef = TypedDict(
     "PardotConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
@@ -1425,14 +1548,16 @@
 SalesforceConnectorProfileCredentialsTypeDef = TypedDict(
     "SalesforceConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
+        "oAuth2GrantType": OAuth2GrantTypeType,
+        "jwtToken": str,
     },
     total=False,
 )
 
 _RequiredSlackConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredSlackConnectorProfileCredentialsTypeDef",
     {
@@ -1445,22 +1570,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class SlackConnectorProfileCredentialsTypeDef(
     _RequiredSlackConnectorProfileCredentialsTypeDef,
     _OptionalSlackConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 _RequiredZendeskConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredZendeskConnectorProfileCredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
     },
 )
@@ -1469,22 +1592,20 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
-
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
 )
@@ -1494,121 +1615,25 @@
         "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Mapping[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
-
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
-CreateConnectorProfileResponseTypeDef = TypedDict(
-    "CreateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFlowResponseTypeDef = TypedDict(
-    "CreateFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConnectorEntitiesResponseTypeDef = TypedDict(
-    "ListConnectorEntitiesResponseTypeDef",
-    {
-        "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConnectorsResponseTypeDef = TypedDict(
-    "ListConnectorsResponseTypeDef",
-    {
-        "connectors": List[ConnectorDetailTypeDef],
-        "nextToken": str,
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
-RegisterConnectorResponseTypeDef = TypedDict(
-    "RegisterConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "executionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectorProfileResponseTypeDef = TypedDict(
-    "UpdateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectorRegistrationResponseTypeDef = TypedDict(
-    "UpdateConnectorRegistrationResponseTypeDef",
-    {
-        "connectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFlowResponseTypeDef = TypedDict(
-    "UpdateFlowResponseTypeDef",
-    {
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1618,86 +1643,78 @@
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": Sequence[str],
         "customProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CustomConnectorDestinationPropertiesTypeDef(
     _RequiredCustomConnectorDestinationPropertiesTypeDef,
     _OptionalCustomConnectorDestinationPropertiesTypeDef,
 ):
     pass
 
-
 _RequiredEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredEventBridgeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalEventBridgeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class EventBridgeDestinationPropertiesTypeDef(
     _RequiredEventBridgeDestinationPropertiesTypeDef,
     _OptionalEventBridgeDestinationPropertiesTypeDef,
 ):
     pass
 
-
 _RequiredHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredHoneycodeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalHoneycodeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class HoneycodeDestinationPropertiesTypeDef(
     _RequiredHoneycodeDestinationPropertiesTypeDef, _OptionalHoneycodeDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredMarketoDestinationPropertiesTypeDef = TypedDict(
     "_RequiredMarketoDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalMarketoDestinationPropertiesTypeDef = TypedDict(
     "_OptionalMarketoDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class MarketoDestinationPropertiesTypeDef(
     _RequiredMarketoDestinationPropertiesTypeDef, _OptionalMarketoDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredRedshiftDestinationPropertiesTypeDef = TypedDict(
     "_RequiredRedshiftDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1706,21 +1723,19 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -1730,21 +1745,19 @@
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
-
 class SalesforceDestinationPropertiesTypeDef(
     _RequiredSalesforceDestinationPropertiesTypeDef, _OptionalSalesforceDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredSnowflakeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSnowflakeDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1753,21 +1766,19 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
-
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -1776,21 +1787,19 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
-
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
-
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
@@ -1844,19 +1853,17 @@
         "supportedDateFormat": str,
         "fieldValueRange": RangeTypeDef,
         "fieldLengthRange": RangeTypeDef,
     },
     total=False,
 )
 
-
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
-
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -1895,26 +1902,25 @@
 )
 _OptionalSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_OptionalSAPODataConnectorProfilePropertiesTypeDef",
     {
         "logonLanguage": str,
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
+        "disableSSO": bool,
     },
     total=False,
 )
 
-
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
-
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
@@ -1933,21 +1939,19 @@
     {
         "fileType": FileTypeType,
         "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
-
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1955,21 +1959,19 @@
     {
         "bucketPrefix": str,
         "s3InputFormatConfig": S3InputFormatConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
-
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesTypeDef = TypedDict(
@@ -1979,21 +1981,19 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
-
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
-
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2011,22 +2011,20 @@
         "oauth2": OAuth2CredentialsTypeDef,
         "apiKey": ApiKeyCredentialsTypeDef,
         "custom": CustomAuthCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class CustomConnectorProfileCredentialsTypeDef(
     _RequiredCustomConnectorProfileCredentialsTypeDef,
     _OptionalCustomConnectorProfileCredentialsTypeDef,
 ):
     pass
 
-
 SAPODataConnectorProfileCredentialsTypeDef = TypedDict(
     "SAPODataConnectorProfileCredentialsTypeDef",
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
@@ -2035,14 +2033,15 @@
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
 _RequiredUpdateConnectorRegistrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorRegistrationRequestRequestTypeDef",
     {
@@ -2050,32 +2049,31 @@
     },
 )
 _OptionalUpdateConnectorRegistrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateConnectorRegistrationRequestRequestTypeDef",
     {
         "description": str,
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateConnectorRegistrationRequestRequestTypeDef(
     _RequiredUpdateConnectorRegistrationRequestRequestTypeDef,
     _OptionalUpdateConnectorRegistrationRequestRequestTypeDef,
 ):
     pass
 
-
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SupportedFieldTypeDetailsTypeDef = TypedDict(
     "SupportedFieldTypeDetailsTypeDef",
     {
         "v1": FieldTypeDetailsTypeDef,
@@ -2147,21 +2145,19 @@
     {
         "bucketPrefix": str,
         "s3OutputFormatConfig": S3OutputFormatConfigTypeDef,
     },
     total=False,
 )
 
-
 class S3DestinationPropertiesTypeDef(
     _RequiredS3DestinationPropertiesTypeDef, _OptionalS3DestinationPropertiesTypeDef
 ):
     pass
 
-
 _RequiredUpsolverDestinationPropertiesTypeDef = TypedDict(
     "_RequiredUpsolverDestinationPropertiesTypeDef",
     {
         "bucketName": str,
         "s3OutputFormatConfig": UpsolverS3OutputFormatConfigTypeDef,
     },
 )
@@ -2169,21 +2165,19 @@
     "_OptionalUpsolverDestinationPropertiesTypeDef",
     {
         "bucketPrefix": str,
     },
     total=False,
 )
 
-
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
-
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
         "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
@@ -2214,19 +2208,17 @@
     "_OptionalTriggerConfigTypeDef",
     {
         "triggerProperties": TriggerPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
     pass
 
-
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2268,27 +2260,25 @@
         "sourceProperties": SourceFieldPropertiesTypeDef,
         "destinationProperties": DestinationFieldPropertiesTypeDef,
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
-
 class ConnectorEntityFieldTypeDef(
     _RequiredConnectorEntityFieldTypeDef, _OptionalConnectorEntityFieldTypeDef
 ):
     pass
 
-
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectorConfigurationTypeDef = TypedDict(
     "ConnectorConfigurationTypeDef",
     {
         "canUseAsSource": bool,
@@ -2313,14 +2303,16 @@
         "supportedOperators": List[OperatorsType],
         "supportedWriteOperations": List[WriteOperationTypeType],
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "logoURL": str,
         "registeredAt": datetime,
         "registeredBy": str,
+        "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
+        "supportedDataTransferApis": List[DataTransferApiTypeDef],
     },
     total=False,
 )
 
 ConnectorProfileTypeDef = TypedDict(
     "ConnectorProfileTypeDef",
     {
@@ -2371,72 +2363,68 @@
         "apiVersion": str,
         "connectorProfileName": str,
         "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
-
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
-
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
     "_OptionalConnectorProfileConfigTypeDef",
     {
         "connectorProfileCredentials": ConnectorProfileCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class ConnectorProfileConfigTypeDef(
     _RequiredConnectorProfileConfigTypeDef, _OptionalConnectorProfileConfigTypeDef
 ):
     pass
 
-
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "connectorConfiguration": ConnectorConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectorsResponseTypeDef = TypedDict(
     "DescribeConnectorsResponseTypeDef",
     {
         "connectorConfigurations": Dict[ConnectorTypeType, ConnectorConfigurationTypeDef],
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectorProfilesResponseTypeDef = TypedDict(
     "DescribeConnectorProfilesResponseTypeDef",
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
@@ -2448,55 +2436,65 @@
     {
         "apiVersion": str,
         "connectorProfileName": str,
     },
     total=False,
 )
 
-
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
-
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
 )
 _OptionalCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_OptionalCreateConnectorProfileRequestRequestTypeDef",
     {
         "kmsArn": str,
         "connectorLabel": str,
+        "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateConnectorProfileRequestRequestTypeDef(
     _RequiredCreateConnectorProfileRequestRequestTypeDef,
     _OptionalCreateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateConnectorProfileRequestRequestTypeDef = TypedDict(
-    "UpdateConnectorProfileRequestRequestTypeDef",
+_RequiredUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
 )
+_OptionalUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConnectorProfileRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateConnectorProfileRequestRequestTypeDef(
+    _RequiredUpdateConnectorProfileRequestRequestTypeDef,
+    _OptionalUpdateConnectorProfileRequestRequestTypeDef,
+):
+    pass
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
@@ -2507,25 +2505,24 @@
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
         "tags": Mapping[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
-
 DescribeFlowResponseTypeDef = TypedDict(
     "DescribeFlowResponseTypeDef",
     {
         "flowArn": str,
         "description": str,
         "flowName": str,
         "kmsArn": str,
@@ -2540,15 +2537,15 @@
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
         "schemaVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
@@ -2559,16 +2556,16 @@
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateFlowRequestRequestTypeDef(
     _RequiredUpdateFlowRequestRequestTypeDef, _OptionalUpdateFlowRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .literals import (
     AggregationTypeType,
     AuthenticationTypeType,
     ConnectionModeType,
     ConnectorTypeType,
     DatadogConnectorOperatorType,
     DataPullModeType,
+    DataTransferApiTypeType,
     DynatraceConnectorOperatorType,
     ExecutionStatusType,
     FileTypeType,
     FlowStatusType,
     GoogleAnalyticsConnectorOperatorType,
     InforNexusConnectorOperatorType,
     MarketoConnectorOperatorType,
@@ -45,14 +46,15 @@
     SalesforceConnectorOperatorType,
     SalesforceDataTransferApiType,
     SAPODataConnectorOperatorType,
     ScheduleFrequencyTypeType,
     ServiceNowConnectorOperatorType,
     SingularConnectorOperatorType,
     SlackConnectorOperatorType,
+    SupportedDataTransferTypeType,
     TaskTypeType,
     TrendmicroConnectorOperatorType,
     TriggerTypeType,
     VeevaConnectorOperatorType,
     WriteOperationTypeType,
     ZendeskConnectorOperatorType,
 )
@@ -62,22 +64,26 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
+    "CancelFlowExecutionsRequestRequestTypeDef",
+    "CancelFlowExecutionsResponseTypeDef",
     "ConnectorRuntimeSettingTypeDef",
+    "DataTransferApiTypeDef",
     "ConnectorDetailTypeDef",
     "DestinationFieldPropertiesTypeDef",
     "SourceFieldPropertiesTypeDef",
     "ConnectorEntityTypeDef",
     "GoogleAnalyticsMetadataTypeDef",
     "HoneycodeMetadataTypeDef",
     "SalesforceMetadataTypeDef",
@@ -105,19 +111,19 @@
     "ServiceNowConnectorProfilePropertiesTypeDef",
     "SlackConnectorProfilePropertiesTypeDef",
     "SnowflakeConnectorProfilePropertiesTypeDef",
     "VeevaConnectorProfilePropertiesTypeDef",
     "ZendeskConnectorProfilePropertiesTypeDef",
     "PrivateConnectionProvisioningStateTypeDef",
     "LambdaConnectorProvisioningConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateConnectorProfileResponseTypeDef",
+    "CreateFlowResponseTypeDef",
     "CustomAuthCredentialsTypeDef",
     "ErrorHandlingConfigTypeDef",
     "OAuth2PropertiesTypeDef",
-    "CustomConnectorSourcePropertiesTypeDef",
     "CustomerProfilesDestinationPropertiesTypeDef",
     "DatadogSourcePropertiesTypeDef",
     "DeleteConnectorProfileRequestRequestTypeDef",
     "DeleteFlowRequestRequestTypeDef",
     "DescribeConnectorEntityRequestRequestTypeDef",
     "DescribeConnectorProfilesRequestRequestTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
@@ -132,60 +138,61 @@
     "GoogleAnalyticsSourcePropertiesTypeDef",
     "IncrementalPullConfigTypeDef",
     "InforNexusSourcePropertiesTypeDef",
     "ListConnectorEntitiesRequestRequestTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListFlowsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "RegistrationOutputTypeDef",
     "OAuth2CustomParameterTypeDef",
     "OAuthPropertiesTypeDef",
     "PardotSourcePropertiesTypeDef",
     "PrefixConfigTypeDef",
+    "RegisterConnectorResponseTypeDef",
+    "ResetConnectorMetadataCacheRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "S3InputFormatConfigTypeDef",
     "SuccessResponseHandlingConfigTypeDef",
     "SAPODataSourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "SingularSourcePropertiesTypeDef",
     "SlackSourcePropertiesTypeDef",
     "TrendmicroSourcePropertiesTypeDef",
     "VeevaSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "StartFlowRequestRequestTypeDef",
+    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
+    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnregisterConnectorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateConnectorProfileResponseTypeDef",
+    "UpdateConnectorRegistrationResponseTypeDef",
+    "UpdateFlowResponseTypeDef",
     "CustomAuthConfigTypeDef",
+    "CustomConnectorSourcePropertiesTypeDef",
+    "ListConnectorsResponseTypeDef",
+    "ListConnectorEntitiesResponseTypeDef",
     "ConnectorMetadataTypeDef",
     "GoogleAnalyticsConnectorProfileCredentialsTypeDef",
     "HoneycodeConnectorProfileCredentialsTypeDef",
     "MarketoConnectorProfileCredentialsTypeDef",
     "OAuth2CredentialsTypeDef",
     "OAuthCredentialsTypeDef",
     "PardotConnectorProfileCredentialsTypeDef",
     "SalesforceConnectorProfileCredentialsTypeDef",
     "SlackConnectorProfileCredentialsTypeDef",
     "ZendeskConnectorProfileCredentialsTypeDef",
     "TaskTypeDef",
     "ConnectorProvisioningConfigTypeDef",
-    "CreateConnectorProfileResponseTypeDef",
-    "CreateFlowResponseTypeDef",
-    "ListConnectorEntitiesResponseTypeDef",
-    "ListConnectorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterConnectorResponseTypeDef",
-    "StartFlowResponseTypeDef",
-    "StopFlowResponseTypeDef",
-    "UpdateConnectorProfileResponseTypeDef",
-    "UpdateConnectorRegistrationResponseTypeDef",
-    "UpdateFlowResponseTypeDef",
     "CustomConnectorDestinationPropertiesTypeDef",
     "EventBridgeDestinationPropertiesTypeDef",
     "HoneycodeDestinationPropertiesTypeDef",
     "MarketoDestinationPropertiesTypeDef",
     "RedshiftDestinationPropertiesTypeDef",
     "SalesforceDestinationPropertiesTypeDef",
     "SnowflakeDestinationPropertiesTypeDef",
@@ -270,19 +277,21 @@
     "_OptionalApiKeyCredentialsTypeDef",
     {
         "apiSecretKey": str,
     },
     total=False,
 )
 
+
 class ApiKeyCredentialsTypeDef(
     _RequiredApiKeyCredentialsTypeDef, _OptionalApiKeyCredentialsTypeDef
 ):
     pass
 
+
 AuthParameterTypeDef = TypedDict(
     "AuthParameterTypeDef",
     {
         "key": str,
         "isRequired": bool,
         "label": str,
         "description": str,
@@ -296,42 +305,82 @@
     "BasicAuthCredentialsTypeDef",
     {
         "username": str,
         "password": str,
     },
 )
 
+_RequiredCancelFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredCancelFlowExecutionsRequestRequestTypeDef",
+    {
+        "flowName": str,
+    },
+)
+_OptionalCancelFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalCancelFlowExecutionsRequestRequestTypeDef",
+    {
+        "executionIds": Sequence[str],
+    },
+    total=False,
+)
+
+
+class CancelFlowExecutionsRequestRequestTypeDef(
+    _RequiredCancelFlowExecutionsRequestRequestTypeDef,
+    _OptionalCancelFlowExecutionsRequestRequestTypeDef,
+):
+    pass
+
+
+CancelFlowExecutionsResponseTypeDef = TypedDict(
+    "CancelFlowExecutionsResponseTypeDef",
+    {
+        "invalidExecutions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConnectorRuntimeSettingTypeDef = TypedDict(
     "ConnectorRuntimeSettingTypeDef",
     {
         "key": str,
         "dataType": str,
         "isRequired": bool,
         "label": str,
         "description": str,
         "scope": str,
         "connectorSuppliedValueOptions": List[str],
     },
     total=False,
 )
 
+DataTransferApiTypeDef = TypedDict(
+    "DataTransferApiTypeDef",
+    {
+        "Name": str,
+        "Type": DataTransferApiTypeType,
+    },
+    total=False,
+)
+
 ConnectorDetailTypeDef = TypedDict(
     "ConnectorDetailTypeDef",
     {
         "connectorDescription": str,
         "connectorName": str,
         "connectorOwner": str,
         "connectorVersion": str,
         "applicationType": str,
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "registeredAt": datetime,
         "registeredBy": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorModes": List[str],
+        "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
     },
     total=False,
 )
 
 DestinationFieldPropertiesTypeDef = TypedDict(
     "DestinationFieldPropertiesTypeDef",
     {
@@ -366,17 +415,19 @@
     {
         "label": str,
         "hasNestedEntities": bool,
     },
     total=False,
 )
 
+
 class ConnectorEntityTypeDef(_RequiredConnectorEntityTypeDef, _OptionalConnectorEntityTypeDef):
     pass
 
+
 GoogleAnalyticsMetadataTypeDef = TypedDict(
     "GoogleAnalyticsMetadataTypeDef",
     {
         "oAuthScopes": List[str],
     },
     total=False,
 )
@@ -390,14 +441,15 @@
 )
 
 SalesforceMetadataTypeDef = TypedDict(
     "SalesforceMetadataTypeDef",
     {
         "oAuthScopes": List[str],
         "dataTransferApis": List[SalesforceDataTransferApiType],
+        "oauth2GrantTypesSupported": List[OAuth2GrantTypeType],
     },
     total=False,
 )
 
 SlackMetadataTypeDef = TypedDict(
     "SlackMetadataTypeDef",
     {
@@ -582,20 +634,22 @@
         "clusterIdentifier": str,
         "workgroupName": str,
         "databaseName": str,
     },
     total=False,
 )
 
+
 class RedshiftConnectorProfilePropertiesTypeDef(
     _RequiredRedshiftConnectorProfilePropertiesTypeDef,
     _OptionalRedshiftConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
         "usePrivateLinkForMetadataAndAuthorization": bool,
     },
@@ -631,20 +685,22 @@
         "privateLinkServiceName": str,
         "accountName": str,
         "region": str,
     },
     total=False,
 )
 
+
 class SnowflakeConnectorProfilePropertiesTypeDef(
     _RequiredSnowflakeConnectorProfilePropertiesTypeDef,
     _OptionalSnowflakeConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 VeevaConnectorProfilePropertiesTypeDef = TypedDict(
     "VeevaConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
     },
 )
 
@@ -668,22 +724,28 @@
 LambdaConnectorProvisioningConfigTypeDef = TypedDict(
     "LambdaConnectorProvisioningConfigTypeDef",
     {
         "lambdaArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateConnectorProfileResponseTypeDef = TypedDict(
+    "CreateConnectorProfileResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "connectorProfileArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFlowResponseTypeDef = TypedDict(
+    "CreateFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCustomAuthCredentialsTypeDef = TypedDict(
     "_RequiredCustomAuthCredentialsTypeDef",
     {
         "customAuthenticationType": str,
@@ -693,19 +755,21 @@
     "_OptionalCustomAuthCredentialsTypeDef",
     {
         "credentialsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CustomAuthCredentialsTypeDef(
     _RequiredCustomAuthCredentialsTypeDef, _OptionalCustomAuthCredentialsTypeDef
 ):
     pass
 
+
 ErrorHandlingConfigTypeDef = TypedDict(
     "ErrorHandlingConfigTypeDef",
     {
         "failOnFirstDestinationError": bool,
         "bucketPrefix": str,
         "bucketName": str,
     },
@@ -723,35 +787,18 @@
     "_OptionalOAuth2PropertiesTypeDef",
     {
         "tokenUrlCustomProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class OAuth2PropertiesTypeDef(_RequiredOAuth2PropertiesTypeDef, _OptionalOAuth2PropertiesTypeDef):
     pass
 
-_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_RequiredCustomConnectorSourcePropertiesTypeDef",
-    {
-        "entityName": str,
-    },
-)
-_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
-    "_OptionalCustomConnectorSourcePropertiesTypeDef",
-    {
-        "customProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CustomConnectorSourcePropertiesTypeDef(
-    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
-):
-    pass
 
 _RequiredCustomerProfilesDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomerProfilesDestinationPropertiesTypeDef",
     {
         "domainName": str,
     },
 )
@@ -759,20 +806,22 @@
     "_OptionalCustomerProfilesDestinationPropertiesTypeDef",
     {
         "objectTypeName": str,
     },
     total=False,
 )
 
+
 class CustomerProfilesDestinationPropertiesTypeDef(
     _RequiredCustomerProfilesDestinationPropertiesTypeDef,
     _OptionalCustomerProfilesDestinationPropertiesTypeDef,
 ):
     pass
 
+
 DatadogSourcePropertiesTypeDef = TypedDict(
     "DatadogSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -786,39 +835,43 @@
     "_OptionalDeleteConnectorProfileRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteConnectorProfileRequestRequestTypeDef(
     _RequiredDeleteConnectorProfileRequestRequestTypeDef,
     _OptionalDeleteConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFlowRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 _OptionalDeleteFlowRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFlowRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class DeleteFlowRequestRequestTypeDef(
     _RequiredDeleteFlowRequestRequestTypeDef, _OptionalDeleteFlowRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectorEntityRequestRequestTypeDef",
     {
         "connectorEntityName": str,
     },
 )
 _OptionalDescribeConnectorEntityRequestRequestTypeDef = TypedDict(
@@ -827,20 +880,22 @@
         "connectorType": ConnectorTypeType,
         "connectorProfileName": str,
         "apiVersion": str,
     },
     total=False,
 )
 
+
 class DescribeConnectorEntityRequestRequestTypeDef(
     _RequiredDescribeConnectorEntityRequestRequestTypeDef,
     _OptionalDescribeConnectorEntityRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeConnectorProfilesRequestRequestTypeDef = TypedDict(
     "DescribeConnectorProfilesRequestRequestTypeDef",
     {
         "connectorProfileNames": Sequence[str],
         "connectorType": ConnectorTypeType,
         "connectorLabel": str,
         "maxResults": int,
@@ -859,19 +914,21 @@
     "_OptionalDescribeConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
     },
     total=False,
 )
 
+
 class DescribeConnectorRequestRequestTypeDef(
     _RequiredDescribeConnectorRequestRequestTypeDef, _OptionalDescribeConnectorRequestRequestTypeDef
 ):
     pass
 
+
 DescribeConnectorsRequestRequestTypeDef = TypedDict(
     "DescribeConnectorsRequestRequestTypeDef",
     {
         "connectorTypes": Sequence[ConnectorTypeType],
         "maxResults": int,
         "nextToken": str,
     },
@@ -889,20 +946,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class DescribeFlowExecutionRecordsRequestRequestTypeDef(
     _RequiredDescribeFlowExecutionRecordsRequestRequestTypeDef,
     _OptionalDescribeFlowExecutionRecordsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFlowRequestRequestTypeDef = TypedDict(
     "DescribeFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
@@ -1006,14 +1065,22 @@
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
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1063,14 +1130,45 @@
         "prefixType": PrefixTypeType,
         "prefixFormat": PrefixFormatType,
         "pathPrefixHierarchy": Sequence[PathPrefixType],
     },
     total=False,
 )
 
+RegisterConnectorResponseTypeDef = TypedDict(
+    "RegisterConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResetConnectorMetadataCacheRequestRequestTypeDef = TypedDict(
+    "ResetConnectorMetadataCacheRequestRequestTypeDef",
+    {
+        "connectorProfileName": str,
+        "connectorType": ConnectorTypeType,
+        "connectorEntityName": str,
+        "entitiesPath": str,
+        "apiVersion": str,
+    },
+    total=False,
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
 S3InputFormatConfigTypeDef = TypedDict(
     "S3InputFormatConfigTypeDef",
     {
         "s3InputFileType": S3InputFileTypeType,
     },
     total=False,
 )
@@ -1104,19 +1202,21 @@
         "enableDynamicFieldUpdate": bool,
         "includeDeletedRecords": bool,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
+
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
+
 _RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
     "_RequiredScheduledTriggerPropertiesTypeDef",
     {
         "scheduleExpression": str,
     },
 )
 _OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
@@ -1129,19 +1229,21 @@
         "scheduleOffset": int,
         "firstExecutionFrom": Union[datetime, str],
         "flowErrorDeactivationThreshold": int,
     },
     total=False,
 )
 
+
 class ScheduledTriggerPropertiesTypeDef(
     _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
 ):
     pass
 
+
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
@@ -1179,40 +1281,75 @@
         "includeSourceFiles": bool,
         "includeRenditions": bool,
         "includeAllVersions": bool,
     },
     total=False,
 )
 
+
 class VeevaSourcePropertiesTypeDef(
     _RequiredVeevaSourcePropertiesTypeDef, _OptionalVeevaSourcePropertiesTypeDef
 ):
     pass
 
+
 ZendeskSourcePropertiesTypeDef = TypedDict(
     "ZendeskSourcePropertiesTypeDef",
     {
         "object": str,
     },
 )
 
-StartFlowRequestRequestTypeDef = TypedDict(
-    "StartFlowRequestRequestTypeDef",
+_RequiredStartFlowRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
+_OptionalStartFlowRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFlowRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class StartFlowRequestRequestTypeDef(
+    _RequiredStartFlowRequestRequestTypeDef, _OptionalStartFlowRequestRequestTypeDef
+):
+    pass
+
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "executionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "flowName": str,
     },
 )
 
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "flowArn": str,
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1227,37 +1364,103 @@
     "_OptionalUnregisterConnectorRequestRequestTypeDef",
     {
         "forceDelete": bool,
     },
     total=False,
 )
 
+
 class UnregisterConnectorRequestRequestTypeDef(
     _RequiredUnregisterConnectorRequestRequestTypeDef,
     _OptionalUnregisterConnectorRequestRequestTypeDef,
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateConnectorProfileResponseTypeDef = TypedDict(
+    "UpdateConnectorProfileResponseTypeDef",
+    {
+        "connectorProfileArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateConnectorRegistrationResponseTypeDef = TypedDict(
+    "UpdateConnectorRegistrationResponseTypeDef",
+    {
+        "connectorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFlowResponseTypeDef = TypedDict(
+    "UpdateFlowResponseTypeDef",
+    {
+        "flowStatus": FlowStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomAuthConfigTypeDef = TypedDict(
     "CustomAuthConfigTypeDef",
     {
         "customAuthenticationType": str,
         "authParameters": List[AuthParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_RequiredCustomConnectorSourcePropertiesTypeDef",
+    {
+        "entityName": str,
+    },
+)
+_OptionalCustomConnectorSourcePropertiesTypeDef = TypedDict(
+    "_OptionalCustomConnectorSourcePropertiesTypeDef",
+    {
+        "customProperties": Mapping[str, str],
+        "dataTransferApi": DataTransferApiTypeDef,
+    },
+    total=False,
+)
+
+
+class CustomConnectorSourcePropertiesTypeDef(
+    _RequiredCustomConnectorSourcePropertiesTypeDef, _OptionalCustomConnectorSourcePropertiesTypeDef
+):
+    pass
+
+
+ListConnectorsResponseTypeDef = TypedDict(
+    "ListConnectorsResponseTypeDef",
+    {
+        "connectors": List[ConnectorDetailTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListConnectorEntitiesResponseTypeDef = TypedDict(
+    "ListConnectorEntitiesResponseTypeDef",
+    {
+        "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConnectorMetadataTypeDef = TypedDict(
     "ConnectorMetadataTypeDef",
     {
         "Amplitude": Dict[str, Any],
         "Datadog": Dict[str, Any],
         "Dynatrace": Dict[str, Any],
         "GoogleAnalytics": GoogleAnalyticsMetadataTypeDef,
@@ -1296,20 +1499,22 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class GoogleAnalyticsConnectorProfileCredentialsTypeDef(
     _RequiredGoogleAnalyticsConnectorProfileCredentialsTypeDef,
     _OptionalGoogleAnalyticsConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 HoneycodeConnectorProfileCredentialsTypeDef = TypedDict(
     "HoneycodeConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
@@ -1328,20 +1533,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class MarketoConnectorProfileCredentialsTypeDef(
     _RequiredMarketoConnectorProfileCredentialsTypeDef,
     _OptionalMarketoConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 OAuth2CredentialsTypeDef = TypedDict(
     "OAuth2CredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
         "accessToken": str,
         "refreshToken": str,
@@ -1363,17 +1570,19 @@
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class OAuthCredentialsTypeDef(_RequiredOAuthCredentialsTypeDef, _OptionalOAuthCredentialsTypeDef):
     pass
 
+
 PardotConnectorProfileCredentialsTypeDef = TypedDict(
     "PardotConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
@@ -1384,14 +1593,16 @@
 SalesforceConnectorProfileCredentialsTypeDef = TypedDict(
     "SalesforceConnectorProfileCredentialsTypeDef",
     {
         "accessToken": str,
         "refreshToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
         "clientCredentialsArn": str,
+        "oAuth2GrantType": OAuth2GrantTypeType,
+        "jwtToken": str,
     },
     total=False,
 )
 
 _RequiredSlackConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredSlackConnectorProfileCredentialsTypeDef",
     {
@@ -1404,20 +1615,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class SlackConnectorProfileCredentialsTypeDef(
     _RequiredSlackConnectorProfileCredentialsTypeDef,
     _OptionalSlackConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 _RequiredZendeskConnectorProfileCredentialsTypeDef = TypedDict(
     "_RequiredZendeskConnectorProfileCredentialsTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
     },
 )
@@ -1426,20 +1639,22 @@
     {
         "accessToken": str,
         "oAuthRequest": ConnectorOAuthRequestTypeDef,
     },
     total=False,
 )
 
+
 class ZendeskConnectorProfileCredentialsTypeDef(
     _RequiredZendeskConnectorProfileCredentialsTypeDef,
     _OptionalZendeskConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "sourceFields": Sequence[str],
         "taskType": TaskTypeType,
     },
 )
@@ -1449,119 +1664,27 @@
         "connectorOperator": ConnectorOperatorTypeDef,
         "destinationField": str,
         "taskProperties": Mapping[OperatorPropertiesKeysType, str],
     },
     total=False,
 )
 
+
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
+
 ConnectorProvisioningConfigTypeDef = TypedDict(
     "ConnectorProvisioningConfigTypeDef",
     {
         "lambda": LambdaConnectorProvisioningConfigTypeDef,
     },
     total=False,
 )
 
-CreateConnectorProfileResponseTypeDef = TypedDict(
-    "CreateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFlowResponseTypeDef = TypedDict(
-    "CreateFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConnectorEntitiesResponseTypeDef = TypedDict(
-    "ListConnectorEntitiesResponseTypeDef",
-    {
-        "connectorEntityMap": Dict[str, List[ConnectorEntityTypeDef]],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConnectorsResponseTypeDef = TypedDict(
-    "ListConnectorsResponseTypeDef",
-    {
-        "connectors": List[ConnectorDetailTypeDef],
-        "nextToken": str,
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
-RegisterConnectorResponseTypeDef = TypedDict(
-    "RegisterConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "executionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "flowArn": str,
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectorProfileResponseTypeDef = TypedDict(
-    "UpdateConnectorProfileResponseTypeDef",
-    {
-        "connectorProfileArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectorRegistrationResponseTypeDef = TypedDict(
-    "UpdateConnectorRegistrationResponseTypeDef",
-    {
-        "connectorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFlowResponseTypeDef = TypedDict(
-    "UpdateFlowResponseTypeDef",
-    {
-        "flowStatus": FlowStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCustomConnectorDestinationPropertiesTypeDef = TypedDict(
     "_RequiredCustomConnectorDestinationPropertiesTypeDef",
     {
         "entityName": str,
     },
 )
 _OptionalCustomConnectorDestinationPropertiesTypeDef = TypedDict(
@@ -1571,78 +1694,86 @@
         "writeOperationType": WriteOperationTypeType,
         "idFieldNames": Sequence[str],
         "customProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CustomConnectorDestinationPropertiesTypeDef(
     _RequiredCustomConnectorDestinationPropertiesTypeDef,
     _OptionalCustomConnectorDestinationPropertiesTypeDef,
 ):
     pass
 
+
 _RequiredEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredEventBridgeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalEventBridgeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalEventBridgeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class EventBridgeDestinationPropertiesTypeDef(
     _RequiredEventBridgeDestinationPropertiesTypeDef,
     _OptionalEventBridgeDestinationPropertiesTypeDef,
 ):
     pass
 
+
 _RequiredHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredHoneycodeDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalHoneycodeDestinationPropertiesTypeDef = TypedDict(
     "_OptionalHoneycodeDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class HoneycodeDestinationPropertiesTypeDef(
     _RequiredHoneycodeDestinationPropertiesTypeDef, _OptionalHoneycodeDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredMarketoDestinationPropertiesTypeDef = TypedDict(
     "_RequiredMarketoDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalMarketoDestinationPropertiesTypeDef = TypedDict(
     "_OptionalMarketoDestinationPropertiesTypeDef",
     {
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class MarketoDestinationPropertiesTypeDef(
     _RequiredMarketoDestinationPropertiesTypeDef, _OptionalMarketoDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredRedshiftDestinationPropertiesTypeDef = TypedDict(
     "_RequiredRedshiftDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1651,19 +1782,21 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftDestinationPropertiesTypeDef(
     _RequiredRedshiftDestinationPropertiesTypeDef, _OptionalRedshiftDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredSalesforceDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSalesforceDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalSalesforceDestinationPropertiesTypeDef = TypedDict(
@@ -1673,19 +1806,21 @@
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
         "dataTransferApi": SalesforceDataTransferApiType,
     },
     total=False,
 )
 
+
 class SalesforceDestinationPropertiesTypeDef(
     _RequiredSalesforceDestinationPropertiesTypeDef, _OptionalSalesforceDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredSnowflakeDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSnowflakeDestinationPropertiesTypeDef",
     {
         "object": str,
         "intermediateBucketName": str,
     },
 )
@@ -1694,19 +1829,21 @@
     {
         "bucketPrefix": str,
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
     },
     total=False,
 )
 
+
 class SnowflakeDestinationPropertiesTypeDef(
     _RequiredSnowflakeDestinationPropertiesTypeDef, _OptionalSnowflakeDestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredZendeskDestinationPropertiesTypeDef = TypedDict(
     "_RequiredZendeskDestinationPropertiesTypeDef",
     {
         "object": str,
     },
 )
 _OptionalZendeskDestinationPropertiesTypeDef = TypedDict(
@@ -1715,19 +1852,21 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
+
 class ZendeskDestinationPropertiesTypeDef(
     _RequiredZendeskDestinationPropertiesTypeDef, _OptionalZendeskDestinationPropertiesTypeDef
 ):
     pass
 
+
 CustomConnectorProfilePropertiesTypeDef = TypedDict(
     "CustomConnectorProfilePropertiesTypeDef",
     {
         "profileProperties": Mapping[str, str],
         "oAuth2Properties": OAuth2PropertiesTypeDef,
     },
     total=False,
@@ -1781,17 +1920,19 @@
         "supportedDateFormat": str,
         "fieldValueRange": RangeTypeDef,
         "fieldLengthRange": RangeTypeDef,
     },
     total=False,
 )
 
+
 class FieldTypeDetailsTypeDef(_RequiredFieldTypeDetailsTypeDef, _OptionalFieldTypeDetailsTypeDef):
     pass
 
+
 MetadataCatalogConfigTypeDef = TypedDict(
     "MetadataCatalogConfigTypeDef",
     {
         "glueDataCatalog": GlueDataCatalogConfigTypeDef,
     },
     total=False,
 )
@@ -1830,24 +1971,27 @@
 )
 _OptionalSAPODataConnectorProfilePropertiesTypeDef = TypedDict(
     "_OptionalSAPODataConnectorProfilePropertiesTypeDef",
     {
         "logonLanguage": str,
         "privateLinkServiceName": str,
         "oAuthProperties": OAuthPropertiesTypeDef,
+        "disableSSO": bool,
     },
     total=False,
 )
 
+
 class SAPODataConnectorProfilePropertiesTypeDef(
     _RequiredSAPODataConnectorProfilePropertiesTypeDef,
     _OptionalSAPODataConnectorProfilePropertiesTypeDef,
 ):
     pass
 
+
 S3OutputFormatConfigTypeDef = TypedDict(
     "S3OutputFormatConfigTypeDef",
     {
         "fileType": FileTypeType,
         "prefixConfig": PrefixConfigTypeDef,
         "aggregationConfig": AggregationConfigTypeDef,
         "preserveSourceDataTyping": bool,
@@ -1866,19 +2010,21 @@
     {
         "fileType": FileTypeType,
         "aggregationConfig": AggregationConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpsolverS3OutputFormatConfigTypeDef(
     _RequiredUpsolverS3OutputFormatConfigTypeDef, _OptionalUpsolverS3OutputFormatConfigTypeDef
 ):
     pass
 
+
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "bucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1886,19 +2032,21 @@
     {
         "bucketPrefix": str,
         "s3InputFormatConfig": S3InputFormatConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3SourcePropertiesTypeDef(
     _RequiredS3SourcePropertiesTypeDef, _OptionalS3SourcePropertiesTypeDef
 ):
     pass
 
+
 _RequiredSAPODataDestinationPropertiesTypeDef = TypedDict(
     "_RequiredSAPODataDestinationPropertiesTypeDef",
     {
         "objectPath": str,
     },
 )
 _OptionalSAPODataDestinationPropertiesTypeDef = TypedDict(
@@ -1908,19 +2056,21 @@
         "idFieldNames": Sequence[str],
         "errorHandlingConfig": ErrorHandlingConfigTypeDef,
         "writeOperationType": WriteOperationTypeType,
     },
     total=False,
 )
 
+
 class SAPODataDestinationPropertiesTypeDef(
     _RequiredSAPODataDestinationPropertiesTypeDef, _OptionalSAPODataDestinationPropertiesTypeDef
 ):
     pass
 
+
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -1938,20 +2088,22 @@
         "oauth2": OAuth2CredentialsTypeDef,
         "apiKey": ApiKeyCredentialsTypeDef,
         "custom": CustomAuthCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class CustomConnectorProfileCredentialsTypeDef(
     _RequiredCustomConnectorProfileCredentialsTypeDef,
     _OptionalCustomConnectorProfileCredentialsTypeDef,
 ):
     pass
 
+
 SAPODataConnectorProfileCredentialsTypeDef = TypedDict(
     "SAPODataConnectorProfileCredentialsTypeDef",
     {
         "basicAuthCredentials": BasicAuthCredentialsTypeDef,
         "oAuthCredentials": OAuthCredentialsTypeDef,
     },
     total=False,
@@ -1960,14 +2112,15 @@
 RegisterConnectorRequestRequestTypeDef = TypedDict(
     "RegisterConnectorRequestRequestTypeDef",
     {
         "connectorLabel": str,
         "description": str,
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
 _RequiredUpdateConnectorRegistrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectorRegistrationRequestRequestTypeDef",
     {
@@ -1975,30 +2128,33 @@
     },
 )
 _OptionalUpdateConnectorRegistrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateConnectorRegistrationRequestRequestTypeDef",
     {
         "description": str,
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateConnectorRegistrationRequestRequestTypeDef(
     _RequiredUpdateConnectorRegistrationRequestRequestTypeDef,
     _OptionalUpdateConnectorRegistrationRequestRequestTypeDef,
 ):
     pass
 
+
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "flows": List[FlowDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SupportedFieldTypeDetailsTypeDef = TypedDict(
     "SupportedFieldTypeDetailsTypeDef",
     {
         "v1": FieldTypeDetailsTypeDef,
@@ -2070,19 +2226,21 @@
     {
         "bucketPrefix": str,
         "s3OutputFormatConfig": S3OutputFormatConfigTypeDef,
     },
     total=False,
 )
 
+
 class S3DestinationPropertiesTypeDef(
     _RequiredS3DestinationPropertiesTypeDef, _OptionalS3DestinationPropertiesTypeDef
 ):
     pass
 
+
 _RequiredUpsolverDestinationPropertiesTypeDef = TypedDict(
     "_RequiredUpsolverDestinationPropertiesTypeDef",
     {
         "bucketName": str,
         "s3OutputFormatConfig": UpsolverS3OutputFormatConfigTypeDef,
     },
 )
@@ -2090,19 +2248,21 @@
     "_OptionalUpsolverDestinationPropertiesTypeDef",
     {
         "bucketPrefix": str,
     },
     total=False,
 )
 
+
 class UpsolverDestinationPropertiesTypeDef(
     _RequiredUpsolverDestinationPropertiesTypeDef, _OptionalUpsolverDestinationPropertiesTypeDef
 ):
     pass
 
+
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Amplitude": AmplitudeSourcePropertiesTypeDef,
         "Datadog": DatadogSourcePropertiesTypeDef,
         "Dynatrace": DynatraceSourcePropertiesTypeDef,
         "GoogleAnalytics": GoogleAnalyticsSourcePropertiesTypeDef,
@@ -2133,17 +2293,19 @@
     "_OptionalTriggerConfigTypeDef",
     {
         "triggerProperties": TriggerPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
     pass
 
+
 ConnectorProfileCredentialsTypeDef = TypedDict(
     "ConnectorProfileCredentialsTypeDef",
     {
         "Amplitude": AmplitudeConnectorProfileCredentialsTypeDef,
         "Datadog": DatadogConnectorProfileCredentialsTypeDef,
         "Dynatrace": DynatraceConnectorProfileCredentialsTypeDef,
         "GoogleAnalytics": GoogleAnalyticsConnectorProfileCredentialsTypeDef,
@@ -2185,25 +2347,27 @@
         "sourceProperties": SourceFieldPropertiesTypeDef,
         "destinationProperties": DestinationFieldPropertiesTypeDef,
         "customProperties": Dict[str, str],
     },
     total=False,
 )
 
+
 class ConnectorEntityFieldTypeDef(
     _RequiredConnectorEntityFieldTypeDef, _OptionalConnectorEntityFieldTypeDef
 ):
     pass
 
+
 DescribeFlowExecutionRecordsResponseTypeDef = TypedDict(
     "DescribeFlowExecutionRecordsResponseTypeDef",
     {
         "flowExecutions": List[ExecutionRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectorConfigurationTypeDef = TypedDict(
     "ConnectorConfigurationTypeDef",
     {
         "canUseAsSource": bool,
@@ -2228,14 +2392,16 @@
         "supportedOperators": List[OperatorsType],
         "supportedWriteOperations": List[WriteOperationTypeType],
         "connectorProvisioningType": Literal["LAMBDA"],
         "connectorProvisioningConfig": ConnectorProvisioningConfigTypeDef,
         "logoURL": str,
         "registeredAt": datetime,
         "registeredBy": str,
+        "supportedDataTransferTypes": List[SupportedDataTransferTypeType],
+        "supportedDataTransferApis": List[DataTransferApiTypeDef],
     },
     total=False,
 )
 
 ConnectorProfileTypeDef = TypedDict(
     "ConnectorProfileTypeDef",
     {
@@ -2286,68 +2452,72 @@
         "apiVersion": str,
         "connectorProfileName": str,
         "incrementalPullConfig": IncrementalPullConfigTypeDef,
     },
     total=False,
 )
 
+
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+
 _RequiredConnectorProfileConfigTypeDef = TypedDict(
     "_RequiredConnectorProfileConfigTypeDef",
     {
         "connectorProfileProperties": ConnectorProfilePropertiesTypeDef,
     },
 )
 _OptionalConnectorProfileConfigTypeDef = TypedDict(
     "_OptionalConnectorProfileConfigTypeDef",
     {
         "connectorProfileCredentials": ConnectorProfileCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class ConnectorProfileConfigTypeDef(
     _RequiredConnectorProfileConfigTypeDef, _OptionalConnectorProfileConfigTypeDef
 ):
     pass
 
+
 DescribeConnectorEntityResponseTypeDef = TypedDict(
     "DescribeConnectorEntityResponseTypeDef",
     {
         "connectorEntityFields": List[ConnectorEntityFieldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "connectorConfiguration": ConnectorConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectorsResponseTypeDef = TypedDict(
     "DescribeConnectorsResponseTypeDef",
     {
         "connectorConfigurations": Dict[ConnectorTypeType, ConnectorConfigurationTypeDef],
         "connectors": List[ConnectorDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectorProfilesResponseTypeDef = TypedDict(
     "DescribeConnectorProfilesResponseTypeDef",
     {
         "connectorProfileDetails": List[ConnectorProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDestinationFlowConfigTypeDef = TypedDict(
     "_RequiredDestinationFlowConfigTypeDef",
     {
         "connectorType": ConnectorTypeType,
@@ -2359,51 +2529,71 @@
     {
         "apiVersion": str,
         "connectorProfileName": str,
     },
     total=False,
 )
 
+
 class DestinationFlowConfigTypeDef(
     _RequiredDestinationFlowConfigTypeDef, _OptionalDestinationFlowConfigTypeDef
 ):
     pass
 
+
 _RequiredCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectorType": ConnectorTypeType,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
 )
 _OptionalCreateConnectorProfileRequestRequestTypeDef = TypedDict(
     "_OptionalCreateConnectorProfileRequestRequestTypeDef",
     {
         "kmsArn": str,
         "connectorLabel": str,
+        "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateConnectorProfileRequestRequestTypeDef(
     _RequiredCreateConnectorProfileRequestRequestTypeDef,
     _OptionalCreateConnectorProfileRequestRequestTypeDef,
 ):
     pass
 
-UpdateConnectorProfileRequestRequestTypeDef = TypedDict(
-    "UpdateConnectorProfileRequestRequestTypeDef",
+
+_RequiredUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConnectorProfileRequestRequestTypeDef",
     {
         "connectorProfileName": str,
         "connectionMode": ConnectionModeType,
         "connectorProfileConfig": ConnectorProfileConfigTypeDef,
     },
 )
+_OptionalUpdateConnectorProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConnectorProfileRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateConnectorProfileRequestRequestTypeDef(
+    _RequiredUpdateConnectorProfileRequestRequestTypeDef,
+    _OptionalUpdateConnectorProfileRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredCreateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowRequestRequestTypeDef",
     {
         "flowName": str,
         "triggerConfig": TriggerConfigTypeDef,
         "sourceFlowConfig": SourceFlowConfigTypeDef,
@@ -2414,23 +2604,26 @@
 _OptionalCreateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowRequestRequestTypeDef",
     {
         "description": str,
         "kmsArn": str,
         "tags": Mapping[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateFlowRequestRequestTypeDef(
     _RequiredCreateFlowRequestRequestTypeDef, _OptionalCreateFlowRequestRequestTypeDef
 ):
     pass
 
+
 DescribeFlowResponseTypeDef = TypedDict(
     "DescribeFlowResponseTypeDef",
     {
         "flowArn": str,
         "description": str,
         "flowName": str,
         "kmsArn": str,
@@ -2445,15 +2638,15 @@
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
         "lastRunMetadataCatalogDetails": List[MetadataCatalogDetailTypeDef],
         "schemaVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFlowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowRequestRequestTypeDef",
     {
         "flowName": str,
@@ -2464,15 +2657,17 @@
     },
 )
 _OptionalUpdateFlowRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateFlowRequestRequestTypeDef",
     {
         "description": str,
         "metadataCatalogConfig": MetadataCatalogConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateFlowRequestRequestTypeDef(
     _RequiredUpdateFlowRequestRequestTypeDef, _OptionalUpdateFlowRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.26.78
-Summary: Type annotations for boto3.Appflow 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.Appflow 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appflow"></a>
 
 # mypy-boto3-appflow
 
 [![PyPI - mypy-boto3-appflow](https://img.shields.io/pypi/v/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,15 @@
     AmplitudeConnectorOperatorType,
     AuthenticationTypeType,
     CatalogTypeType,
     ConnectionModeType,
     ConnectorProvisioningTypeType,
     ConnectorTypeType,
     DataPullModeType,
+    DataTransferApiTypeType,
     DatadogConnectorOperatorType,
     DynatraceConnectorOperatorType,
     ExecutionStatusType,
     FileTypeType,
     FlowStatusType,
     GoogleAnalyticsConnectorOperatorType,
     InforNexusConnectorOperatorType,
@@ -311,14 +312,15 @@
     SAPODataConnectorOperatorType,
     SalesforceConnectorOperatorType,
     SalesforceDataTransferApiType,
     ScheduleFrequencyTypeType,
     ServiceNowConnectorOperatorType,
     SingularConnectorOperatorType,
     SlackConnectorOperatorType,
+    SupportedDataTransferTypeType,
     TaskTypeType,
     TrendmicroConnectorOperatorType,
     TriggerTypeType,
     VeevaConnectorOperatorType,
     WriteOperationTypeType,
     ZendeskConnectorOperatorType,
     AppflowServiceName,
@@ -343,15 +345,18 @@
 from mypy_boto3_appflow.type_defs import (
     AggregationConfigTypeDef,
     AmplitudeConnectorProfileCredentialsTypeDef,
     AmplitudeSourcePropertiesTypeDef,
     ApiKeyCredentialsTypeDef,
     AuthParameterTypeDef,
     BasicAuthCredentialsTypeDef,
+    CancelFlowExecutionsRequestRequestTypeDef,
+    CancelFlowExecutionsResponseTypeDef,
     ConnectorRuntimeSettingTypeDef,
+    DataTransferApiTypeDef,
     ConnectorDetailTypeDef,
     DestinationFieldPropertiesTypeDef,
     SourceFieldPropertiesTypeDef,
     ConnectorEntityTypeDef,
     GoogleAnalyticsMetadataTypeDef,
     HoneycodeMetadataTypeDef,
     SalesforceMetadataTypeDef,
@@ -379,19 +384,19 @@
     ServiceNowConnectorProfilePropertiesTypeDef,
     SlackConnectorProfilePropertiesTypeDef,
     SnowflakeConnectorProfilePropertiesTypeDef,
     VeevaConnectorProfilePropertiesTypeDef,
     ZendeskConnectorProfilePropertiesTypeDef,
     PrivateConnectionProvisioningStateTypeDef,
     LambdaConnectorProvisioningConfigTypeDef,
-    ResponseMetadataTypeDef,
+    CreateConnectorProfileResponseTypeDef,
+    CreateFlowResponseTypeDef,
     CustomAuthCredentialsTypeDef,
     ErrorHandlingConfigTypeDef,
     OAuth2PropertiesTypeDef,
-    CustomConnectorSourcePropertiesTypeDef,
     CustomerProfilesDestinationPropertiesTypeDef,
     DatadogSourcePropertiesTypeDef,
     DeleteConnectorProfileRequestRequestTypeDef,
     DeleteFlowRequestRequestTypeDef,
     DescribeConnectorEntityRequestRequestTypeDef,
     DescribeConnectorProfilesRequestRequestTypeDef,
     DescribeConnectorRequestRequestTypeDef,
@@ -406,60 +411,61 @@
     GoogleAnalyticsSourcePropertiesTypeDef,
     IncrementalPullConfigTypeDef,
     InforNexusSourcePropertiesTypeDef,
     ListConnectorEntitiesRequestRequestTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListFlowsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MarketoSourcePropertiesTypeDef,
     RegistrationOutputTypeDef,
     OAuth2CustomParameterTypeDef,
     OAuthPropertiesTypeDef,
     PardotSourcePropertiesTypeDef,
     PrefixConfigTypeDef,
+    RegisterConnectorResponseTypeDef,
+    ResetConnectorMetadataCacheRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     S3InputFormatConfigTypeDef,
     SuccessResponseHandlingConfigTypeDef,
     SAPODataSourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     SingularSourcePropertiesTypeDef,
     SlackSourcePropertiesTypeDef,
     TrendmicroSourcePropertiesTypeDef,
     VeevaSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     StartFlowRequestRequestTypeDef,
+    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
+    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UnregisterConnectorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectorProfileResponseTypeDef,
+    UpdateConnectorRegistrationResponseTypeDef,
+    UpdateFlowResponseTypeDef,
     CustomAuthConfigTypeDef,
+    CustomConnectorSourcePropertiesTypeDef,
+    ListConnectorsResponseTypeDef,
+    ListConnectorEntitiesResponseTypeDef,
     ConnectorMetadataTypeDef,
     GoogleAnalyticsConnectorProfileCredentialsTypeDef,
     HoneycodeConnectorProfileCredentialsTypeDef,
     MarketoConnectorProfileCredentialsTypeDef,
     OAuth2CredentialsTypeDef,
     OAuthCredentialsTypeDef,
     PardotConnectorProfileCredentialsTypeDef,
     SalesforceConnectorProfileCredentialsTypeDef,
     SlackConnectorProfileCredentialsTypeDef,
     ZendeskConnectorProfileCredentialsTypeDef,
     TaskTypeDef,
     ConnectorProvisioningConfigTypeDef,
-    CreateConnectorProfileResponseTypeDef,
-    CreateFlowResponseTypeDef,
-    ListConnectorEntitiesResponseTypeDef,
-    ListConnectorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterConnectorResponseTypeDef,
-    StartFlowResponseTypeDef,
-    StopFlowResponseTypeDef,
-    UpdateConnectorProfileResponseTypeDef,
-    UpdateConnectorRegistrationResponseTypeDef,
-    UpdateFlowResponseTypeDef,
     CustomConnectorDestinationPropertiesTypeDef,
     EventBridgeDestinationPropertiesTypeDef,
     HoneycodeDestinationPropertiesTypeDef,
     MarketoDestinationPropertiesTypeDef,
     RedshiftDestinationPropertiesTypeDef,
     SalesforceDestinationPropertiesTypeDef,
     SnowflakeDestinationPropertiesTypeDef,
@@ -518,42 +524,42 @@
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

### Comparing `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.27.0/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.26.78/setup.py` & `mypy-boto3-appflow-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-appflow.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.26.78",
+    version="1.27.0",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Appflow 1.26.78 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.Appflow 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/",
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


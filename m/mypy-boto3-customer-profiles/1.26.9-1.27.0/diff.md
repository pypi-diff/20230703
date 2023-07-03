# Comparing `tmp/mypy-boto3-customer-profiles-1.26.9.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.26.9.tar", last modified: Mon Nov 14 20:49:29 2022, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.27.0.tar", last modified: Mon Jul  3 19:50:36 2023, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.26.9.tar` & `mypy-boto3-customer-profiles-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.644561 mypy-boto3-customer-profiles-1.26.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17430 2022-11-14 20:49:29.644561 mypy-boto3-customer-profiles-1.26.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15956 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.636561 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30393 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    30348 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11330 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    11328 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    49140 2022-11-14 20:48:53.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    49072 2022-11-14 20:48:52.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.640561 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17430 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 20:49:29.648561 mypy-boto3-customer-profiles-1.26.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-14 20:48:50.000000 mypy-boto3-customer-profiles-1.26.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.923078 mypy-boto3-customer-profiles-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-03 19:50:36.919078 mypy-boto3-customer-profiles-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.919078 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38754 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38697 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-03 19:35:11.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63019 2023-07-03 19:35:13.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-07-03 19:35:11.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:36.919078 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-03 19:50:36.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:50:36.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:36.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:36.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:36.000000 mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:36.923078 mypy-boto3-customer-profiles-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:35:10.000000 mypy-boto3-customer-profiles-1.27.0/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/LICENSE` & `mypy-boto3-customer-profiles-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-customer-profiles-1.26.9/PKG-INFO` & `mypy-boto3-customer-profiles-1.27.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-customer-profiles
-Version: 1.26.9
-Summary: Type annotations for boto3.CustomerProfiles 1.26.9 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-customer-profiles"></a>
 
 # mypy-boto3-customer-profiles
 
 [![PyPI - mypy-boto3-customer-profiles](https://img.shields.io/pypi/v/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +40,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -267,46 +237,73 @@
 from mypy_boto3_customer_profiles import CustomerProfilesClient
 
 client: CustomerProfilesClient = Session().client("customer-profiles")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_customer_profiles.paginator` module contains type annotations for
+all paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_customer_profiles import CustomerProfilesClient
+from mypy_boto3_customer_profiles.paginator import ListEventStreamsPaginator
+
+client: CustomerProfilesClient = Session().client("customer-profiles")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_event_streams_paginator: ListEventStreamsPaginator = client.get_paginator("list_event_streams")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_customer_profiles.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_customer_profiles.literals import (
     ConflictResolvingModelType,
     DataPullModeType,
+    EventStreamDestinationStatusType,
+    EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
+    ListEventStreamsPaginatorName,
     MarketoConnectorOperatorType,
     OperatorPropertiesKeysType,
+    OperatorType,
     PartyTypeType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
+    StatisticType,
     StatusType,
     TaskTypeType,
     TriggerTypeType,
+    UnitType,
     WorkflowTypeType,
     ZendeskConnectorOperatorType,
     logicalOperatorType,
     CustomerProfilesServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: ConflictResolvingModelType) -> bool:
     ...
 ```
@@ -317,121 +314,153 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfileKeyResponseTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
+    AttributeItemTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    RangeTypeDef,
+    ThresholdTypeDef,
     ConnectorOperatorTypeDef,
+    CreateEventStreamRequestRequestTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
+    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
+    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
+    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
+    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
+    DestinationSummaryTypeDef,
     DomainStatsTypeDef,
+    EventStreamDestinationDetailsTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeDefinitionRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
+    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
+    ListCalculatedAttributeDefinitionItemTypeDef,
+    ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+    ListCalculatedAttributeForProfileItemTypeDef,
+    ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
+    MergeProfilesResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
+    PutProfileObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
-    AddProfileKeyResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DeleteIntegrationResponseTypeDef,
-    DeleteProfileKeyResponseTypeDef,
-    DeleteProfileObjectResponseTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
-    DeleteProfileResponseTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
-    GetIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MergeProfilesResponseTypeDef,
-    PutIntegrationResponseTypeDef,
-    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
+    AttributeDetailsTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    ConditionsTypeDef,
     TaskTypeDef,
+    EventStreamSummaryTypeDef,
+    GetEventStreamResponseTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
+    ListCalculatedAttributeDefinitionsResponseTypeDef,
+    ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    CreateCalculatedAttributeDefinitionResponseTypeDef,
+    GetCalculatedAttributeDefinitionResponseTypeDef,
+    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
+    ListEventStreamsResponseTypeDef,
     MatchingRequestTypeDef,
     MatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
@@ -456,42 +485,42 @@
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

### Comparing `mypy-boto3-customer-profiles-1.26.9/README.md` & `mypy-boto3-customer-profiles-1.27.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-customer-profiles
+Version: 1.27.0
+Summary: Type annotations for boto3.CustomerProfiles 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-customer-profiles"></a>
 
 # mypy-boto3-customer-profiles
 
 [![PyPI - mypy-boto3-customer-profiles](https://img.shields.io/pypi/v/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -236,46 +269,73 @@
 from mypy_boto3_customer_profiles import CustomerProfilesClient
 
 client: CustomerProfilesClient = Session().client("customer-profiles")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_customer_profiles.paginator` module contains type annotations for
+all paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_customer_profiles import CustomerProfilesClient
+from mypy_boto3_customer_profiles.paginator import ListEventStreamsPaginator
+
+client: CustomerProfilesClient = Session().client("customer-profiles")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_event_streams_paginator: ListEventStreamsPaginator = client.get_paginator("list_event_streams")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_customer_profiles.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_customer_profiles.literals import (
     ConflictResolvingModelType,
     DataPullModeType,
+    EventStreamDestinationStatusType,
+    EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
+    ListEventStreamsPaginatorName,
     MarketoConnectorOperatorType,
     OperatorPropertiesKeysType,
+    OperatorType,
     PartyTypeType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
+    StatisticType,
     StatusType,
     TaskTypeType,
     TriggerTypeType,
+    UnitType,
     WorkflowTypeType,
     ZendeskConnectorOperatorType,
     logicalOperatorType,
     CustomerProfilesServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: ConflictResolvingModelType) -> bool:
     ...
 ```
@@ -286,121 +346,153 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfileKeyResponseTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
+    AttributeItemTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    RangeTypeDef,
+    ThresholdTypeDef,
     ConnectorOperatorTypeDef,
+    CreateEventStreamRequestRequestTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
+    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
+    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
+    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
+    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
+    DestinationSummaryTypeDef,
     DomainStatsTypeDef,
+    EventStreamDestinationDetailsTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeDefinitionRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
+    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
+    ListCalculatedAttributeDefinitionItemTypeDef,
+    ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+    ListCalculatedAttributeForProfileItemTypeDef,
+    ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
+    MergeProfilesResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
+    PutProfileObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
-    AddProfileKeyResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DeleteIntegrationResponseTypeDef,
-    DeleteProfileKeyResponseTypeDef,
-    DeleteProfileObjectResponseTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
-    DeleteProfileResponseTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
-    GetIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MergeProfilesResponseTypeDef,
-    PutIntegrationResponseTypeDef,
-    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
+    AttributeDetailsTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    ConditionsTypeDef,
     TaskTypeDef,
+    EventStreamSummaryTypeDef,
+    GetEventStreamResponseTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
+    ListCalculatedAttributeDefinitionsResponseTypeDef,
+    ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    CreateCalculatedAttributeDefinitionResponseTypeDef,
+    GetCalculatedAttributeDefinitionResponseTypeDef,
+    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
+    ListEventStreamsResponseTypeDef,
     MatchingRequestTypeDef,
     MatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
@@ -425,42 +517,42 @@
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

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.26.9\nVersion:         1.26.9\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.9")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,44 +15,55 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import GenderType, PartyTypeType, StatusType, logicalOperatorType
+from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
+from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
+    AttributeDetailsTypeDef,
+    ConditionsTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileResponseTypeDef,
     FieldSourceProfileIdsTypeDef,
     FlowDefinitionTypeDef,
     GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeDefinitionResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainResponseTypeDef,
+    GetEventStreamResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     GetIntegrationResponseTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
     IntegrationConfigTypeDef,
     ListAccountIntegrationsResponseTypeDef,
+    ListCalculatedAttributeDefinitionsResponseTypeDef,
+    ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
@@ -62,14 +73,15 @@
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     SearchProfilesResponseTypeDef,
     UpdateAddressTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -136,14 +148,33 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#close)
         """
 
+    def create_calculated_attribute_definition(
+        self,
+        *,
+        DomainName: str,
+        CalculatedAttributeName: str,
+        AttributeDetails: AttributeDetailsTypeDef,
+        Statistic: StatisticType,
+        DisplayName: str = ...,
+        Description: str = ...,
+        Conditions: ConditionsTypeDef = ...,
+        Tags: Mapping[str, str] = ...
+    ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
+        """
+        Creates a new calculated attribute definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_calculated_attribute_definition)
+        """
+
     def create_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
@@ -154,14 +185,25 @@
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_domain)
         """
 
+    def create_event_stream(
+        self, *, DomainName: str, Uri: str, EventStreamName: str, Tags: Mapping[str, str] = ...
+    ) -> CreateEventStreamResponseTypeDef:
+        """
+        Creates an event stream, which is a subscription to real-time events, such as
+        when profiles are created and updated through Amazon Connect Customer Profiles.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_event_stream)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_event_stream)
+        """
+
     def create_integration_workflow(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"],
         IntegrationConfig: IntegrationConfigTypeDef,
         ObjectTypeName: str,
@@ -195,32 +237,52 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
         MailingAddress: AddressTypeDef = ...,
         BillingAddress: AddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...
+        Attributes: Mapping[str, str] = ...,
+        PartyTypeString: str = ...,
+        GenderString: str = ...
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_profile)
         """
 
+    def delete_calculated_attribute_definition(
+        self, *, DomainName: str, CalculatedAttributeName: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes an existing calculated attribute definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_calculated_attribute_definition)
+        """
+
     def delete_domain(self, *, DomainName: str) -> DeleteDomainResponseTypeDef:
         """
         Deletes a specific domain and all of its customer data, such as customer profile
         attributes and their related objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_domain)
         """
 
+    def delete_event_stream(self, *, DomainName: str, EventStreamName: str) -> Dict[str, Any]:
+        """
+        Disables and deletes the specified event stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_event_stream)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_event_stream)
+        """
+
     def delete_integration(self, *, DomainName: str, Uri: str) -> DeleteIntegrationResponseTypeDef:
         """
         Removes an integration from a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_integration)
         """
@@ -298,22 +360,53 @@
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_auto_merging_preview)
         """
 
+    def get_calculated_attribute_definition(
+        self, *, DomainName: str, CalculatedAttributeName: str
+    ) -> GetCalculatedAttributeDefinitionResponseTypeDef:
+        """
+        Provides more information on a calculated attribute definition for Customer
+        Profiles.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_definition)
+        """
+
+    def get_calculated_attribute_for_profile(
+        self, *, DomainName: str, ProfileId: str, CalculatedAttributeName: str
+    ) -> GetCalculatedAttributeForProfileResponseTypeDef:
+        """
+        Retrieve a calculated attribute for a customer profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_for_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_for_profile)
+        """
+
     def get_domain(self, *, DomainName: str) -> GetDomainResponseTypeDef:
         """
         Returns information about a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_domain)
         """
 
+    def get_event_stream(
+        self, *, DomainName: str, EventStreamName: str
+    ) -> GetEventStreamResponseTypeDef:
+        """
+        Returns information about the specified event stream in a specific domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_event_stream)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_event_stream)
+        """
+
     def get_identity_resolution_job(
         self, *, DomainName: str, JobId: str
     ) -> GetIdentityResolutionJobResponseTypeDef:
         """
         Returns information about an Identity Resolution Job in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_identity_resolution_job)
@@ -386,24 +479,56 @@
         """
         Lists all of the integrations associated to a specific URI in the AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_account_integrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_account_integrations)
         """
 
+    def list_calculated_attribute_definitions(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListCalculatedAttributeDefinitionsResponseTypeDef:
+        """
+        Lists calculated attribute definitions for Customer Profiles See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/customer-
+        profiles-2020-08-15/ListCalculatedAttributeDefinitions).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attribute_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attribute_definitions)
+        """
+
+    def list_calculated_attributes_for_profile(
+        self, *, DomainName: str, ProfileId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListCalculatedAttributesForProfileResponseTypeDef:
+        """
+        Retrieve a list of calculated attributes for a customer profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attributes_for_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attributes_for_profile)
+        """
+
     def list_domains(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDomainsResponseTypeDef:
         """
         Returns a list of all the domains for an AWS account that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_domains)
         """
 
+    def list_event_streams(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListEventStreamsResponseTypeDef:
+        """
+        Returns a list of all the event streams in a specific domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_event_streams)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_event_streams)
+        """
+
     def list_identity_resolution_jobs(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListIdentityResolutionJobsResponseTypeDef:
         """
         Lists all of the Identity Resolution Jobs in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_identity_resolution_jobs)
@@ -494,15 +619,15 @@
         *,
         DomainName: str,
         MainProfileId: str,
         ProfileIdsToBeMerged: Sequence[str],
         FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...
     ) -> MergeProfilesResponseTypeDef:
         """
-        Runs an AWS Lambda job that does the following * All the profileKeys in the
+        Runs an AWS Lambda job that does the following: * All the profileKeys in the
         `ProfileToBeMerged` will be moved to the main profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#merge_profiles)
         """
 
     def put_integration(
@@ -589,14 +714,30 @@
         Removes one or more tags from the specified Amazon Connect Customer Profiles
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#untag_resource)
         """
 
+    def update_calculated_attribute_definition(
+        self,
+        *,
+        DomainName: str,
+        CalculatedAttributeName: str,
+        DisplayName: str = ...,
+        Description: str = ...,
+        Conditions: ConditionsTypeDef = ...
+    ) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:
+        """
+        Updates an existing calculated attribute definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_calculated_attribute_definition)
+        """
+
     def update_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
@@ -632,15 +773,25 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: UpdateAddressTypeDef = ...,
         ShippingAddress: UpdateAddressTypeDef = ...,
         MailingAddress: UpdateAddressTypeDef = ...,
         BillingAddress: UpdateAddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...
+        Attributes: Mapping[str, str] = ...,
+        PartyTypeString: str = ...,
+        GenderString: str = ...
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_profile)
         """
+
+    def get_paginator(
+        self, operation_name: Literal["list_event_streams"]
+    ) -> ListEventStreamsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/client.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -15,44 +15,55 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import GenderType, PartyTypeType, StatusType, logicalOperatorType
+from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
+from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
+    AttributeDetailsTypeDef,
+    ConditionsTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
+    CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileResponseTypeDef,
     FieldSourceProfileIdsTypeDef,
     FlowDefinitionTypeDef,
     GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeDefinitionResponseTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainResponseTypeDef,
+    GetEventStreamResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     GetIntegrationResponseTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
     IntegrationConfigTypeDef,
     ListAccountIntegrationsResponseTypeDef,
+    ListCalculatedAttributeDefinitionsResponseTypeDef,
+    ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
+    ListEventStreamsResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
@@ -62,14 +73,15 @@
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     SearchProfilesResponseTypeDef,
     UpdateAddressTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -128,14 +140,32 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#close)
         """
+    def create_calculated_attribute_definition(
+        self,
+        *,
+        DomainName: str,
+        CalculatedAttributeName: str,
+        AttributeDetails: AttributeDetailsTypeDef,
+        Statistic: StatisticType,
+        DisplayName: str = ...,
+        Description: str = ...,
+        Conditions: ConditionsTypeDef = ...,
+        Tags: Mapping[str, str] = ...
+    ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
+        """
+        Creates a new calculated attribute definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_calculated_attribute_definition)
+        """
     def create_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
@@ -145,14 +175,24 @@
         """
         Creates a domain, which is a container for all customer data, such as customer
         profile attributes, object types, profile keys, and encryption keys.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_domain)
         """
+    def create_event_stream(
+        self, *, DomainName: str, Uri: str, EventStreamName: str, Tags: Mapping[str, str] = ...
+    ) -> CreateEventStreamResponseTypeDef:
+        """
+        Creates an event stream, which is a subscription to real-time events, such as
+        when profiles are created and updated through Amazon Connect Customer Profiles.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_event_stream)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_event_stream)
+        """
     def create_integration_workflow(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"],
         IntegrationConfig: IntegrationConfigTypeDef,
         ObjectTypeName: str,
@@ -185,30 +225,48 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
         MailingAddress: AddressTypeDef = ...,
         BillingAddress: AddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...
+        Attributes: Mapping[str, str] = ...,
+        PartyTypeString: str = ...,
+        GenderString: str = ...
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_profile)
         """
+    def delete_calculated_attribute_definition(
+        self, *, DomainName: str, CalculatedAttributeName: str
+    ) -> Dict[str, Any]:
+        """
+        Deletes an existing calculated attribute definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_calculated_attribute_definition)
+        """
     def delete_domain(self, *, DomainName: str) -> DeleteDomainResponseTypeDef:
         """
         Deletes a specific domain and all of its customer data, such as customer profile
         attributes and their related objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_domain)
         """
+    def delete_event_stream(self, *, DomainName: str, EventStreamName: str) -> Dict[str, Any]:
+        """
+        Disables and deletes the specified event stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_event_stream)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_event_stream)
+        """
     def delete_integration(self, *, DomainName: str, Uri: str) -> DeleteIntegrationResponseTypeDef:
         """
         Removes an integration from a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#delete_integration)
         """
@@ -278,21 +336,49 @@
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_auto_merging_preview)
         """
+    def get_calculated_attribute_definition(
+        self, *, DomainName: str, CalculatedAttributeName: str
+    ) -> GetCalculatedAttributeDefinitionResponseTypeDef:
+        """
+        Provides more information on a calculated attribute definition for Customer
+        Profiles.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_definition)
+        """
+    def get_calculated_attribute_for_profile(
+        self, *, DomainName: str, ProfileId: str, CalculatedAttributeName: str
+    ) -> GetCalculatedAttributeForProfileResponseTypeDef:
+        """
+        Retrieve a calculated attribute for a customer profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_for_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_calculated_attribute_for_profile)
+        """
     def get_domain(self, *, DomainName: str) -> GetDomainResponseTypeDef:
         """
         Returns information about a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_domain)
         """
+    def get_event_stream(
+        self, *, DomainName: str, EventStreamName: str
+    ) -> GetEventStreamResponseTypeDef:
+        """
+        Returns information about the specified event stream in a specific domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_event_stream)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_event_stream)
+        """
     def get_identity_resolution_job(
         self, *, DomainName: str, JobId: str
     ) -> GetIdentityResolutionJobResponseTypeDef:
         """
         Returns information about an Identity Resolution Job in a specific domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_identity_resolution_job)
@@ -357,23 +443,52 @@
     ) -> ListAccountIntegrationsResponseTypeDef:
         """
         Lists all of the integrations associated to a specific URI in the AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_account_integrations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_account_integrations)
         """
+    def list_calculated_attribute_definitions(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListCalculatedAttributeDefinitionsResponseTypeDef:
+        """
+        Lists calculated attribute definitions for Customer Profiles See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/customer-
+        profiles-2020-08-15/ListCalculatedAttributeDefinitions).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attribute_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attribute_definitions)
+        """
+    def list_calculated_attributes_for_profile(
+        self, *, DomainName: str, ProfileId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListCalculatedAttributesForProfileResponseTypeDef:
+        """
+        Retrieve a list of calculated attributes for a customer profile.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attributes_for_profile)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_calculated_attributes_for_profile)
+        """
     def list_domains(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDomainsResponseTypeDef:
         """
         Returns a list of all the domains for an AWS account that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_domains)
         """
+    def list_event_streams(
+        self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListEventStreamsResponseTypeDef:
+        """
+        Returns a list of all the event streams in a specific domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_event_streams)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#list_event_streams)
+        """
     def list_identity_resolution_jobs(
         self, *, DomainName: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListIdentityResolutionJobsResponseTypeDef:
         """
         Lists all of the Identity Resolution Jobs in your domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_identity_resolution_jobs)
@@ -457,15 +572,15 @@
         *,
         DomainName: str,
         MainProfileId: str,
         ProfileIdsToBeMerged: Sequence[str],
         FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...
     ) -> MergeProfilesResponseTypeDef:
         """
-        Runs an AWS Lambda job that does the following * All the profileKeys in the
+        Runs an AWS Lambda job that does the following: * All the profileKeys in the
         `ProfileToBeMerged` will be moved to the main profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#merge_profiles)
         """
     def put_integration(
         self,
@@ -545,14 +660,29 @@
         """
         Removes one or more tags from the specified Amazon Connect Customer Profiles
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#untag_resource)
         """
+    def update_calculated_attribute_definition(
+        self,
+        *,
+        DomainName: str,
+        CalculatedAttributeName: str,
+        DisplayName: str = ...,
+        Description: str = ...,
+        Conditions: ConditionsTypeDef = ...
+    ) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:
+        """
+        Updates an existing calculated attribute definition.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_calculated_attribute_definition)
+        """
     def update_domain(
         self,
         *,
         DomainName: str,
         DefaultExpirationDays: int = ...,
         DefaultEncryptionKey: str = ...,
         DeadLetterQueueUrl: str = ...,
@@ -587,15 +717,24 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: UpdateAddressTypeDef = ...,
         ShippingAddress: UpdateAddressTypeDef = ...,
         MailingAddress: UpdateAddressTypeDef = ...,
         BillingAddress: UpdateAddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...
+        Attributes: Mapping[str, str] = ...,
+        PartyTypeString: str = ...,
+        GenderString: str = ...
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_profile)
         """
+    def get_paginator(
+        self, operation_name: Literal["list_event_streams"]
+    ) -> ListEventStreamsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/literals.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,49 +18,59 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "ConflictResolvingModelType",
     "DataPullModeType",
+    "EventStreamDestinationStatusType",
+    "EventStreamStateType",
     "FieldContentTypeType",
     "GenderType",
     "IdentityResolutionJobStatusType",
     "JobScheduleDayOfTheWeekType",
+    "ListEventStreamsPaginatorName",
     "MarketoConnectorOperatorType",
     "OperatorPropertiesKeysType",
+    "OperatorType",
     "PartyTypeType",
     "S3ConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "ServiceNowConnectorOperatorType",
     "SourceConnectorTypeType",
     "StandardIdentifierType",
+    "StatisticType",
     "StatusType",
     "TaskTypeType",
     "TriggerTypeType",
+    "UnitType",
     "WorkflowTypeType",
     "ZendeskConnectorOperatorType",
     "logicalOperatorType",
     "CustomerProfilesServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
+EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
+EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
 IdentityResolutionJobStatusType = Literal[
     "COMPLETED", "FAILED", "FIND_MATCHING", "MERGING", "PARTIAL_SUCCESS", "PENDING", "PREPROCESSING"
 ]
 JobScheduleDayOfTheWeekType = Literal[
     "FRIDAY", "MONDAY", "SATURDAY", "SUNDAY", "THURSDAY", "TUESDAY", "WEDNESDAY"
 ]
+ListEventStreamsPaginatorName = Literal["list_event_streams"]
 MarketoConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "GREATER_THAN",
     "LESS_THAN",
     "MASK_ALL",
@@ -87,14 +97,15 @@
     "SUBFIELD_CATEGORY_MAP",
     "TRUNCATE_LENGTH",
     "UPPER_BOUND",
     "VALIDATION_ACTION",
     "VALUE",
     "VALUES",
 ]
+OperatorType = Literal["EQUAL_TO", "GREATER_THAN", "LESS_THAN", "NOT_EQUAL_TO"]
 PartyTypeType = Literal["BUSINESS", "INDIVIDUAL", "OTHER"]
 S3ConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "GREATER_THAN",
@@ -160,19 +171,30 @@
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
 SourceConnectorTypeType = Literal["Marketo", "S3", "Salesforce", "Servicenow", "Zendesk"]
 StandardIdentifierType = Literal[
     "ASSET", "CASE", "LOOKUP_ONLY", "NEW_ONLY", "ORDER", "PROFILE", "SECONDARY", "UNIQUE"
 ]
+StatisticType = Literal[
+    "AVERAGE",
+    "COUNT",
+    "FIRST_OCCURRENCE",
+    "LAST_OCCURRENCE",
+    "MAXIMUM",
+    "MAX_OCCURRENCE",
+    "MINIMUM",
+    "SUM",
+]
 StatusType = Literal[
     "CANCELLED", "COMPLETE", "FAILED", "IN_PROGRESS", "NOT_STARTED", "RETRY", "SPLIT"
 ]
 TaskTypeType = Literal["Arithmetic", "Filter", "Map", "Mask", "Merge", "Truncate", "Validate"]
 TriggerTypeType = Literal["Event", "OnDemand", "Scheduled"]
+UnitType = Literal["DAYS"]
 WorkflowTypeType = Literal["APPFLOW_INTEGRATION"]
 ZendeskConnectorOperatorType = Literal[
     "ADDITION",
     "DIVISION",
     "GREATER_THAN",
     "MASK_ALL",
     "MASK_FIRST_N",
@@ -199,23 +221,25 @@
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
@@ -225,30 +249,35 @@
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
@@ -274,14 +303,15 @@
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
@@ -326,51 +356,57 @@
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
@@ -383,14 +419,15 @@
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
@@ -402,28 +439,35 @@
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
@@ -451,56 +495,64 @@
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
@@ -518,14 +570,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_event_streams"]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -17,48 +17,58 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ConflictResolvingModelType",
     "DataPullModeType",
+    "EventStreamDestinationStatusType",
+    "EventStreamStateType",
     "FieldContentTypeType",
     "GenderType",
     "IdentityResolutionJobStatusType",
     "JobScheduleDayOfTheWeekType",
+    "ListEventStreamsPaginatorName",
     "MarketoConnectorOperatorType",
     "OperatorPropertiesKeysType",
+    "OperatorType",
     "PartyTypeType",
     "S3ConnectorOperatorType",
     "SalesforceConnectorOperatorType",
     "ServiceNowConnectorOperatorType",
     "SourceConnectorTypeType",
     "StandardIdentifierType",
+    "StatisticType",
     "StatusType",
     "TaskTypeType",
     "TriggerTypeType",
+    "UnitType",
     "WorkflowTypeType",
     "ZendeskConnectorOperatorType",
     "logicalOperatorType",
     "CustomerProfilesServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 ConflictResolvingModelType = Literal["RECENCY", "SOURCE"]
 DataPullModeType = Literal["Complete", "Incremental"]
+EventStreamDestinationStatusType = Literal["HEALTHY", "UNHEALTHY"]
+EventStreamStateType = Literal["RUNNING", "STOPPED"]
 FieldContentTypeType = Literal["EMAIL_ADDRESS", "NAME", "NUMBER", "PHONE_NUMBER", "STRING"]
 GenderType = Literal["FEMALE", "MALE", "UNSPECIFIED"]
 IdentityResolutionJobStatusType = Literal[
     "COMPLETED", "FAILED", "FIND_MATCHING", "MERGING", "PARTIAL_SUCCESS", "PENDING", "PREPROCESSING"
 ]
 JobScheduleDayOfTheWeekType = Literal[
     "FRIDAY", "MONDAY", "SATURDAY", "SUNDAY", "THURSDAY", "TUESDAY", "WEDNESDAY"
 ]
+ListEventStreamsPaginatorName = Literal["list_event_streams"]
 MarketoConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "GREATER_THAN",
     "LESS_THAN",
     "MASK_ALL",
@@ -85,14 +95,15 @@
     "SUBFIELD_CATEGORY_MAP",
     "TRUNCATE_LENGTH",
     "UPPER_BOUND",
     "VALIDATION_ACTION",
     "VALUE",
     "VALUES",
 ]
+OperatorType = Literal["EQUAL_TO", "GREATER_THAN", "LESS_THAN", "NOT_EQUAL_TO"]
 PartyTypeType = Literal["BUSINESS", "INDIVIDUAL", "OTHER"]
 S3ConnectorOperatorType = Literal[
     "ADDITION",
     "BETWEEN",
     "DIVISION",
     "EQUAL_TO",
     "GREATER_THAN",
@@ -158,19 +169,30 @@
     "VALIDATE_NON_ZERO",
     "VALIDATE_NUMERIC",
 ]
 SourceConnectorTypeType = Literal["Marketo", "S3", "Salesforce", "Servicenow", "Zendesk"]
 StandardIdentifierType = Literal[
     "ASSET", "CASE", "LOOKUP_ONLY", "NEW_ONLY", "ORDER", "PROFILE", "SECONDARY", "UNIQUE"
 ]
+StatisticType = Literal[
+    "AVERAGE",
+    "COUNT",
+    "FIRST_OCCURRENCE",
+    "LAST_OCCURRENCE",
+    "MAXIMUM",
+    "MAX_OCCURRENCE",
+    "MINIMUM",
+    "SUM",
+]
 StatusType = Literal[
     "CANCELLED", "COMPLETE", "FAILED", "IN_PROGRESS", "NOT_STARTED", "RETRY", "SPLIT"
 ]
 TaskTypeType = Literal["Arithmetic", "Filter", "Map", "Mask", "Merge", "Truncate", "Validate"]
 TriggerTypeType = Literal["Event", "OnDemand", "Scheduled"]
+UnitType = Literal["DAYS"]
 WorkflowTypeType = Literal["APPFLOW_INTEGRATION"]
 ZendeskConnectorOperatorType = Literal[
     "ADDITION",
     "DIVISION",
     "GREATER_THAN",
     "MASK_ALL",
     "MASK_FIRST_N",
@@ -197,23 +219,25 @@
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
@@ -223,30 +247,35 @@
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
@@ -272,14 +301,15 @@
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
@@ -324,51 +354,57 @@
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
@@ -381,14 +417,15 @@
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
@@ -400,28 +437,35 @@
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
@@ -449,56 +493,64 @@
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
@@ -516,14 +568,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_event_streams"]
 RegionName = Literal[
     "af-south-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ConflictResolvingModelType,
     DataPullModeType,
+    EventStreamDestinationStatusType,
+    EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     MarketoConnectorOperatorType,
     OperatorPropertiesKeysType,
+    OperatorType,
     PartyTypeType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
+    StatisticType,
     StatusType,
     TaskTypeType,
     TriggerTypeType,
     ZendeskConnectorOperatorType,
     logicalOperatorType,
 )
 
@@ -45,121 +49,153 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddProfileKeyResponseTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
+    "AttributeItemTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationTypeDef",
+    "RangeTypeDef",
+    "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
+    "CreateEventStreamRequestRequestTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
+    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
+    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
+    "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
+    "EventStreamDestinationDetailsTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
+    "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "GetCalculatedAttributeForProfileRequestRequestTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
+    "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
+    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
+    "ListCalculatedAttributeDefinitionItemTypeDef",
+    "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
+    "ListCalculatedAttributeForProfileItemTypeDef",
+    "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
+    "MergeProfilesResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutIntegrationResponseTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
+    "PutProfileObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
-    "AddProfileKeyResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
-    "DeleteDomainResponseTypeDef",
-    "DeleteIntegrationResponseTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
-    "DeleteProfileResponseTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
-    "GetIntegrationResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "PutIntegrationResponseTypeDef",
-    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
+    "AttributeDetailsTypeDef",
     "AutoMergingTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
+    "ConditionsTypeDef",
     "TaskTypeDef",
+    "EventStreamSummaryTypeDef",
+    "GetEventStreamResponseTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
     "PutProfileObjectTypeRequestRequestTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
+    "ListCalculatedAttributeDefinitionsResponseTypeDef",
+    "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TriggerPropertiesTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
+    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
+    "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+    "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "TriggerConfigTypeDef",
     "SourceFlowConfigTypeDef",
@@ -182,22 +218,20 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
@@ -272,14 +306,21 @@
         "BatchRecordsStartTime": str,
         "BatchRecordsEndTime": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
+AttributeItemTypeDef = TypedDict(
+    "AttributeItemTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -300,96 +341,270 @@
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
+    {
+        "Value": int,
+        "Unit": Literal["DAYS"],
+    },
+)
+
+ThresholdTypeDef = TypedDict(
+    "ThresholdTypeDef",
+    {
+        "Value": str,
+        "Operator": OperatorType,
+    },
+)
+
 ConnectorOperatorTypeDef = TypedDict(
     "ConnectorOperatorTypeDef",
     {
         "Marketo": MarketoConnectorOperatorType,
         "S3": S3ConnectorOperatorType,
         "Salesforce": SalesforceConnectorOperatorType,
         "ServiceNow": ServiceNowConnectorOperatorType,
         "Zendesk": ZendeskConnectorOperatorType,
     },
     total=False,
 )
 
+_RequiredCreateEventStreamRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventStreamRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "EventStreamName": str,
+    },
+)
+_OptionalCreateEventStreamRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventStreamRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateEventStreamRequestRequestTypeDef(
+    _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
+):
+    pass
+
+
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+    },
+)
+
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteEventStreamRequestRequestTypeDef = TypedDict(
+    "DeleteEventStreamRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamName": str,
+    },
+)
+
 DeleteIntegrationRequestRequestTypeDef = TypedDict(
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
 
+_RequiredDestinationSummaryTypeDef = TypedDict(
+    "_RequiredDestinationSummaryTypeDef",
+    {
+        "Uri": str,
+        "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalDestinationSummaryTypeDef = TypedDict(
+    "_OptionalDestinationSummaryTypeDef",
+    {
+        "UnhealthySince": datetime,
+    },
+    total=False,
+)
+
+
+class DestinationSummaryTypeDef(
+    _RequiredDestinationSummaryTypeDef, _OptionalDestinationSummaryTypeDef
+):
+    pass
+
+
 DomainStatsTypeDef = TypedDict(
     "DomainStatsTypeDef",
     {
         "ProfileCount": int,
         "MeteringProfileCount": int,
         "ObjectCount": int,
         "TotalSize": int,
     },
     total=False,
 )
 
+_RequiredEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_RequiredEventStreamDestinationDetailsTypeDef",
+    {
+        "Uri": str,
+        "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_OptionalEventStreamDestinationDetailsTypeDef",
+    {
+        "UnhealthySince": datetime,
+        "Message": str,
+    },
+    total=False,
+)
+
+
+class EventStreamDestinationDetailsTypeDef(
+    _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
+):
+    pass
+
+
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalS3ExportingConfigTypeDef = TypedDict(
@@ -449,21 +664,68 @@
     {
         "KeyName": str,
         "Values": List[str],
     },
     total=False,
 )
 
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+    },
+)
+
+GetCalculatedAttributeForProfileRequestRequestTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ProfileId": str,
+        "CalculatedAttributeName": str,
+    },
+)
+
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+GetEventStreamRequestRequestTypeDef = TypedDict(
+    "GetEventStreamRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamName": str,
+    },
+)
+
 GetIdentityResolutionJobRequestRequestTypeDef = TypedDict(
     "GetIdentityResolutionJobRequestRequestTypeDef",
     {
         "DomainName": str,
         "JobId": str,
     },
 )
@@ -482,14 +744,30 @@
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -647,14 +925,85 @@
 
 class ListIntegrationItemTypeDef(
     _RequiredListIntegrationItemTypeDef, _OptionalListIntegrationItemTypeDef
 ):
     pass
 
 
+ListCalculatedAttributeDefinitionItemTypeDef = TypedDict(
+    "ListCalculatedAttributeDefinitionItemTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCalculatedAttributeDefinitionsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListCalculatedAttributeDefinitionsRequestRequestTypeDef(
+    _RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+    _OptionalListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+):
+    pass
+
+
+ListCalculatedAttributeForProfileItemTypeDef = TypedDict(
+    "ListCalculatedAttributeForProfileItemTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ProfileId": str,
+    },
+)
+_OptionalListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalListCalculatedAttributesForProfileRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListCalculatedAttributesForProfileRequestRequestTypeDef(
+    _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef,
+    _OptionalListCalculatedAttributesForProfileRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredListDomainItemTypeDef = TypedDict(
     "_RequiredListDomainItemTypeDef",
     {
         "DomainName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
@@ -677,14 +1026,58 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListEventStreamsRequestRequestTypeDef(
+    _RequiredListEventStreamsRequestRequestTypeDef, _OptionalListEventStreamsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredListIdentityResolutionJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityResolutionJobsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListIdentityResolutionJobsRequestRequestTypeDef = TypedDict(
@@ -814,14 +1207,22 @@
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
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "WorkflowId": str,
         "Status": StatusType,
         "StatusDescription": str,
@@ -859,23 +1260,76 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
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
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
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
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -984,160 +1438,19 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
-    {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
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
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1189,14 +1502,16 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Mapping[str, str],
+        "PartyTypeString": str,
+        "GenderString": str,
     },
     total=False,
 )
 
 
 class CreateProfileRequestRequestTypeDef(
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
@@ -1224,14 +1539,22 @@
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
     total=False,
 )
 
+AttributeDetailsTypeDef = TypedDict(
+    "AttributeDetailsTypeDef",
+    {
+        "Attributes": Sequence[AttributeItemTypeDef],
+        "Expression": str,
+    },
+)
+
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1269,14 +1592,24 @@
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
 
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
+    {
+        "Range": RangeTypeDef,
+        "ObjectCount": int,
+        "Threshold": ThresholdTypeDef,
+    },
+    total=False,
+)
+
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "SourceFields": Sequence[str],
         "TaskType": TaskTypeType,
     },
 )
@@ -1291,14 +1624,54 @@
 )
 
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
 
+_RequiredEventStreamSummaryTypeDef = TypedDict(
+    "_RequiredEventStreamSummaryTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamName": str,
+        "EventStreamArn": str,
+        "State": EventStreamStateType,
+    },
+)
+_OptionalEventStreamSummaryTypeDef = TypedDict(
+    "_OptionalEventStreamSummaryTypeDef",
+    {
+        "StoppedSince": datetime,
+        "DestinationSummary": DestinationSummaryTypeDef,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class EventStreamSummaryTypeDef(
+    _RequiredEventStreamSummaryTypeDef, _OptionalEventStreamSummaryTypeDef
+):
+    pass
+
+
+GetEventStreamResponseTypeDef = TypedDict(
+    "GetEventStreamResponseTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamArn": str,
+        "CreatedAt": datetime,
+        "State": EventStreamStateType,
+        "StoppedSince": datetime,
+        "DestinationDetails": EventStreamDestinationDetailsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
     },
     total=False,
 )
@@ -1356,26 +1729,28 @@
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
+        "PartyTypeString": str,
+        "GenderString": str,
     },
     total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
@@ -1386,29 +1761,29 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1450,69 +1825,87 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
+    "ListCalculatedAttributeDefinitionsResponseTypeDef",
+    {
+        "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
+    "ListCalculatedAttributesForProfileResponseTypeDef",
+    {
+        "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1539,15 +1932,15 @@
 
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
@@ -1594,14 +1987,16 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": UpdateAddressTypeDef,
         "ShippingAddress": UpdateAddressTypeDef,
         "MailingAddress": UpdateAddressTypeDef,
         "BillingAddress": UpdateAddressTypeDef,
         "Attributes": Mapping[str, str],
+        "PartyTypeString": str,
+        "GenderString": str,
     },
     total=False,
 )
 
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
@@ -1616,26 +2011,136 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Statistic": StatisticType,
+    },
+)
+_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "Conditions": ConditionsTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Conditions": ConditionsTypeDef,
+        "Statistic": StatisticType,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
+        "Conditions": ConditionsTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+    },
+)
+_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "Conditions": ConditionsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
+        "Conditions": ConditionsTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEventStreamsResponseTypeDef = TypedDict(
+    "ListEventStreamsResponseTypeDef",
+    {
+        "Items": List[EventStreamSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
@@ -1677,15 +2182,15 @@
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
         "AutoMerging": AutoMergingTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -1701,15 +2206,15 @@
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -1806,15 +2311,15 @@
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainResponseTypeDef = TypedDict(
     "GetDomainResponseTypeDef",
     {
         "DomainName": str,
@@ -1822,39 +2327,39 @@
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Stats": DomainStatsTypeDef,
         "Matching": MatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ConflictResolvingModelType,
     DataPullModeType,
+    EventStreamDestinationStatusType,
+    EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
     MarketoConnectorOperatorType,
     OperatorPropertiesKeysType,
+    OperatorType,
     PartyTypeType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
+    StatisticType,
     StatusType,
     TaskTypeType,
     TriggerTypeType,
     ZendeskConnectorOperatorType,
     logicalOperatorType,
 )
 
@@ -44,121 +48,153 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddProfileKeyResponseTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
+    "AttributeItemTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationTypeDef",
+    "RangeTypeDef",
+    "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
+    "CreateEventStreamRequestRequestTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
+    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
+    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
+    "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
+    "EventStreamDestinationDetailsTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
+    "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "GetCalculatedAttributeForProfileRequestRequestTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
+    "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
+    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
+    "ListCalculatedAttributeDefinitionItemTypeDef",
+    "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
+    "ListCalculatedAttributeForProfileItemTypeDef",
+    "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
+    "MergeProfilesResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutIntegrationResponseTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
+    "PutProfileObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
-    "AddProfileKeyResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
-    "DeleteDomainResponseTypeDef",
-    "DeleteIntegrationResponseTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
-    "DeleteProfileResponseTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
-    "GetIntegrationResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "PutIntegrationResponseTypeDef",
-    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
+    "AttributeDetailsTypeDef",
     "AutoMergingTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
+    "ConditionsTypeDef",
     "TaskTypeDef",
+    "EventStreamSummaryTypeDef",
+    "GetEventStreamResponseTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
     "PutProfileObjectTypeRequestRequestTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
+    "ListCalculatedAttributeDefinitionsResponseTypeDef",
+    "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TriggerPropertiesTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
+    "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
+    "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+    "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
     "TriggerConfigTypeDef",
     "SourceFlowConfigTypeDef",
@@ -181,22 +217,20 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
@@ -269,14 +303,21 @@
         "BatchRecordsStartTime": str,
         "BatchRecordsEndTime": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
+AttributeItemTypeDef = TypedDict(
+    "AttributeItemTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 _RequiredConflictResolutionTypeDef = TypedDict(
     "_RequiredConflictResolutionTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
     },
 )
 _OptionalConflictResolutionTypeDef = TypedDict(
@@ -295,96 +336,264 @@
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
+    {
+        "Value": int,
+        "Unit": Literal["DAYS"],
+    },
+)
+
+ThresholdTypeDef = TypedDict(
+    "ThresholdTypeDef",
+    {
+        "Value": str,
+        "Operator": OperatorType,
+    },
+)
+
 ConnectorOperatorTypeDef = TypedDict(
     "ConnectorOperatorTypeDef",
     {
         "Marketo": MarketoConnectorOperatorType,
         "S3": S3ConnectorOperatorType,
         "Salesforce": SalesforceConnectorOperatorType,
         "ServiceNow": ServiceNowConnectorOperatorType,
         "Zendesk": ZendeskConnectorOperatorType,
     },
     total=False,
 )
 
+_RequiredCreateEventStreamRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventStreamRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "EventStreamName": str,
+    },
+)
+_OptionalCreateEventStreamRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventStreamRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateEventStreamRequestRequestTypeDef(
+    _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
+):
+    pass
+
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+    },
+)
+
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteEventStreamRequestRequestTypeDef = TypedDict(
+    "DeleteEventStreamRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamName": str,
+    },
+)
+
 DeleteIntegrationRequestRequestTypeDef = TypedDict(
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
 
+_RequiredDestinationSummaryTypeDef = TypedDict(
+    "_RequiredDestinationSummaryTypeDef",
+    {
+        "Uri": str,
+        "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalDestinationSummaryTypeDef = TypedDict(
+    "_OptionalDestinationSummaryTypeDef",
+    {
+        "UnhealthySince": datetime,
+    },
+    total=False,
+)
+
+class DestinationSummaryTypeDef(
+    _RequiredDestinationSummaryTypeDef, _OptionalDestinationSummaryTypeDef
+):
+    pass
+
 DomainStatsTypeDef = TypedDict(
     "DomainStatsTypeDef",
     {
         "ProfileCount": int,
         "MeteringProfileCount": int,
         "ObjectCount": int,
         "TotalSize": int,
     },
     total=False,
 )
 
+_RequiredEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_RequiredEventStreamDestinationDetailsTypeDef",
+    {
+        "Uri": str,
+        "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_OptionalEventStreamDestinationDetailsTypeDef",
+    {
+        "UnhealthySince": datetime,
+        "Message": str,
+    },
+    total=False,
+)
+
+class EventStreamDestinationDetailsTypeDef(
+    _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
+):
+    pass
+
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalS3ExportingConfigTypeDef = TypedDict(
@@ -442,21 +651,68 @@
     {
         "KeyName": str,
         "Values": List[str],
     },
     total=False,
 )
 
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+    },
+)
+
+GetCalculatedAttributeForProfileRequestRequestTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ProfileId": str,
+        "CalculatedAttributeName": str,
+    },
+)
+
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+GetEventStreamRequestRequestTypeDef = TypedDict(
+    "GetEventStreamRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamName": str,
+    },
+)
+
 GetIdentityResolutionJobRequestRequestTypeDef = TypedDict(
     "GetIdentityResolutionJobRequestRequestTypeDef",
     {
         "DomainName": str,
         "JobId": str,
     },
 )
@@ -475,14 +731,30 @@
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -632,14 +904,81 @@
 )
 
 class ListIntegrationItemTypeDef(
     _RequiredListIntegrationItemTypeDef, _OptionalListIntegrationItemTypeDef
 ):
     pass
 
+ListCalculatedAttributeDefinitionItemTypeDef = TypedDict(
+    "ListCalculatedAttributeDefinitionItemTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCalculatedAttributeDefinitionsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListCalculatedAttributeDefinitionsRequestRequestTypeDef(
+    _RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+    _OptionalListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+):
+    pass
+
+ListCalculatedAttributeForProfileItemTypeDef = TypedDict(
+    "ListCalculatedAttributeForProfileItemTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ProfileId": str,
+    },
+)
+_OptionalListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalListCalculatedAttributesForProfileRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListCalculatedAttributesForProfileRequestRequestTypeDef(
+    _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef,
+    _OptionalListCalculatedAttributesForProfileRequestRequestTypeDef,
+):
+    pass
+
 _RequiredListDomainItemTypeDef = TypedDict(
     "_RequiredListDomainItemTypeDef",
     {
         "DomainName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
@@ -660,14 +999,54 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListEventStreamsRequestRequestTypeDef(
+    _RequiredListEventStreamsRequestRequestTypeDef, _OptionalListEventStreamsRequestRequestTypeDef
+):
+    pass
+
 _RequiredListIdentityResolutionJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityResolutionJobsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListIdentityResolutionJobsRequestRequestTypeDef = TypedDict(
@@ -789,14 +1168,22 @@
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
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "WorkflowId": str,
         "Status": StatusType,
         "StatusDescription": str,
@@ -832,23 +1219,76 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
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
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
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
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -951,160 +1391,19 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
-    {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
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
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1154,14 +1453,16 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Mapping[str, str],
+        "PartyTypeString": str,
+        "GenderString": str,
     },
     total=False,
 )
 
 class CreateProfileRequestRequestTypeDef(
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
 ):
@@ -1187,14 +1488,22 @@
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
     total=False,
 )
 
+AttributeDetailsTypeDef = TypedDict(
+    "AttributeDetailsTypeDef",
+    {
+        "Attributes": Sequence[AttributeItemTypeDef],
+        "Expression": str,
+    },
+)
+
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1228,14 +1537,24 @@
 
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
+    {
+        "Range": RangeTypeDef,
+        "ObjectCount": int,
+        "Threshold": ThresholdTypeDef,
+    },
+    total=False,
+)
+
 _RequiredTaskTypeDef = TypedDict(
     "_RequiredTaskTypeDef",
     {
         "SourceFields": Sequence[str],
         "TaskType": TaskTypeType,
     },
 )
@@ -1248,14 +1567,52 @@
     },
     total=False,
 )
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
+_RequiredEventStreamSummaryTypeDef = TypedDict(
+    "_RequiredEventStreamSummaryTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamName": str,
+        "EventStreamArn": str,
+        "State": EventStreamStateType,
+    },
+)
+_OptionalEventStreamSummaryTypeDef = TypedDict(
+    "_OptionalEventStreamSummaryTypeDef",
+    {
+        "StoppedSince": datetime,
+        "DestinationSummary": DestinationSummaryTypeDef,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class EventStreamSummaryTypeDef(
+    _RequiredEventStreamSummaryTypeDef, _OptionalEventStreamSummaryTypeDef
+):
+    pass
+
+GetEventStreamResponseTypeDef = TypedDict(
+    "GetEventStreamResponseTypeDef",
+    {
+        "DomainName": str,
+        "EventStreamArn": str,
+        "CreatedAt": datetime,
+        "State": EventStreamStateType,
+        "StoppedSince": datetime,
+        "DestinationDetails": EventStreamDestinationDetailsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
     },
     total=False,
 )
@@ -1311,26 +1668,28 @@
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
+        "PartyTypeString": str,
+        "GenderString": str,
     },
     total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
@@ -1341,29 +1700,29 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1403,69 +1762,87 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
+    "ListCalculatedAttributeDefinitionsResponseTypeDef",
+    {
+        "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
+    "ListCalculatedAttributesForProfileResponseTypeDef",
+    {
+        "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1490,15 +1867,15 @@
     pass
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
@@ -1545,14 +1922,16 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": UpdateAddressTypeDef,
         "ShippingAddress": UpdateAddressTypeDef,
         "MailingAddress": UpdateAddressTypeDef,
         "BillingAddress": UpdateAddressTypeDef,
         "Attributes": Mapping[str, str],
+        "PartyTypeString": str,
+        "GenderString": str,
     },
     total=False,
 )
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
@@ -1565,26 +1944,132 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Statistic": StatisticType,
+    },
+)
+_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "Conditions": ConditionsTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalCreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "CreateCalculatedAttributeDefinitionResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Conditions": ConditionsTypeDef,
+        "Statistic": StatisticType,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeDefinitionResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
+        "Conditions": ConditionsTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "CalculatedAttributeName": str,
+    },
+)
+_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "Conditions": ConditionsTypeDef,
+    },
+    total=False,
+)
+
+class UpdateCalculatedAttributeDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+):
+    pass
+
+UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
+    "UpdateCalculatedAttributeDefinitionResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Statistic": StatisticType,
+        "Conditions": ConditionsTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEventStreamsResponseTypeDef = TypedDict(
+    "ListEventStreamsResponseTypeDef",
+    {
+        "Items": List[EventStreamSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
@@ -1624,15 +2109,15 @@
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
         "AutoMerging": AutoMergingTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -1648,15 +2133,15 @@
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -1745,15 +2230,15 @@
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainResponseTypeDef = TypedDict(
     "GetDomainResponseTypeDef",
     {
         "DomainName": str,
@@ -1761,39 +2246,39 @@
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Stats": DomainStatsTypeDef,
         "Matching": MatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.26.9
-Summary: Type annotations for boto3.CustomerProfiles 1.26.9 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CustomerProfiles 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
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
 
 <a id="mypy-boto3-customer-profiles"></a>
 
 # mypy-boto3-customer-profiles
 
 [![PyPI - mypy-boto3-customer-profiles](https://img.shields.io/pypi/v/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -267,46 +269,73 @@
 from mypy_boto3_customer_profiles import CustomerProfilesClient
 
 client: CustomerProfilesClient = Session().client("customer-profiles")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_customer_profiles.paginator` module contains type annotations for
+all paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_customer_profiles import CustomerProfilesClient
+from mypy_boto3_customer_profiles.paginator import ListEventStreamsPaginator
+
+client: CustomerProfilesClient = Session().client("customer-profiles")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_event_streams_paginator: ListEventStreamsPaginator = client.get_paginator("list_event_streams")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_customer_profiles.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_customer_profiles.literals import (
     ConflictResolvingModelType,
     DataPullModeType,
+    EventStreamDestinationStatusType,
+    EventStreamStateType,
     FieldContentTypeType,
     GenderType,
     IdentityResolutionJobStatusType,
     JobScheduleDayOfTheWeekType,
+    ListEventStreamsPaginatorName,
     MarketoConnectorOperatorType,
     OperatorPropertiesKeysType,
+    OperatorType,
     PartyTypeType,
     S3ConnectorOperatorType,
     SalesforceConnectorOperatorType,
     ServiceNowConnectorOperatorType,
     SourceConnectorTypeType,
     StandardIdentifierType,
+    StatisticType,
     StatusType,
     TaskTypeType,
     TriggerTypeType,
+    UnitType,
     WorkflowTypeType,
     ZendeskConnectorOperatorType,
     logicalOperatorType,
     CustomerProfilesServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: ConflictResolvingModelType) -> bool:
     ...
 ```
@@ -317,121 +346,153 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfileKeyResponseTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
+    AttributeItemTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationTypeDef,
+    RangeTypeDef,
+    ThresholdTypeDef,
     ConnectorOperatorTypeDef,
+    CreateEventStreamRequestRequestTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
+    DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
+    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
+    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
+    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
+    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
+    DestinationSummaryTypeDef,
     DomainStatsTypeDef,
+    EventStreamDestinationDetailsTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
+    GetCalculatedAttributeDefinitionRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
+    GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
+    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
+    ListCalculatedAttributeDefinitionItemTypeDef,
+    ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
+    ListCalculatedAttributeForProfileItemTypeDef,
+    ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
+    MergeProfilesResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
+    PutProfileObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
-    AddProfileKeyResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DeleteIntegrationResponseTypeDef,
-    DeleteProfileKeyResponseTypeDef,
-    DeleteProfileObjectResponseTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
-    DeleteProfileResponseTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
-    GetIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MergeProfilesResponseTypeDef,
-    PutIntegrationResponseTypeDef,
-    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
+    AttributeDetailsTypeDef,
     AutoMergingTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    ConditionsTypeDef,
     TaskTypeDef,
+    EventStreamSummaryTypeDef,
+    GetEventStreamResponseTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
     ProfileTypeDef,
     GetMatchesResponseTypeDef,
     GetProfileObjectTypeResponseTypeDef,
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
+    ListCalculatedAttributeDefinitionsResponseTypeDef,
+    ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TriggerPropertiesTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    CreateCalculatedAttributeDefinitionResponseTypeDef,
+    GetCalculatedAttributeDefinitionResponseTypeDef,
+    UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
+    UpdateCalculatedAttributeDefinitionResponseTypeDef,
+    ListEventStreamsResponseTypeDef,
     MatchingRequestTypeDef,
     MatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
     TriggerConfigTypeDef,
     SourceFlowConfigTypeDef,
@@ -456,42 +517,42 @@
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

### Comparing `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.27.0/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_customer_profiles/__init__.py
 mypy_boto3_customer_profiles/__init__.pyi
 mypy_boto3_customer_profiles/__main__.py
 mypy_boto3_customer_profiles/client.py
 mypy_boto3_customer_profiles/client.pyi
 mypy_boto3_customer_profiles/literals.py
 mypy_boto3_customer_profiles/literals.pyi
+mypy_boto3_customer_profiles/paginator.py
+mypy_boto3_customer_profiles/paginator.pyi
 mypy_boto3_customer_profiles/py.typed
 mypy_boto3_customer_profiles/type_defs.py
 mypy_boto3_customer_profiles/type_defs.pyi
 mypy_boto3_customer_profiles/version.py
 mypy_boto3_customer_profiles.egg-info/PKG-INFO
 mypy_boto3_customer_profiles.egg-info/SOURCES.txt
 mypy_boto3_customer_profiles.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-customer-profiles-1.26.9/setup.py` & `mypy-boto3-customer-profiles-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-customer-profiles.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.26.9",
+    version="1.27.0",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CustomerProfiles 1.26.9 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CustomerProfiles 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_customer_profiles": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_customer_profiles": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/",
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


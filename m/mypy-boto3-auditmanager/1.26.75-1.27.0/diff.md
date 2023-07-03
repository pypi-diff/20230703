# Comparing `tmp/mypy-boto3-auditmanager-1.26.75.tar.gz` & `tmp/mypy-boto3-auditmanager-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-auditmanager-1.26.75.tar", last modified: Mon Feb 20 20:25:59 2023, max compression
+gzip compressed data, was "mypy-boto3-auditmanager-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-auditmanager-1.26.75.tar` & `mypy-boto3-auditmanager-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42576 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42509 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56795 2023-02-20 20:25:43.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56750 2023-02-20 20:25:42.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 20:25:59.000000 mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 20:25:59.228019 mypy-boto3-auditmanager-1.26.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-20 20:25:41.000000 mypy-boto3-auditmanager-1.26.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.838863 mypy-boto3-auditmanager-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-03 19:50:24.838863 mypy-boto3-auditmanager-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.838863 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-03 19:32:53.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-03 19:32:53.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57825 2023-07-03 19:32:54.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57780 2023-07-03 19:32:54.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.838863 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-03 19:50:24.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:50:24.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:24.000000 mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.838863 mypy-boto3-auditmanager-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:32:52.000000 mypy-boto3-auditmanager-1.27.0/setup.py
```

### Comparing `mypy-boto3-auditmanager-1.26.75/LICENSE` & `mypy-boto3-auditmanager-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-auditmanager-1.26.75/PKG-INFO` & `mypy-boto3-auditmanager-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.26.75
-Summary: Type annotations for boto3.AuditManager 1.26.75 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.AuditManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-auditmanager"></a>
 
 # mypy-boto3-auditmanager
 
 [![PyPI - mypy-boto3-auditmanager](https://img.shields.io/pypi/v/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.26.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +289,15 @@
     ControlSetStatusType,
     ControlStatusType,
     ControlTypeType,
     DelegationStatusType,
     DeleteResourcesType,
     EvidenceFinderBackfillStatusType,
     EvidenceFinderEnablementStatusType,
+    ExportDestinationTypeType,
     FrameworkTypeType,
     KeywordInputTypeType,
     ObjectTypeEnumType,
     RoleTypeType,
     SettingAttributeType,
     ShareRequestActionType,
     ShareRequestStatusType,
@@ -335,99 +336,102 @@
     FrameworkMetadataTypeDef,
     AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
+    DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
+    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
+    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
+    GetEvidenceFileUploadUrlRequestRequestTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
+    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
-    DeregisterAccountResponseTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
-    ListAssessmentFrameworkShareRequestsResponseTypeDef,
     ListAssessmentFrameworksResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterAccountResponseTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
+    ListAssessmentFrameworkShareRequestsResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
@@ -493,42 +497,42 @@
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

### Comparing `mypy-boto3-auditmanager-1.26.75/README.md` & `mypy-boto3-auditmanager-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-auditmanager"></a>
 
 # mypy-boto3-auditmanager
 
 [![PyPI - mypy-boto3-auditmanager](https://img.shields.io/pypi/v/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.26.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,14 +257,15 @@
     ControlSetStatusType,
     ControlStatusType,
     ControlTypeType,
     DelegationStatusType,
     DeleteResourcesType,
     EvidenceFinderBackfillStatusType,
     EvidenceFinderEnablementStatusType,
+    ExportDestinationTypeType,
     FrameworkTypeType,
     KeywordInputTypeType,
     ObjectTypeEnumType,
     RoleTypeType,
     SettingAttributeType,
     ShareRequestActionType,
     ShareRequestStatusType,
@@ -303,99 +304,102 @@
     FrameworkMetadataTypeDef,
     AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
+    DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
+    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
+    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
+    GetEvidenceFileUploadUrlRequestRequestTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
+    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
-    DeregisterAccountResponseTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
-    ListAssessmentFrameworkShareRequestsResponseTypeDef,
     ListAssessmentFrameworksResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterAccountResponseTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
+    ListAssessmentFrameworkShareRequestsResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
@@ -461,42 +465,42 @@
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

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/__main__.py` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AuditManager 1.26.75\nVersion:         1.26.75\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.AuditManager 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.75")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.py` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,24 +39,26 @@
     CreateAssessmentFrameworkControlSetTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     CreateAssessmentReportResponseTypeDef,
     CreateAssessmentResponseTypeDef,
     CreateControlMappingSourceTypeDef,
     CreateControlResponseTypeDef,
     CreateDelegationRequestTypeDef,
+    DefaultExportDestinationTypeDef,
     DeregisterAccountResponseTypeDef,
     DeregistrationPolicyTypeDef,
     GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     GetAssessmentReportUrlResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetChangeLogsResponseTypeDef,
     GetControlResponseTypeDef,
     GetDelegationsResponseTypeDef,
     GetEvidenceByEvidenceFolderResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
     GetEvidenceResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetOrganizationAdminAccountResponseTypeDef,
@@ -190,16 +192,15 @@
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         manualEvidence: Sequence[ManualEvidenceTypeDef]
     ) -> BatchImportEvidenceToAssessmentControlResponseTypeDef:
         """
-        Uploads one or more pieces of evidence to a control in an Audit Manager
-        assessment.
+        Adds one or more pieces of evidence to a control in an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.batch_import_evidence_to_assessment_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#batch_import_evidence_to_assessment_control)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -363,43 +364,43 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#generate_presigned_url)
         """
 
     def get_account_status(self) -> GetAccountStatusResponseTypeDef:
         """
-        Returns the registration status of an account in Audit Manager.
+        Gets the registration status of an account in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_account_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_account_status)
         """
 
     def get_assessment(self, *, assessmentId: str) -> GetAssessmentResponseTypeDef:
         """
-        Returns an assessment from Audit Manager.
+        Gets information about a specified assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_assessment)
         """
 
     def get_assessment_framework(
         self, *, frameworkId: str
     ) -> GetAssessmentFrameworkResponseTypeDef:
         """
-        Returns a framework from Audit Manager.
+        Gets information about a specified framework.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_assessment_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_assessment_framework)
         """
 
     def get_assessment_report_url(
         self, *, assessmentReportId: str, assessmentId: str
     ) -> GetAssessmentReportUrlResponseTypeDef:
         """
-        Returns the URL of an assessment report in Audit Manager.
+        Gets the URL of an assessment report in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_assessment_report_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_assessment_report_url)
         """
 
     def get_change_logs(
         self,
@@ -407,43 +408,43 @@
         assessmentId: str,
         controlSetId: str = ...,
         controlId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetChangeLogsResponseTypeDef:
         """
-        Returns a list of changelogs from Audit Manager.
+        Gets a list of changelogs from Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_change_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_change_logs)
         """
 
     def get_control(self, *, controlId: str) -> GetControlResponseTypeDef:
         """
-        Returns a control from Audit Manager.
+        Gets information about a specified control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_control)
         """
 
     def get_delegations(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> GetDelegationsResponseTypeDef:
         """
-        Returns a list of delegations from an audit owner to a delegate.
+        Gets a list of delegations from an audit owner to a delegate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_delegations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_delegations)
         """
 
     def get_evidence(
         self, *, assessmentId: str, controlSetId: str, evidenceFolderId: str, evidenceId: str
     ) -> GetEvidenceResponseTypeDef:
         """
-        Returns evidence from Audit Manager.
+        Gets information about a specified evidence item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence)
         """
 
     def get_evidence_by_evidence_folder(
         self,
@@ -451,35 +452,46 @@
         assessmentId: str,
         controlSetId: str,
         evidenceFolderId: str,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetEvidenceByEvidenceFolderResponseTypeDef:
         """
-        Returns all evidence from a specified evidence folder in Audit Manager.
+        Gets all evidence from a specified evidence folder in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_by_evidence_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_by_evidence_folder)
         """
 
+    def get_evidence_file_upload_url(
+        self, *, fileName: str
+    ) -> GetEvidenceFileUploadUrlResponseTypeDef:
+        """
+        Creates a presigned Amazon S3 URL that can be used to upload a file as manual
+        evidence.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_file_upload_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_file_upload_url)
+        """
+
     def get_evidence_folder(
         self, *, assessmentId: str, controlSetId: str, evidenceFolderId: str
     ) -> GetEvidenceFolderResponseTypeDef:
         """
-        Returns an evidence folder from the specified assessment in Audit Manager.
+        Gets an evidence folder from a specified assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_folder)
         """
 
     def get_evidence_folders_by_assessment(
         self, *, assessmentId: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetEvidenceFoldersByAssessmentResponseTypeDef:
         """
-        Returns the evidence folders from a specified assessment in Audit Manager.
+        Gets the evidence folders from a specified assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folders_by_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_folders_by_assessment)
         """
 
     def get_evidence_folders_by_assessment_control(
         self,
@@ -487,16 +499,16 @@
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetEvidenceFoldersByAssessmentControlResponseTypeDef:
         """
-        Returns a list of evidence folders that are associated with a specified control
-        in an Audit Manager assessment.
+        Gets a list of evidence folders that are associated with a specified control in
+        an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folders_by_assessment_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_folders_by_assessment_control)
         """
 
     def get_insights(self) -> GetInsightsResponseTypeDef:
         """
@@ -514,33 +526,33 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_insights_by_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_insights_by_assessment)
         """
 
     def get_organization_admin_account(self) -> GetOrganizationAdminAccountResponseTypeDef:
         """
-        Returns the name of the delegated Amazon Web Services administrator account for
-        the organization.
+        Gets the name of the delegated Amazon Web Services administrator account for a
+        specified organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_organization_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_organization_admin_account)
         """
 
     def get_services_in_scope(self) -> GetServicesInScopeResponseTypeDef:
         """
-        Returns a list of all of the Amazon Web Services that you can choose to include
-        in your assessment.
+        Gets a list of all of the Amazon Web Services that you can choose to include in
+        your assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_services_in_scope)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_services_in_scope)
         """
 
     def get_settings(self, *, attribute: SettingAttributeType) -> GetSettingsResponseTypeDef:
         """
-        Returns the settings for the specified Amazon Web Services account.
+        Gets the settings for a specified Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_settings)
         """
 
     def list_assessment_control_insights_by_control_domain(
         self,
@@ -824,15 +836,16 @@
         self,
         *,
         snsTopic: str = ...,
         defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         defaultProcessOwners: Sequence[RoleTypeDef] = ...,
         kmsKey: str = ...,
         evidenceFinderEnabled: bool = ...,
-        deregistrationPolicy: DeregistrationPolicyTypeDef = ...
+        deregistrationPolicy: DeregistrationPolicyTypeDef = ...,
+        defaultExportDestination: DefaultExportDestinationTypeDef = ...
     ) -> UpdateSettingsResponseTypeDef:
         """
         Updates Audit Manager settings for the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#update_settings)
         """
```

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/client.pyi` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,24 +39,26 @@
     CreateAssessmentFrameworkControlSetTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     CreateAssessmentReportResponseTypeDef,
     CreateAssessmentResponseTypeDef,
     CreateControlMappingSourceTypeDef,
     CreateControlResponseTypeDef,
     CreateDelegationRequestTypeDef,
+    DefaultExportDestinationTypeDef,
     DeregisterAccountResponseTypeDef,
     DeregistrationPolicyTypeDef,
     GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     GetAssessmentReportUrlResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetChangeLogsResponseTypeDef,
     GetControlResponseTypeDef,
     GetDelegationsResponseTypeDef,
     GetEvidenceByEvidenceFolderResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
     GetEvidenceResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetOrganizationAdminAccountResponseTypeDef,
@@ -181,16 +183,15 @@
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         manualEvidence: Sequence[ManualEvidenceTypeDef]
     ) -> BatchImportEvidenceToAssessmentControlResponseTypeDef:
         """
-        Uploads one or more pieces of evidence to a control in an Audit Manager
-        assessment.
+        Adds one or more pieces of evidence to a control in an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.batch_import_evidence_to_assessment_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#batch_import_evidence_to_assessment_control)
         """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
@@ -338,129 +339,139 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#generate_presigned_url)
         """
     def get_account_status(self) -> GetAccountStatusResponseTypeDef:
         """
-        Returns the registration status of an account in Audit Manager.
+        Gets the registration status of an account in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_account_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_account_status)
         """
     def get_assessment(self, *, assessmentId: str) -> GetAssessmentResponseTypeDef:
         """
-        Returns an assessment from Audit Manager.
+        Gets information about a specified assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_assessment)
         """
     def get_assessment_framework(
         self, *, frameworkId: str
     ) -> GetAssessmentFrameworkResponseTypeDef:
         """
-        Returns a framework from Audit Manager.
+        Gets information about a specified framework.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_assessment_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_assessment_framework)
         """
     def get_assessment_report_url(
         self, *, assessmentReportId: str, assessmentId: str
     ) -> GetAssessmentReportUrlResponseTypeDef:
         """
-        Returns the URL of an assessment report in Audit Manager.
+        Gets the URL of an assessment report in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_assessment_report_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_assessment_report_url)
         """
     def get_change_logs(
         self,
         *,
         assessmentId: str,
         controlSetId: str = ...,
         controlId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetChangeLogsResponseTypeDef:
         """
-        Returns a list of changelogs from Audit Manager.
+        Gets a list of changelogs from Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_change_logs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_change_logs)
         """
     def get_control(self, *, controlId: str) -> GetControlResponseTypeDef:
         """
-        Returns a control from Audit Manager.
+        Gets information about a specified control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_control)
         """
     def get_delegations(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> GetDelegationsResponseTypeDef:
         """
-        Returns a list of delegations from an audit owner to a delegate.
+        Gets a list of delegations from an audit owner to a delegate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_delegations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_delegations)
         """
     def get_evidence(
         self, *, assessmentId: str, controlSetId: str, evidenceFolderId: str, evidenceId: str
     ) -> GetEvidenceResponseTypeDef:
         """
-        Returns evidence from Audit Manager.
+        Gets information about a specified evidence item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence)
         """
     def get_evidence_by_evidence_folder(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         evidenceFolderId: str,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetEvidenceByEvidenceFolderResponseTypeDef:
         """
-        Returns all evidence from a specified evidence folder in Audit Manager.
+        Gets all evidence from a specified evidence folder in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_by_evidence_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_by_evidence_folder)
         """
+    def get_evidence_file_upload_url(
+        self, *, fileName: str
+    ) -> GetEvidenceFileUploadUrlResponseTypeDef:
+        """
+        Creates a presigned Amazon S3 URL that can be used to upload a file as manual
+        evidence.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_file_upload_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_file_upload_url)
+        """
     def get_evidence_folder(
         self, *, assessmentId: str, controlSetId: str, evidenceFolderId: str
     ) -> GetEvidenceFolderResponseTypeDef:
         """
-        Returns an evidence folder from the specified assessment in Audit Manager.
+        Gets an evidence folder from a specified assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folder)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_folder)
         """
     def get_evidence_folders_by_assessment(
         self, *, assessmentId: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetEvidenceFoldersByAssessmentResponseTypeDef:
         """
-        Returns the evidence folders from a specified assessment in Audit Manager.
+        Gets the evidence folders from a specified assessment in Audit Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folders_by_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_folders_by_assessment)
         """
     def get_evidence_folders_by_assessment_control(
         self,
         *,
         assessmentId: str,
         controlSetId: str,
         controlId: str,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetEvidenceFoldersByAssessmentControlResponseTypeDef:
         """
-        Returns a list of evidence folders that are associated with a specified control
-        in an Audit Manager assessment.
+        Gets a list of evidence folders that are associated with a specified control in
+        an Audit Manager assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_evidence_folders_by_assessment_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_evidence_folders_by_assessment_control)
         """
     def get_insights(self) -> GetInsightsResponseTypeDef:
         """
         Gets the latest analytics data for all your current active assessments.
@@ -475,31 +486,31 @@
         Gets the latest analytics data for a specific active assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_insights_by_assessment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_insights_by_assessment)
         """
     def get_organization_admin_account(self) -> GetOrganizationAdminAccountResponseTypeDef:
         """
-        Returns the name of the delegated Amazon Web Services administrator account for
-        the organization.
+        Gets the name of the delegated Amazon Web Services administrator account for a
+        specified organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_organization_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_organization_admin_account)
         """
     def get_services_in_scope(self) -> GetServicesInScopeResponseTypeDef:
         """
-        Returns a list of all of the Amazon Web Services that you can choose to include
-        in your assessment.
+        Gets a list of all of the Amazon Web Services that you can choose to include in
+        your assessment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_services_in_scope)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_services_in_scope)
         """
     def get_settings(self, *, attribute: SettingAttributeType) -> GetSettingsResponseTypeDef:
         """
-        Returns the settings for the specified Amazon Web Services account.
+        Gets the settings for a specified Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.get_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#get_settings)
         """
     def list_assessment_control_insights_by_control_domain(
         self,
         *,
@@ -758,15 +769,16 @@
         self,
         *,
         snsTopic: str = ...,
         defaultAssessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         defaultProcessOwners: Sequence[RoleTypeDef] = ...,
         kmsKey: str = ...,
         evidenceFinderEnabled: bool = ...,
-        deregistrationPolicy: DeregistrationPolicyTypeDef = ...
+        deregistrationPolicy: DeregistrationPolicyTypeDef = ...,
+        defaultExportDestination: DefaultExportDestinationTypeDef = ...
     ) -> UpdateSettingsResponseTypeDef:
         """
         Updates Audit Manager settings for the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.update_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/client/#update_settings)
         """
```

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.py` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "ControlSetStatusType",
     "ControlStatusType",
     "ControlTypeType",
     "DelegationStatusType",
     "DeleteResourcesType",
     "EvidenceFinderBackfillStatusType",
     "EvidenceFinderEnablementStatusType",
+    "ExportDestinationTypeType",
     "FrameworkTypeType",
     "KeywordInputTypeType",
     "ObjectTypeEnumType",
     "RoleTypeType",
     "SettingAttributeType",
     "ShareRequestActionType",
     "ShareRequestStatusType",
@@ -71,23 +72,25 @@
 ControlTypeType = Literal["Custom", "Standard"]
 DelegationStatusType = Literal["COMPLETE", "IN_PROGRESS", "UNDER_REVIEW"]
 DeleteResourcesType = Literal["ALL", "DEFAULT"]
 EvidenceFinderBackfillStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
 EvidenceFinderEnablementStatusType = Literal[
     "DISABLED", "DISABLE_IN_PROGRESS", "ENABLED", "ENABLE_IN_PROGRESS"
 ]
+ExportDestinationTypeType = Literal["S3"]
 FrameworkTypeType = Literal["Custom", "Standard"]
-KeywordInputTypeType = Literal["SELECT_FROM_LIST"]
+KeywordInputTypeType = Literal["INPUT_TEXT", "SELECT_FROM_LIST", "UPLOAD_FILE"]
 ObjectTypeEnumType = Literal[
     "ASSESSMENT", "ASSESSMENT_REPORT", "CONTROL", "CONTROL_SET", "DELEGATION"
 ]
 RoleTypeType = Literal["PROCESS_OWNER", "RESOURCE_OWNER"]
 SettingAttributeType = Literal[
     "ALL",
     "DEFAULT_ASSESSMENT_REPORTS_DESTINATION",
+    "DEFAULT_EXPORT_DESTINATION",
     "DEFAULT_PROCESS_OWNERS",
     "DEREGISTRATION_POLICY",
     "EVIDENCE_FINDER_ENABLEMENT",
     "IS_AWS_ORG_ENABLED",
     "SNS_TOPIC",
 ]
 ShareRequestActionType = Literal["ACCEPT", "DECLINE", "REVOKE"]
@@ -112,14 +115,15 @@
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
@@ -159,14 +163,15 @@
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
@@ -245,14 +250,15 @@
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
@@ -263,14 +269,15 @@
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
@@ -306,14 +313,15 @@
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
@@ -332,16 +340,19 @@
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
@@ -421,18 +432,21 @@
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

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/literals.pyi` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "ControlSetStatusType",
     "ControlStatusType",
     "ControlTypeType",
     "DelegationStatusType",
     "DeleteResourcesType",
     "EvidenceFinderBackfillStatusType",
     "EvidenceFinderEnablementStatusType",
+    "ExportDestinationTypeType",
     "FrameworkTypeType",
     "KeywordInputTypeType",
     "ObjectTypeEnumType",
     "RoleTypeType",
     "SettingAttributeType",
     "ShareRequestActionType",
     "ShareRequestStatusType",
@@ -69,23 +70,25 @@
 ControlTypeType = Literal["Custom", "Standard"]
 DelegationStatusType = Literal["COMPLETE", "IN_PROGRESS", "UNDER_REVIEW"]
 DeleteResourcesType = Literal["ALL", "DEFAULT"]
 EvidenceFinderBackfillStatusType = Literal["COMPLETED", "IN_PROGRESS", "NOT_STARTED"]
 EvidenceFinderEnablementStatusType = Literal[
     "DISABLED", "DISABLE_IN_PROGRESS", "ENABLED", "ENABLE_IN_PROGRESS"
 ]
+ExportDestinationTypeType = Literal["S3"]
 FrameworkTypeType = Literal["Custom", "Standard"]
-KeywordInputTypeType = Literal["SELECT_FROM_LIST"]
+KeywordInputTypeType = Literal["INPUT_TEXT", "SELECT_FROM_LIST", "UPLOAD_FILE"]
 ObjectTypeEnumType = Literal[
     "ASSESSMENT", "ASSESSMENT_REPORT", "CONTROL", "CONTROL_SET", "DELEGATION"
 ]
 RoleTypeType = Literal["PROCESS_OWNER", "RESOURCE_OWNER"]
 SettingAttributeType = Literal[
     "ALL",
     "DEFAULT_ASSESSMENT_REPORTS_DESTINATION",
+    "DEFAULT_EXPORT_DESTINATION",
     "DEFAULT_PROCESS_OWNERS",
     "DEREGISTRATION_POLICY",
     "EVIDENCE_FINDER_ENABLEMENT",
     "IS_AWS_ORG_ENABLED",
     "SNS_TOPIC",
 ]
 ShareRequestActionType = Literal["ACCEPT", "DECLINE", "REVOKE"]
@@ -110,14 +113,15 @@
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
@@ -157,14 +161,15 @@
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
@@ -243,14 +248,15 @@
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
@@ -261,14 +267,15 @@
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
@@ -304,14 +311,15 @@
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
@@ -330,16 +338,19 @@
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
@@ -419,18 +430,21 @@
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

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.py` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ControlStatusType,
     ControlTypeType,
     DelegationStatusType,
     DeleteResourcesType,
     EvidenceFinderBackfillStatusType,
     EvidenceFinderEnablementStatusType,
     FrameworkTypeType,
+    KeywordInputTypeType,
     ObjectTypeEnumType,
     RoleTypeType,
     SettingAttributeType,
     ShareRequestActionType,
     ShareRequestStatusType,
     ShareRequestTypeType,
     SourceFrequencyType,
@@ -62,99 +63,102 @@
     "FrameworkMetadataTypeDef",
     "AssessmentReportsDestinationTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
     "SourceKeywordTypeDef",
     "ControlMetadataTypeDef",
     "CreateAssessmentFrameworkControlTypeDef",
     "CreateAssessmentReportRequestRequestTypeDef",
+    "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
+    "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
+    "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
     "URLTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetChangeLogsRequestRequestTypeDef",
     "GetControlRequestRequestTypeDef",
     "GetDelegationsRequestRequestTypeDef",
     "GetEvidenceByEvidenceFolderRequestRequestTypeDef",
+    "GetEvidenceFileUploadUrlRequestRequestTypeDef",
+    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     "GetEvidenceRequestRequestTypeDef",
     "GetInsightsByAssessmentRequestRequestTypeDef",
     "InsightsByAssessmentTypeDef",
     "InsightsTypeDef",
+    "GetOrganizationAdminAccountResponseTypeDef",
     "ServiceMetadataTypeDef",
     "GetSettingsRequestRequestTypeDef",
     "ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef",
     "ListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     "ListAssessmentFrameworksRequestRequestTypeDef",
     "ListAssessmentReportsRequestRequestTypeDef",
     "ListAssessmentsRequestRequestTypeDef",
     "ListControlDomainInsightsByAssessmentRequestRequestTypeDef",
     "ListControlDomainInsightsRequestRequestTypeDef",
     "ListControlInsightsByControlDomainRequestRequestTypeDef",
     "ListControlsRequestRequestTypeDef",
     "ListKeywordsForDataSourceRequestRequestTypeDef",
+    "ListKeywordsForDataSourceResponseTypeDef",
     "ListNotificationsRequestRequestTypeDef",
     "NotificationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RegisterAccountRequestRequestTypeDef",
+    "RegisterAccountResponseTypeDef",
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
+    "RegisterOrganizationAdminAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartAssessmentFrameworkShareRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    "CreateAssessmentReportResponseTypeDef",
-    "DeregisterAccountResponseTypeDef",
-    "GetAccountStatusResponseTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
-    "GetOrganizationAdminAccountResponseTypeDef",
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
     "ListAssessmentFrameworksResponseTypeDef",
-    "ListAssessmentReportsResponseTypeDef",
-    "ListKeywordsForDataSourceResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterAccountResponseTypeDef",
-    "RegisterOrganizationAdminAccountResponseTypeDef",
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
     "StartAssessmentFrameworkShareResponseTypeDef",
     "UpdateAssessmentFrameworkShareResponseTypeDef",
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    "ListAssessmentReportsResponseTypeDef",
+    "CreateAssessmentReportResponseTypeDef",
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     "BatchCreateDelegationByAssessmentRequestRequestTypeDef",
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
@@ -405,25 +409,14 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
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
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
         "roleArn": str,
         "roleType": RoleTypeType,
@@ -458,14 +451,16 @@
     },
 )
 
 ManualEvidenceTypeDef = TypedDict(
     "ManualEvidenceTypeDef",
     {
         "s3ResourcePath": str,
+        "textResponse": str,
+        "evidenceFileName": str,
     },
     total=False,
 )
 
 ChangeLogTypeDef = TypedDict(
     "ChangeLogTypeDef",
     {
@@ -487,15 +482,15 @@
     },
     total=False,
 )
 
 SourceKeywordTypeDef = TypedDict(
     "SourceKeywordTypeDef",
     {
-        "keywordInputType": Literal["SELECT_FROM_LIST"],
+        "keywordInputType": KeywordInputTypeType,
         "keywordValue": str,
     },
     total=False,
 )
 
 ControlMetadataTypeDef = TypedDict(
     "ControlMetadataTypeDef",
@@ -537,14 +532,23 @@
 class CreateAssessmentReportRequestRequestTypeDef(
     _RequiredCreateAssessmentReportRequestRequestTypeDef,
     _OptionalCreateAssessmentReportRequestRequestTypeDef,
 ):
     pass
 
 
+DefaultExportDestinationTypeDef = TypedDict(
+    "DefaultExportDestinationTypeDef",
+    {
+        "destinationType": Literal["S3"],
+        "destination": str,
+    },
+    total=False,
+)
+
 DelegationMetadataTypeDef = TypedDict(
     "DelegationMetadataTypeDef",
     {
         "id": str,
         "assessmentName": str,
         "assessmentId": str,
         "status": DelegationStatusType,
@@ -588,14 +592,22 @@
 DeleteControlRequestRequestTypeDef = TypedDict(
     "DeleteControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
+DeregisterAccountResponseTypeDef = TypedDict(
+    "DeregisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeregisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
@@ -633,14 +645,22 @@
         "arn": str,
         "value": str,
         "complianceCheck": str,
     },
     total=False,
 )
 
+GetAccountStatusResponseTypeDef = TypedDict(
+    "GetAccountStatusResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "GetAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
     },
 )
 
@@ -729,14 +749,30 @@
 class GetEvidenceByEvidenceFolderRequestRequestTypeDef(
     _RequiredGetEvidenceByEvidenceFolderRequestRequestTypeDef,
     _OptionalGetEvidenceByEvidenceFolderRequestRequestTypeDef,
 ):
     pass
 
 
+GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlRequestRequestTypeDef",
+    {
+        "fileName": str,
+    },
+)
+
+GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlResponseTypeDef",
+    {
+        "evidenceFileName": str,
+        "uploadUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEvidenceFolderRequestRequestTypeDef = TypedDict(
     "GetEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
     },
@@ -830,14 +866,23 @@
         "assessmentControlsCountByNoncompliantEvidence": int,
         "totalAssessmentControlsCount": int,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
+GetOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "GetOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
         "category": str,
@@ -1037,14 +1082,23 @@
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
 
+ListKeywordsForDataSourceResponseTypeDef = TypedDict(
+    "ListKeywordsForDataSourceResponseTypeDef",
+    {
+        "keywords": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListNotificationsRequestRequestTypeDef = TypedDict(
     "ListNotificationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1068,30 +1122,66 @@
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
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "kmsKey": str,
         "delegatedAdminAccount": str,
     },
     total=False,
 )
 
+RegisterAccountResponseTypeDef = TypedDict(
+    "RegisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
 )
 
+RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "RegisterOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
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
 _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "frameworkId": str,
         "destinationAccount": str,
         "destinationRegion": str,
     },
@@ -1183,14 +1273,26 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
+ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    {
+        "signatureValid": bool,
+        "signatureAlgorithm": str,
+        "signatureDateTime": str,
+        "signatureKeyId": str,
+        "validationErrors": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
     },
     total=False,
@@ -1223,177 +1325,106 @@
         "evidenceSources": List[str],
         "evidenceCount": int,
         "assessmentReportEvidenceCount": int,
     },
     total=False,
 )
 
-BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAssessmentReportResponseTypeDef = TypedDict(
-    "CreateAssessmentReportResponseTypeDef",
-    {
-        "assessmentReport": AssessmentReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterAccountResponseTypeDef = TypedDict(
-    "DeregisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountStatusResponseTypeDef = TypedDict(
-    "GetAccountStatusResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceFolderResponseTypeDef",
     {
         "evidenceFolder": AssessmentEvidenceFolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceFoldersByAssessmentControlResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceFoldersByAssessmentResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "GetOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
-    {
-        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentFrameworksResponseTypeDef = TypedDict(
     "ListAssessmentFrameworksResponseTypeDef",
     {
         "frameworkMetadataList": List[AssessmentFrameworkMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAssessmentReportsResponseTypeDef = TypedDict(
-    "ListAssessmentReportsResponseTypeDef",
-    {
-        "assessmentReports": List[AssessmentReportMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListKeywordsForDataSourceResponseTypeDef = TypedDict(
-    "ListKeywordsForDataSourceResponseTypeDef",
+ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
     {
-        "keywords": List[str],
+        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "StartAssessmentFrameworkShareResponseTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RegisterAccountResponseTypeDef = TypedDict(
-    "RegisterAccountResponseTypeDef",
+UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "UpdateAssessmentFrameworkShareResponseTypeDef",
     {
-        "status": AccountStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "RegisterOrganizationAdminAccountResponseTypeDef",
+BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
     {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "StartAssessmentFrameworkShareResponseTypeDef",
+BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "UpdateAssessmentFrameworkShareResponseTypeDef",
+ListAssessmentReportsResponseTypeDef = TypedDict(
+    "ListAssessmentReportsResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentReports": List[AssessmentReportMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+CreateAssessmentReportResponseTypeDef = TypedDict(
+    "CreateAssessmentReportResponseTypeDef",
     {
-        "signatureValid": bool,
-        "signatureAlgorithm": str,
-        "signatureDateTime": str,
-        "signatureKeyId": str,
-        "validationErrors": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentReport": AssessmentReportTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
         "createDelegationRequest": CreateDelegationRequestTypeDef,
@@ -1411,15 +1442,15 @@
     },
 )
 
 BatchDeleteDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     {
         "errors": List[BatchDeleteDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
         "manualEvidence": ManualEvidenceTypeDef,
@@ -1440,15 +1471,15 @@
 )
 
 GetChangeLogsResponseTypeDef = TypedDict(
     "GetChangeLogsResponseTypeDef",
     {
         "changeLogs": List[ChangeLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ControlDomainInsightsTypeDef = TypedDict(
     "ControlDomainInsightsTypeDef",
     {
         "name": str,
@@ -1514,15 +1545,15 @@
 )
 
 ListControlsResponseTypeDef = TypedDict(
     "ListControlsResponseTypeDef",
     {
         "controlMetadataList": List[ControlMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
@@ -1568,41 +1599,43 @@
 
 
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "snsTopic": str,
         "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "defaultProcessOwners": Sequence[RoleTypeDef],
         "kmsKey": str,
         "evidenceFinderEnabled": bool,
         "deregistrationPolicy": DeregistrationPolicyTypeDef,
+        "defaultExportDestination": DefaultExportDestinationTypeDef,
     },
     total=False,
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "isAwsOrgEnabled": bool,
         "snsTopic": str,
         "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "defaultProcessOwners": List[RoleTypeDef],
         "kmsKey": str,
         "evidenceFinderEnablement": EvidenceFinderEnablementTypeDef,
         "deregistrationPolicy": DeregistrationPolicyTypeDef,
+        "defaultExportDestination": DefaultExportDestinationTypeDef,
     },
     total=False,
 )
 
 EvidenceTypeDef = TypedDict(
     "EvidenceTypeDef",
     {
@@ -1625,48 +1658,48 @@
     total=False,
 )
 
 GetAssessmentReportUrlResponseTypeDef = TypedDict(
     "GetAssessmentReportUrlResponseTypeDef",
     {
         "preSignedUrl": URLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightsByAssessmentResponseTypeDef = TypedDict(
     "GetInsightsByAssessmentResponseTypeDef",
     {
         "insights": InsightsByAssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "insights": InsightsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServicesInScopeResponseTypeDef = TypedDict(
     "GetServicesInScopeResponseTypeDef",
     {
         "serviceMetadata": List[ServiceMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotificationsResponseTypeDef = TypedDict(
     "ListNotificationsResponseTypeDef",
     {
         "notifications": List[NotificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentMetadataTypeDef = TypedDict(
     "AssessmentMetadataTypeDef",
     {
         "name": str,
@@ -1736,15 +1769,15 @@
 
 
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
@@ -1759,68 +1792,68 @@
     total=False,
 )
 
 UpdateAssessmentControlResponseTypeDef = TypedDict(
     "UpdateAssessmentControlResponseTypeDef",
     {
         "control": AssessmentControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     {
         "delegations": List[DelegationTypeDef],
         "errors": List[BatchCreateDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchImportEvidenceToAssessmentControlResponseTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     {
         "errors": List[BatchImportEvidenceToAssessmentControlErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlDomainInsightsByAssessmentResponseTypeDef = TypedDict(
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlDomainInsightsResponseTypeDef = TypedDict(
     "ListControlDomainInsightsResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListAssessmentControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsByAssessment": List[ControlInsightsMetadataByAssessmentItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsMetadata": List[ControlInsightsMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ControlTypeDef = TypedDict(
     "ControlTypeDef",
     {
         "arn": str,
@@ -1944,40 +1977,40 @@
     pass
 
 
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSettingsResponseTypeDef = TypedDict(
     "UpdateSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceByEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceByEvidenceFolderResponseTypeDef",
     {
         "evidence": List[EvidenceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceResponseTypeDef = TypedDict(
     "GetEvidenceResponseTypeDef",
     {
         "evidence": EvidenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentFrameworkTypeDef = TypedDict(
     "AssessmentFrameworkTypeDef",
     {
         "id": str,
@@ -1988,15 +2021,15 @@
     total=False,
 )
 
 UpdateAssessmentControlSetStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusResponseTypeDef",
     {
         "controlSet": AssessmentControlSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ControlSetTypeDef = TypedDict(
     "ControlSetTypeDef",
     {
         "id": str,
@@ -2006,31 +2039,31 @@
     total=False,
 )
 
 CreateControlResponseTypeDef = TypedDict(
     "CreateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetControlResponseTypeDef = TypedDict(
     "GetControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateControlResponseTypeDef = TypedDict(
     "UpdateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
@@ -2063,59 +2096,59 @@
     total=False,
 )
 
 CreateAssessmentResponseTypeDef = TypedDict(
     "CreateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
         "userRole": RoleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentStatusResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssessmentFrameworkResponseTypeDef = TypedDict(
     "CreateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssessmentFrameworkResponseTypeDef = TypedDict(
     "GetAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentFrameworkResponseTypeDef = TypedDict(
     "UpdateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager/type_defs.pyi` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ControlStatusType,
     ControlTypeType,
     DelegationStatusType,
     DeleteResourcesType,
     EvidenceFinderBackfillStatusType,
     EvidenceFinderEnablementStatusType,
     FrameworkTypeType,
+    KeywordInputTypeType,
     ObjectTypeEnumType,
     RoleTypeType,
     SettingAttributeType,
     ShareRequestActionType,
     ShareRequestStatusType,
     ShareRequestTypeType,
     SourceFrequencyType,
@@ -61,99 +62,102 @@
     "FrameworkMetadataTypeDef",
     "AssessmentReportsDestinationTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
     "SourceKeywordTypeDef",
     "ControlMetadataTypeDef",
     "CreateAssessmentFrameworkControlTypeDef",
     "CreateAssessmentReportRequestRequestTypeDef",
+    "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
+    "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
+    "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
     "URLTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetChangeLogsRequestRequestTypeDef",
     "GetControlRequestRequestTypeDef",
     "GetDelegationsRequestRequestTypeDef",
     "GetEvidenceByEvidenceFolderRequestRequestTypeDef",
+    "GetEvidenceFileUploadUrlRequestRequestTypeDef",
+    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     "GetEvidenceRequestRequestTypeDef",
     "GetInsightsByAssessmentRequestRequestTypeDef",
     "InsightsByAssessmentTypeDef",
     "InsightsTypeDef",
+    "GetOrganizationAdminAccountResponseTypeDef",
     "ServiceMetadataTypeDef",
     "GetSettingsRequestRequestTypeDef",
     "ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef",
     "ListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     "ListAssessmentFrameworksRequestRequestTypeDef",
     "ListAssessmentReportsRequestRequestTypeDef",
     "ListAssessmentsRequestRequestTypeDef",
     "ListControlDomainInsightsByAssessmentRequestRequestTypeDef",
     "ListControlDomainInsightsRequestRequestTypeDef",
     "ListControlInsightsByControlDomainRequestRequestTypeDef",
     "ListControlsRequestRequestTypeDef",
     "ListKeywordsForDataSourceRequestRequestTypeDef",
+    "ListKeywordsForDataSourceResponseTypeDef",
     "ListNotificationsRequestRequestTypeDef",
     "NotificationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RegisterAccountRequestRequestTypeDef",
+    "RegisterAccountResponseTypeDef",
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
+    "RegisterOrganizationAdminAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartAssessmentFrameworkShareRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    "CreateAssessmentReportResponseTypeDef",
-    "DeregisterAccountResponseTypeDef",
-    "GetAccountStatusResponseTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
-    "GetOrganizationAdminAccountResponseTypeDef",
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
     "ListAssessmentFrameworksResponseTypeDef",
-    "ListAssessmentReportsResponseTypeDef",
-    "ListKeywordsForDataSourceResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterAccountResponseTypeDef",
-    "RegisterOrganizationAdminAccountResponseTypeDef",
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
     "StartAssessmentFrameworkShareResponseTypeDef",
     "UpdateAssessmentFrameworkShareResponseTypeDef",
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    "ListAssessmentReportsResponseTypeDef",
+    "CreateAssessmentReportResponseTypeDef",
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     "BatchCreateDelegationByAssessmentRequestRequestTypeDef",
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
@@ -404,25 +408,14 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
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
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
         "roleArn": str,
         "roleType": RoleTypeType,
@@ -457,14 +450,16 @@
     },
 )
 
 ManualEvidenceTypeDef = TypedDict(
     "ManualEvidenceTypeDef",
     {
         "s3ResourcePath": str,
+        "textResponse": str,
+        "evidenceFileName": str,
     },
     total=False,
 )
 
 ChangeLogTypeDef = TypedDict(
     "ChangeLogTypeDef",
     {
@@ -486,15 +481,15 @@
     },
     total=False,
 )
 
 SourceKeywordTypeDef = TypedDict(
     "SourceKeywordTypeDef",
     {
-        "keywordInputType": Literal["SELECT_FROM_LIST"],
+        "keywordInputType": KeywordInputTypeType,
         "keywordValue": str,
     },
     total=False,
 )
 
 ControlMetadataTypeDef = TypedDict(
     "ControlMetadataTypeDef",
@@ -534,14 +529,23 @@
 
 class CreateAssessmentReportRequestRequestTypeDef(
     _RequiredCreateAssessmentReportRequestRequestTypeDef,
     _OptionalCreateAssessmentReportRequestRequestTypeDef,
 ):
     pass
 
+DefaultExportDestinationTypeDef = TypedDict(
+    "DefaultExportDestinationTypeDef",
+    {
+        "destinationType": Literal["S3"],
+        "destination": str,
+    },
+    total=False,
+)
+
 DelegationMetadataTypeDef = TypedDict(
     "DelegationMetadataTypeDef",
     {
         "id": str,
         "assessmentName": str,
         "assessmentId": str,
         "status": DelegationStatusType,
@@ -585,14 +589,22 @@
 DeleteControlRequestRequestTypeDef = TypedDict(
     "DeleteControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
+DeregisterAccountResponseTypeDef = TypedDict(
+    "DeregisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeregisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
@@ -630,14 +642,22 @@
         "arn": str,
         "value": str,
         "complianceCheck": str,
     },
     total=False,
 )
 
+GetAccountStatusResponseTypeDef = TypedDict(
+    "GetAccountStatusResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "GetAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
     },
 )
 
@@ -722,14 +742,30 @@
 
 class GetEvidenceByEvidenceFolderRequestRequestTypeDef(
     _RequiredGetEvidenceByEvidenceFolderRequestRequestTypeDef,
     _OptionalGetEvidenceByEvidenceFolderRequestRequestTypeDef,
 ):
     pass
 
+GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlRequestRequestTypeDef",
+    {
+        "fileName": str,
+    },
+)
+
+GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlResponseTypeDef",
+    {
+        "evidenceFileName": str,
+        "uploadUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEvidenceFolderRequestRequestTypeDef = TypedDict(
     "GetEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
     },
@@ -819,14 +855,23 @@
         "assessmentControlsCountByNoncompliantEvidence": int,
         "totalAssessmentControlsCount": int,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
+GetOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "GetOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
         "category": str,
@@ -1012,14 +1057,23 @@
 
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
+ListKeywordsForDataSourceResponseTypeDef = TypedDict(
+    "ListKeywordsForDataSourceResponseTypeDef",
+    {
+        "keywords": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListNotificationsRequestRequestTypeDef = TypedDict(
     "ListNotificationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1043,30 +1097,66 @@
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
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "kmsKey": str,
         "delegatedAdminAccount": str,
     },
     total=False,
 )
 
+RegisterAccountResponseTypeDef = TypedDict(
+    "RegisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
 )
 
+RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "RegisterOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
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
 _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "frameworkId": str,
         "destinationAccount": str,
         "destinationRegion": str,
     },
@@ -1154,14 +1244,26 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
+ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    {
+        "signatureValid": bool,
+        "signatureAlgorithm": str,
+        "signatureDateTime": str,
+        "signatureKeyId": str,
+        "validationErrors": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
     },
     total=False,
@@ -1194,177 +1296,106 @@
         "evidenceSources": List[str],
         "evidenceCount": int,
         "assessmentReportEvidenceCount": int,
     },
     total=False,
 )
 
-BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAssessmentReportResponseTypeDef = TypedDict(
-    "CreateAssessmentReportResponseTypeDef",
-    {
-        "assessmentReport": AssessmentReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterAccountResponseTypeDef = TypedDict(
-    "DeregisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccountStatusResponseTypeDef = TypedDict(
-    "GetAccountStatusResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceFolderResponseTypeDef",
     {
         "evidenceFolder": AssessmentEvidenceFolderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceFoldersByAssessmentControlResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceFoldersByAssessmentResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "GetOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
-    {
-        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentFrameworksResponseTypeDef = TypedDict(
     "ListAssessmentFrameworksResponseTypeDef",
     {
         "frameworkMetadataList": List[AssessmentFrameworkMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAssessmentReportsResponseTypeDef = TypedDict(
-    "ListAssessmentReportsResponseTypeDef",
-    {
-        "assessmentReports": List[AssessmentReportMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListKeywordsForDataSourceResponseTypeDef = TypedDict(
-    "ListKeywordsForDataSourceResponseTypeDef",
+ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
     {
-        "keywords": List[str],
+        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "StartAssessmentFrameworkShareResponseTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RegisterAccountResponseTypeDef = TypedDict(
-    "RegisterAccountResponseTypeDef",
+UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "UpdateAssessmentFrameworkShareResponseTypeDef",
     {
-        "status": AccountStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "RegisterOrganizationAdminAccountResponseTypeDef",
+BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
     {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "StartAssessmentFrameworkShareResponseTypeDef",
+BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "UpdateAssessmentFrameworkShareResponseTypeDef",
+ListAssessmentReportsResponseTypeDef = TypedDict(
+    "ListAssessmentReportsResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentReports": List[AssessmentReportMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+CreateAssessmentReportResponseTypeDef = TypedDict(
+    "CreateAssessmentReportResponseTypeDef",
     {
-        "signatureValid": bool,
-        "signatureAlgorithm": str,
-        "signatureDateTime": str,
-        "signatureKeyId": str,
-        "validationErrors": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentReport": AssessmentReportTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
         "createDelegationRequest": CreateDelegationRequestTypeDef,
@@ -1382,15 +1413,15 @@
     },
 )
 
 BatchDeleteDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     {
         "errors": List[BatchDeleteDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
         "manualEvidence": ManualEvidenceTypeDef,
@@ -1411,15 +1442,15 @@
 )
 
 GetChangeLogsResponseTypeDef = TypedDict(
     "GetChangeLogsResponseTypeDef",
     {
         "changeLogs": List[ChangeLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ControlDomainInsightsTypeDef = TypedDict(
     "ControlDomainInsightsTypeDef",
     {
         "name": str,
@@ -1485,15 +1516,15 @@
 )
 
 ListControlsResponseTypeDef = TypedDict(
     "ListControlsResponseTypeDef",
     {
         "controlMetadataList": List[ControlMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
@@ -1535,41 +1566,43 @@
     pass
 
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "snsTopic": str,
         "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "defaultProcessOwners": Sequence[RoleTypeDef],
         "kmsKey": str,
         "evidenceFinderEnabled": bool,
         "deregistrationPolicy": DeregistrationPolicyTypeDef,
+        "defaultExportDestination": DefaultExportDestinationTypeDef,
     },
     total=False,
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "isAwsOrgEnabled": bool,
         "snsTopic": str,
         "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "defaultProcessOwners": List[RoleTypeDef],
         "kmsKey": str,
         "evidenceFinderEnablement": EvidenceFinderEnablementTypeDef,
         "deregistrationPolicy": DeregistrationPolicyTypeDef,
+        "defaultExportDestination": DefaultExportDestinationTypeDef,
     },
     total=False,
 )
 
 EvidenceTypeDef = TypedDict(
     "EvidenceTypeDef",
     {
@@ -1592,48 +1625,48 @@
     total=False,
 )
 
 GetAssessmentReportUrlResponseTypeDef = TypedDict(
     "GetAssessmentReportUrlResponseTypeDef",
     {
         "preSignedUrl": URLTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightsByAssessmentResponseTypeDef = TypedDict(
     "GetInsightsByAssessmentResponseTypeDef",
     {
         "insights": InsightsByAssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "insights": InsightsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServicesInScopeResponseTypeDef = TypedDict(
     "GetServicesInScopeResponseTypeDef",
     {
         "serviceMetadata": List[ServiceMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNotificationsResponseTypeDef = TypedDict(
     "ListNotificationsResponseTypeDef",
     {
         "notifications": List[NotificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentMetadataTypeDef = TypedDict(
     "AssessmentMetadataTypeDef",
     {
         "name": str,
@@ -1699,15 +1732,15 @@
     pass
 
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
@@ -1722,68 +1755,68 @@
     total=False,
 )
 
 UpdateAssessmentControlResponseTypeDef = TypedDict(
     "UpdateAssessmentControlResponseTypeDef",
     {
         "control": AssessmentControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     {
         "delegations": List[DelegationTypeDef],
         "errors": List[BatchCreateDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchImportEvidenceToAssessmentControlResponseTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     {
         "errors": List[BatchImportEvidenceToAssessmentControlErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlDomainInsightsByAssessmentResponseTypeDef = TypedDict(
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlDomainInsightsResponseTypeDef = TypedDict(
     "ListControlDomainInsightsResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListAssessmentControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsByAssessment": List[ControlInsightsMetadataByAssessmentItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsMetadata": List[ControlInsightsMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ControlTypeDef = TypedDict(
     "ControlTypeDef",
     {
         "arn": str,
@@ -1899,40 +1932,40 @@
 ):
     pass
 
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSettingsResponseTypeDef = TypedDict(
     "UpdateSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceByEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceByEvidenceFolderResponseTypeDef",
     {
         "evidence": List[EvidenceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEvidenceResponseTypeDef = TypedDict(
     "GetEvidenceResponseTypeDef",
     {
         "evidence": EvidenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentFrameworkTypeDef = TypedDict(
     "AssessmentFrameworkTypeDef",
     {
         "id": str,
@@ -1943,15 +1976,15 @@
     total=False,
 )
 
 UpdateAssessmentControlSetStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusResponseTypeDef",
     {
         "controlSet": AssessmentControlSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ControlSetTypeDef = TypedDict(
     "ControlSetTypeDef",
     {
         "id": str,
@@ -1961,31 +1994,31 @@
     total=False,
 )
 
 CreateControlResponseTypeDef = TypedDict(
     "CreateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetControlResponseTypeDef = TypedDict(
     "GetControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateControlResponseTypeDef = TypedDict(
     "UpdateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
@@ -2018,59 +2051,59 @@
     total=False,
 )
 
 CreateAssessmentResponseTypeDef = TypedDict(
     "CreateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
         "userRole": RoleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentStatusResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssessmentFrameworkResponseTypeDef = TypedDict(
     "CreateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssessmentFrameworkResponseTypeDef = TypedDict(
     "GetAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentFrameworkResponseTypeDef = TypedDict(
     "UpdateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/PKG-INFO` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.26.75
-Summary: Type annotations for boto3.AuditManager 1.26.75 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.AuditManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-auditmanager"></a>
 
 # mypy-boto3-auditmanager
 
 [![PyPI - mypy-boto3-auditmanager](https://img.shields.io/pypi/v/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.26.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +289,15 @@
     ControlSetStatusType,
     ControlStatusType,
     ControlTypeType,
     DelegationStatusType,
     DeleteResourcesType,
     EvidenceFinderBackfillStatusType,
     EvidenceFinderEnablementStatusType,
+    ExportDestinationTypeType,
     FrameworkTypeType,
     KeywordInputTypeType,
     ObjectTypeEnumType,
     RoleTypeType,
     SettingAttributeType,
     ShareRequestActionType,
     ShareRequestStatusType,
@@ -335,99 +336,102 @@
     FrameworkMetadataTypeDef,
     AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
+    DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
+    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
+    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
+    GetEvidenceFileUploadUrlRequestRequestTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
+    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
-    DeregisterAccountResponseTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
-    ListAssessmentFrameworkShareRequestsResponseTypeDef,
     ListAssessmentFrameworksResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterAccountResponseTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
+    ListAssessmentFrameworkShareRequestsResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
@@ -493,42 +497,42 @@
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

### Comparing `mypy-boto3-auditmanager-1.26.75/mypy_boto3_auditmanager.egg-info/SOURCES.txt` & `mypy-boto3-auditmanager-1.27.0/mypy_boto3_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.26.75/setup.py` & `mypy-boto3-auditmanager-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-auditmanager.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-auditmanager",
-    version="1.26.75",
+    version="1.27.0",
     packages=["mypy_boto3_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AuditManager 1.26.75 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.AuditManager 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/",
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


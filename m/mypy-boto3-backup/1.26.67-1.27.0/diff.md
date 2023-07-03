# Comparing `tmp/mypy-boto3-backup-1.26.67.tar.gz` & `tmp/mypy-boto3-backup-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-1.26.67.tar", last modified: Wed Feb  8 20:27:03 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-1.27.0.tar", last modified: Mon Jul  3 19:50:25 2023, max compression
```

## Comparing `mypy-boto3-backup-1.26.67.tar` & `mypy-boto3-backup-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20554 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/mypy_boto3_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54858 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54766 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-02-08 20:26:21.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    67581 2023-02-08 20:26:24.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67506 2023-02-08 20:26:23.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-08 20:27:03.000000 mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 20:27:03.702110 mypy-boto3-backup-1.26.67/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-08 20:26:20.000000 mypy-boto3-backup-1.26.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.006866 mypy-boto3-backup-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-03 19:50:25.006866 mypy-boto3-backup-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.006866 mypy-boto3-backup-1.27.0/mypy_boto3_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54908 2023-07-03 19:33:01.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-03 19:33:01.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-03 19:33:01.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-07-03 19:33:01.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-03 19:33:01.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    67854 2023-07-03 19:33:03.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67779 2023-07-03 19:33:02.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.006866 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-03 19:50:24.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:24.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:24.000000 mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:25.006866 mypy-boto3-backup-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:33:00.000000 mypy-boto3-backup-1.27.0/setup.py
```

### Comparing `mypy-boto3-backup-1.26.67/LICENSE` & `mypy-boto3-backup-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-backup-1.26.67/PKG-INFO` & `mypy-boto3-backup-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.26.67
-Summary: Type annotations for boto3.Backup 1.26.67 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Backup 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-backup"></a>
 
 # mypy-boto3-backup
 
 [![PyPI - mypy-boto3-backup](https://img.shields.io/pypi/v/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.26.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,143 +390,143 @@
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
     ConditionParameterTypeDef,
     ControlInputParameterTypeDef,
     ControlScopeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultInputRequestTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
+    CreateReportPlanOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
+    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
+    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
+    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    PaginatorConfigTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
     ListBackupJobsInputRequestTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
     ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
     ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
     ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
+    ListTagsOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDestinationTypeDef,
+    ResponseMetadataTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
+    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
+    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
+    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    RecoveryPointByBackupVaultTypeDef,
-    ConditionsTypeDef,
-    FrameworkControlTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    CreateBackupSelectionOutputTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
-    CreateReportPlanOutputTypeDef,
-    DeleteBackupPlanOutputTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    DescribeBackupVaultOutputTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
-    DescribeRestoreJobOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     ListBackupSelectionsOutputTypeDef,
     ListBackupVaultsOutputTypeDef,
-    ListTagsOutputTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
-    StartReportJobOutputTypeDef,
-    StartRestoreJobOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
-    UpdateFrameworkOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    RecoveryPointByBackupVaultTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
-    UpdateReportPlanOutputTypeDef,
+    ConditionsTypeDef,
+    FrameworkControlTypeDef,
     CreateReportPlanInputRequestTypeDef,
     ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
@@ -566,42 +566,42 @@
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

### Comparing `mypy-boto3-backup-1.26.67/README.md` & `mypy-boto3-backup-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-backup"></a>
 
 # mypy-boto3-backup
 
 [![PyPI - mypy-boto3-backup](https://img.shields.io/pypi/v/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.26.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,143 +358,143 @@
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
     ConditionParameterTypeDef,
     ControlInputParameterTypeDef,
     ControlScopeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultInputRequestTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
+    CreateReportPlanOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
+    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
+    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
+    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    PaginatorConfigTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
     ListBackupJobsInputRequestTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
     ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
     ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
     ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
+    ListTagsOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDestinationTypeDef,
+    ResponseMetadataTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
+    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
+    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
+    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    RecoveryPointByBackupVaultTypeDef,
-    ConditionsTypeDef,
-    FrameworkControlTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    CreateBackupSelectionOutputTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
-    CreateReportPlanOutputTypeDef,
-    DeleteBackupPlanOutputTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    DescribeBackupVaultOutputTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
-    DescribeRestoreJobOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     ListBackupSelectionsOutputTypeDef,
     ListBackupVaultsOutputTypeDef,
-    ListTagsOutputTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
-    StartReportJobOutputTypeDef,
-    StartRestoreJobOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
-    UpdateFrameworkOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    RecoveryPointByBackupVaultTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
-    UpdateReportPlanOutputTypeDef,
+    ConditionsTypeDef,
+    FrameworkControlTypeDef,
     CreateReportPlanInputRequestTypeDef,
     ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
@@ -534,42 +534,42 @@
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

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.py` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/__init__.pyi` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/__main__.py` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Backup 1.26.67\nVersion:         1.26.67\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Backup 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.67")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.py` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         """
 
     def delete_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the resource selection associated with a backup plan that is specified
-        by the `SelectionId` .
+        by the `SelectionId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_selection)
         """
 
     def delete_backup_vault(self, *, BackupVaultName: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -352,15 +352,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_report_plan)
         """
 
     def describe_backup_job(self, *, BackupJobId: str) -> DescribeBackupJobOutputTypeDef:
         """
-        Returns backup job details for the specified `BackupJobId` .
+        Returns backup job details for the specified `BackupJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_backup_job)
         """
 
     def describe_backup_vault(self, *, BackupVaultName: str) -> DescribeBackupVaultOutputTypeDef:
         """
@@ -376,15 +376,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_copy_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_copy_job)
         """
 
     def describe_framework(self, *, FrameworkName: str) -> DescribeFrameworkOutputTypeDef:
         """
-        Returns the framework details for the specified `FrameworkName` .
+        Returns the framework details for the specified `FrameworkName`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_framework)
         """
 
     def describe_global_settings(self) -> DescribeGlobalSettingsOutputTypeDef:
         """
@@ -425,15 +425,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_region_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_region_settings)
         """
 
     def describe_report_job(self, *, ReportJobId: str) -> DescribeReportJobOutputTypeDef:
         """
         Returns the details associated with creating a report as specified by its
-        `ReportJobId` .
+        `ReportJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_report_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_report_job)
         """
 
     def describe_report_plan(self, *, ReportPlanName: str) -> DescribeReportPlanOutputTypeDef:
         """
@@ -912,15 +912,16 @@
     def start_restore_job(
         self,
         *,
         RecoveryPointArn: str,
         Metadata: Mapping[str, str],
         IamRoleArn: str = ...,
         IdempotencyToken: str = ...,
-        ResourceType: str = ...
+        ResourceType: str = ...,
+        CopySourceTagsToRestoredResource: bool = ...
     ) -> StartRestoreJobOutputTypeDef:
         """
         Recovers the saved resource identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_restore_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_restore_job)
         """
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/client.pyi` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_plan)
         """
     def delete_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the resource selection associated with a backup plan that is specified
-        by the `SelectionId` .
+        by the `SelectionId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_selection)
         """
     def delete_backup_vault(self, *, BackupVaultName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the backup vault identified by its name.
@@ -329,15 +329,15 @@
         Deletes the report plan specified by a report plan name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_report_plan)
         """
     def describe_backup_job(self, *, BackupJobId: str) -> DescribeBackupJobOutputTypeDef:
         """
-        Returns backup job details for the specified `BackupJobId` .
+        Returns backup job details for the specified `BackupJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_backup_job)
         """
     def describe_backup_vault(self, *, BackupVaultName: str) -> DescribeBackupVaultOutputTypeDef:
         """
         Returns metadata about a backup vault specified by its name.
@@ -350,15 +350,15 @@
         Returns metadata associated with creating a copy of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_copy_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_copy_job)
         """
     def describe_framework(self, *, FrameworkName: str) -> DescribeFrameworkOutputTypeDef:
         """
-        Returns the framework details for the specified `FrameworkName` .
+        Returns the framework details for the specified `FrameworkName`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_framework)
         """
     def describe_global_settings(self) -> DescribeGlobalSettingsOutputTypeDef:
         """
         Describes whether the Amazon Web Services account is opted in to cross-account
@@ -394,15 +394,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_region_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_region_settings)
         """
     def describe_report_job(self, *, ReportJobId: str) -> DescribeReportJobOutputTypeDef:
         """
         Returns the details associated with creating a report as specified by its
-        `ReportJobId` .
+        `ReportJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_report_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_report_job)
         """
     def describe_report_plan(self, *, ReportPlanName: str) -> DescribeReportPlanOutputTypeDef:
         """
         Returns a list of all report plans for an Amazon Web Services account and Amazon
@@ -842,15 +842,16 @@
     def start_restore_job(
         self,
         *,
         RecoveryPointArn: str,
         Metadata: Mapping[str, str],
         IamRoleArn: str = ...,
         IdempotencyToken: str = ...,
-        ResourceType: str = ...
+        ResourceType: str = ...,
+        CopySourceTagsToRestoredResource: bool = ...
     ) -> StartRestoreJobOutputTypeDef:
         """
         Recovers the saved resource identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_restore_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_restore_job)
         """
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.py` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/literals.py`

 * *Files 2% similar despite different names*

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
@@ -157,14 +158,15 @@
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
@@ -243,14 +245,15 @@
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
@@ -261,14 +264,15 @@
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
@@ -304,14 +308,15 @@
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
@@ -330,16 +335,19 @@
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
@@ -419,18 +427,21 @@
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
@@ -470,21 +481,25 @@
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

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/literals.pyi` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,14 +243,15 @@
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
@@ -259,14 +262,15 @@
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
@@ -302,14 +306,15 @@
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
@@ -328,16 +333,19 @@
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
@@ -417,18 +425,21 @@
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
@@ -468,21 +479,25 @@
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

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.py` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,90 +108,90 @@
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupjobspaginator)
         """
 
 
 class ListBackupPlanTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupPlanTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
         """
 
 
 class ListBackupPlanVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupPlanVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
         """
 
 
 class ListBackupPlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
     """
 
     def paginate(
-        self, *, IncludeDeleted: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, IncludeDeleted: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
         """
 
 
 class ListBackupSelectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupSelectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
         """
 
 
 class ListBackupVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
         """
 
 
@@ -210,45 +210,45 @@
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listcopyjobspaginator)
         """
 
 
 class ListLegalHoldsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLegalHoldsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
         """
 
 
 class ListProtectedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtectedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
         """
 
 
@@ -264,45 +264,45 @@
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 
 class ListRecoveryPointsByLegalHoldPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
     """
 
     def paginate(
-        self, *, LegalHoldId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, LegalHoldId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
         """
 
 
 class ListRecoveryPointsByResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsByResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
         """
 
 
@@ -317,13 +317,13 @@
         *,
         ByAccountId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/paginator.pyi` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -105,85 +105,85 @@
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupjobspaginator)
         """
 
 class ListBackupPlanTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupPlanTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplantemplatespaginator)
         """
 
 class ListBackupPlanVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupPlanVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanversionspaginator)
         """
 
 class ListBackupPlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
     """
 
     def paginate(
-        self, *, IncludeDeleted: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, IncludeDeleted: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupplanspaginator)
         """
 
 class ListBackupSelectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupSelectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupselectionspaginator)
         """
 
 class ListBackupVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupvaultspaginator)
         """
 
 class ListCopyJobsPaginator(Paginator):
@@ -201,43 +201,43 @@
         ByCreatedAfter: Union[datetime, str] = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listcopyjobspaginator)
         """
 
 class ListLegalHoldsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLegalHoldsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listlegalholdspaginator)
         """
 
 class ListProtectedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProtectedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listprotectedresourcespaginator)
         """
 
 class ListRecoveryPointsByBackupVaultPaginator(Paginator):
@@ -252,43 +252,43 @@
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 class ListRecoveryPointsByLegalHoldPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
     """
 
     def paginate(
-        self, *, LegalHoldId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, LegalHoldId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbylegalholdpaginator)
         """
 
 class ListRecoveryPointsByResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecoveryPointsByResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbyresourcepaginator)
         """
 
 class ListRestoreJobsPaginator(Paginator):
@@ -302,13 +302,13 @@
         *,
         ByAccountId: str = ...,
         ByCreatedBefore: Union[datetime, str] = ...,
         ByCreatedAfter: Union[datetime, str] = ...,
         ByStatus: RestoreJobStatusType = ...,
         ByCompleteBefore: Union[datetime, str] = ...,
         ByCompleteAfter: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.py` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,143 +44,143 @@
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
     "ConditionParameterTypeDef",
     "ControlInputParameterTypeDef",
     "ControlScopeTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBackupSelectionOutputTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
+    "CreateBackupVaultOutputTypeDef",
+    "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
+    "CreateReportPlanOutputTypeDef",
     "DateRangeTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
+    "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
     "DeleteRecoveryPointInputRequestTypeDef",
     "DeleteReportPlanInputRequestTypeDef",
     "DescribeBackupJobInputRequestTypeDef",
     "DescribeBackupVaultInputRequestTypeDef",
+    "DescribeBackupVaultOutputTypeDef",
     "DescribeCopyJobInputRequestTypeDef",
     "DescribeFrameworkInputRequestTypeDef",
+    "DescribeGlobalSettingsOutputTypeDef",
     "DescribeProtectedResourceInputRequestTypeDef",
+    "DescribeProtectedResourceOutputTypeDef",
     "DescribeRecoveryPointInputRequestTypeDef",
+    "DescribeRegionSettingsOutputTypeDef",
     "DescribeReportJobInputRequestTypeDef",
     "DescribeReportPlanInputRequestTypeDef",
     "DescribeRestoreJobInputRequestTypeDef",
+    "DescribeRestoreJobOutputTypeDef",
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     "DisassociateRecoveryPointInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportBackupPlanTemplateInputRequestTypeDef",
+    "ExportBackupPlanTemplateOutputTypeDef",
     "FrameworkTypeDef",
     "GetBackupPlanFromJSONInputRequestTypeDef",
     "GetBackupPlanFromTemplateInputRequestTypeDef",
     "GetBackupPlanInputRequestTypeDef",
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
+    "GetBackupVaultAccessPolicyOutputTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
+    "GetBackupVaultNotificationsOutputTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    "GetSupportedResourceTypesOutputTypeDef",
     "LegalHoldTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     "ListBackupJobsInputRequestTypeDef",
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
+    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupPlansInputRequestTypeDef",
+    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
     "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
+    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
     "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
+    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
     "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
+    "ListTagsOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
     "ReportDestinationTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartBackupJobOutputTypeDef",
+    "StartCopyJobOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
+    "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
+    "StartRestoreJobOutputTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateFrameworkOutputTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
+    "UpdateReportPlanOutputTypeDef",
     "BackupPlansListMemberTypeDef",
+    "CreateBackupPlanOutputTypeDef",
+    "UpdateBackupPlanOutputTypeDef",
     "BackupJobTypeDef",
     "CopyJobTypeDef",
+    "DescribeBackupJobOutputTypeDef",
+    "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
-    "RecoveryPointByBackupVaultTypeDef",
-    "ConditionsTypeDef",
-    "FrameworkControlTypeDef",
-    "CreateBackupPlanOutputTypeDef",
-    "CreateBackupSelectionOutputTypeDef",
-    "CreateBackupVaultOutputTypeDef",
-    "CreateFrameworkOutputTypeDef",
-    "CreateReportPlanOutputTypeDef",
-    "DeleteBackupPlanOutputTypeDef",
-    "DescribeBackupJobOutputTypeDef",
-    "DescribeBackupVaultOutputTypeDef",
-    "DescribeGlobalSettingsOutputTypeDef",
-    "DescribeProtectedResourceOutputTypeDef",
-    "DescribeRecoveryPointOutputTypeDef",
-    "DescribeRegionSettingsOutputTypeDef",
-    "DescribeRestoreJobOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportBackupPlanTemplateOutputTypeDef",
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    "GetBackupVaultNotificationsOutputTypeDef",
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    "GetSupportedResourceTypesOutputTypeDef",
-    "ListBackupPlanTemplatesOutputTypeDef",
     "ListBackupSelectionsOutputTypeDef",
     "ListBackupVaultsOutputTypeDef",
-    "ListTagsOutputTypeDef",
-    "StartBackupJobOutputTypeDef",
-    "StartCopyJobOutputTypeDef",
-    "StartReportJobOutputTypeDef",
-    "StartRestoreJobOutputTypeDef",
-    "UpdateBackupPlanOutputTypeDef",
-    "UpdateFrameworkOutputTypeDef",
+    "DescribeRecoveryPointOutputTypeDef",
+    "RecoveryPointByBackupVaultTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
-    "UpdateReportPlanOutputTypeDef",
+    "ConditionsTypeDef",
+    "FrameworkControlTypeDef",
     "CreateReportPlanInputRequestTypeDef",
     "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
     "RecoveryPointSelectionTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
-    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
     "ReportJobTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
@@ -344,22 +344,21 @@
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBackupSelectionOutputTypeDef = TypedDict(
+    "CreateBackupSelectionOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
@@ -378,14 +377,33 @@
 
 class CreateBackupVaultInputRequestTypeDef(
     _RequiredCreateBackupVaultInputRequestTypeDef, _OptionalCreateBackupVaultInputRequestTypeDef
 ):
     pass
 
 
+CreateBackupVaultOutputTypeDef = TypedDict(
+    "CreateBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFrameworkOutputTypeDef = TypedDict(
+    "CreateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredReportDeliveryChannelTypeDef = TypedDict(
     "_RequiredReportDeliveryChannelTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalReportDeliveryChannelTypeDef = TypedDict(
@@ -423,14 +441,24 @@
 )
 
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
 
+CreateReportPlanOutputTypeDef = TypedDict(
+    "CreateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "FromDate": Union[datetime, str],
         "ToDate": Union[datetime, str],
     },
 )
@@ -438,14 +466,25 @@
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
+DeleteBackupPlanOutputTypeDef = TypedDict(
+    "DeleteBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "DeletionDate": datetime,
+        "VersionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBackupSelectionInputRequestTypeDef = TypedDict(
     "DeleteBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "SelectionId": str,
     },
 )
@@ -510,43 +549,89 @@
 DescribeBackupVaultInputRequestTypeDef = TypedDict(
     "DescribeBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
+DescribeBackupVaultOutputTypeDef = TypedDict(
+    "DescribeBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "EncryptionKeyArn": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "NumberOfRecoveryPoints": int,
+        "Locked": bool,
+        "MinRetentionDays": int,
+        "MaxRetentionDays": int,
+        "LockDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeCopyJobInputRequestTypeDef = TypedDict(
     "DescribeCopyJobInputRequestTypeDef",
     {
         "CopyJobId": str,
     },
 )
 
 DescribeFrameworkInputRequestTypeDef = TypedDict(
     "DescribeFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 
+DescribeGlobalSettingsOutputTypeDef = TypedDict(
+    "DescribeGlobalSettingsOutputTypeDef",
+    {
+        "GlobalSettings": Dict[str, str],
+        "LastUpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProtectedResourceInputRequestTypeDef = TypedDict(
     "DescribeProtectedResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+DescribeProtectedResourceOutputTypeDef = TypedDict(
+    "DescribeProtectedResourceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceType": str,
+        "LastBackupTime": datetime,
+        "ResourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRecoveryPointInputRequestTypeDef = TypedDict(
     "DescribeRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
+DescribeRegionSettingsOutputTypeDef = TypedDict(
+    "DescribeRegionSettingsOutputTypeDef",
+    {
+        "ResourceTypeOptInPreference": Dict[str, bool],
+        "ResourceTypeManagementPreference": Dict[str, bool],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeReportJobInputRequestTypeDef = TypedDict(
     "DescribeReportJobInputRequestTypeDef",
     {
         "ReportJobId": str,
     },
 )
 
@@ -560,14 +645,34 @@
 DescribeRestoreJobInputRequestTypeDef = TypedDict(
     "DescribeRestoreJobInputRequestTypeDef",
     {
         "RestoreJobId": str,
     },
 )
 
+DescribeRestoreJobOutputTypeDef = TypedDict(
+    "DescribeRestoreJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "RestoreJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "Status": RestoreJobStatusType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "ExpectedCompletionTimeMinutes": int,
+        "CreatedResourceArn": str,
+        "ResourceType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateRecoveryPointFromParentInputRequestTypeDef = TypedDict(
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
@@ -576,21 +681,36 @@
     "DisassociateRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportBackupPlanTemplateInputRequestTypeDef = TypedDict(
     "ExportBackupPlanTemplateInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
+ExportBackupPlanTemplateOutputTypeDef = TypedDict(
+    "ExportBackupPlanTemplateOutputTypeDef",
+    {
+        "BackupPlanTemplateJson": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FrameworkTypeDef = TypedDict(
     "FrameworkTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "NumberOfControls": int,
@@ -646,21 +766,42 @@
 GetBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
+GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBackupVaultNotificationsInputRequestTypeDef = TypedDict(
     "GetBackupVaultNotificationsInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
+GetBackupVaultNotificationsOutputTypeDef = TypedDict(
+    "GetBackupVaultNotificationsOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SNSTopicArn": str,
+        "BackupVaultEvents": List[BackupVaultEventType],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLegalHoldInputRequestTypeDef = TypedDict(
     "GetLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 
@@ -668,34 +809,60 @@
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
+GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "RestoreMetadata": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSupportedResourceTypesOutputTypeDef = TypedDict(
+    "GetSupportedResourceTypesOutputTypeDef",
+    {
+        "ResourceTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LegalHoldTypeDef = TypedDict(
     "LegalHoldTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBackupJobsInputRequestTypeDef = TypedDict(
     "ListBackupJobsInputRequestTypeDef",
     {
@@ -711,23 +878,53 @@
         "ByCompleteAfter": Union[datetime, str],
         "ByCompleteBefore": Union[datetime, str],
         "ByParentJobId": str,
     },
     total=False,
 )
 
+ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
+    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBackupPlanVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupPlanVersionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupPlanVersionsInputRequestTypeDef = TypedDict(
@@ -743,24 +940,55 @@
 class ListBackupPlanVersionsInputRequestTypeDef(
     _RequiredListBackupPlanVersionsInputRequestTypeDef,
     _OptionalListBackupPlanVersionsInputRequestTypeDef,
 ):
     pass
 
 
+ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    {
+        "IncludeDeleted": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBackupPlansInputRequestTypeDef = TypedDict(
     "ListBackupPlansInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IncludeDeleted": bool,
     },
     total=False,
 )
 
+_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
+    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBackupSelectionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupSelectionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupSelectionsInputRequestTypeDef = TypedDict(
@@ -776,23 +1004,49 @@
 class ListBackupSelectionsInputRequestTypeDef(
     _RequiredListBackupSelectionsInputRequestTypeDef,
     _OptionalListBackupSelectionsInputRequestTypeDef,
 ):
     pass
 
 
+ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBackupVaultsInputRequestTypeDef = TypedDict(
     "ListBackupVaultsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCopyJobsInputRequestTypeDef = TypedDict(
     "ListCopyJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByResourceArn": str,
         "ByState": CopyJobStateType,
@@ -813,23 +1067,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLegalHoldsInputRequestTypeDef = TypedDict(
     "ListLegalHoldsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProtectedResourcesInputRequestTypeDef = TypedDict(
     "ListProtectedResourcesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -842,14 +1112,42 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
+_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByParentRecoveryPointArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
@@ -871,14 +1169,36 @@
 class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
     _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
     _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "LegalHoldId": str,
+    },
+)
+_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
+    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -898,18 +1218,43 @@
     pass
 
 
 RecoveryPointMemberTypeDef = TypedDict(
     "RecoveryPointMemberTypeDef",
     {
         "RecoveryPointArn": str,
+        "ResourceArn": str,
+        "ResourceType": str,
+        "BackupVaultName": str,
     },
     total=False,
 )
 
+_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
+    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
@@ -964,14 +1309,28 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
+    {
+        "ByAccountId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRestoreJobsInputRequestTypeDef = TypedDict(
     "ListRestoreJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByAccountId": str,
         "ByCreatedBefore": Union[datetime, str],
@@ -1021,14 +1380,33 @@
 
 class ListTagsInputRequestTypeDef(
     _RequiredListTagsInputRequestTypeDef, _OptionalListTagsInputRequestTypeDef
 ):
     pass
 
 
+ListTagsOutputTypeDef = TypedDict(
+    "ListTagsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
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
 _RequiredPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -1085,14 +1463,46 @@
     {
         "S3BucketName": str,
         "S3Keys": List[str],
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
+StartBackupJobOutputTypeDef = TypedDict(
+    "StartBackupJobOutputTypeDef",
+    {
+        "BackupJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartCopyJobOutputTypeDef = TypedDict(
+    "StartCopyJobOutputTypeDef",
+    {
+        "CopyJobId": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1106,38 +1516,55 @@
 
 class StartReportJobInputRequestTypeDef(
     _RequiredStartReportJobInputRequestTypeDef, _OptionalStartReportJobInputRequestTypeDef
 ):
     pass
 
 
+StartReportJobOutputTypeDef = TypedDict(
+    "StartReportJobOutputTypeDef",
+    {
+        "ReportJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartRestoreJobInputRequestTypeDef = TypedDict(
     "_RequiredStartRestoreJobInputRequestTypeDef",
     {
         "RecoveryPointArn": str,
         "Metadata": Mapping[str, str],
     },
 )
 _OptionalStartRestoreJobInputRequestTypeDef = TypedDict(
     "_OptionalStartRestoreJobInputRequestTypeDef",
     {
         "IamRoleArn": str,
         "IdempotencyToken": str,
         "ResourceType": str,
+        "CopySourceTagsToRestoredResource": bool,
     },
     total=False,
 )
 
 
 class StartRestoreJobInputRequestTypeDef(
     _RequiredStartRestoreJobInputRequestTypeDef, _OptionalStartRestoreJobInputRequestTypeDef
 ):
     pass
 
 
+StartRestoreJobOutputTypeDef = TypedDict(
+    "StartRestoreJobOutputTypeDef",
+    {
+        "RestoreJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopBackupJobInputRequestTypeDef = TypedDict(
     "StopBackupJobInputRequestTypeDef",
     {
         "BackupJobId": str,
     },
 )
 
@@ -1153,14 +1580,24 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeyList": Sequence[str],
     },
 )
 
+UpdateFrameworkOutputTypeDef = TypedDict(
+    "UpdateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "GlobalSettings": Mapping[str, str],
     },
     total=False,
 )
@@ -1170,14 +1607,24 @@
     {
         "ResourceTypeOptInPreference": Mapping[str, bool],
         "ResourceTypeManagementPreference": Mapping[str, bool],
     },
     total=False,
 )
 
+UpdateReportPlanOutputTypeDef = TypedDict(
+    "UpdateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BackupPlansListMemberTypeDef = TypedDict(
     "BackupPlansListMemberTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
@@ -1186,14 +1633,38 @@
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
     },
     total=False,
 )
 
+CreateBackupPlanOutputTypeDef = TypedDict(
+    "CreateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBackupPlanOutputTypeDef = TypedDict(
+    "UpdateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
         "AccountId": str,
         "BackupJobId": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
@@ -1244,14 +1715,55 @@
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
         "ResourceName": str,
     },
     total=False,
 )
 
+DescribeBackupJobOutputTypeDef = TypedDict(
+    "DescribeBackupJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "BackupJobId": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "ResourceArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "State": BackupJobStateType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "ResourceType": str,
+        "BytesTransferred": int,
+        "ExpectedCompletionDate": datetime,
+        "StartBy": datetime,
+        "BackupOptions": Dict[str, str],
+        "BackupType": str,
+        "ParentJobId": str,
+        "IsParent": bool,
+        "NumberOfChildJobs": int,
+        "ChildJobsInState": Dict[BackupJobStateType, int],
+        "ResourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupPlanTemplatesOutputTypeDef = TypedDict(
+    "ListBackupPlanTemplatesOutputTypeDef",
+    {
+        "NextToken": str,
+        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
         "DestinationBackupVaultArn": str,
     },
 )
 _OptionalCopyActionTypeDef = TypedDict(
@@ -1339,16 +1851,34 @@
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
 
-RecoveryPointByBackupVaultTypeDef = TypedDict(
-    "RecoveryPointByBackupVaultTypeDef",
+ListBackupSelectionsOutputTypeDef = TypedDict(
+    "ListBackupSelectionsOutputTypeDef",
+    {
+        "NextToken": str,
+        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupVaultsOutputTypeDef = TypedDict(
+    "ListBackupVaultsOutputTypeDef",
+    {
+        "BackupVaultList": List[BackupVaultListMemberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeRecoveryPointOutputTypeDef = TypedDict(
+    "DescribeRecoveryPointOutputTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1359,187 +1889,26 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
+        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ConditionsTypeDef = TypedDict(
-    "ConditionsTypeDef",
-    {
-        "StringEquals": Sequence[ConditionParameterTypeDef],
-        "StringNotEquals": Sequence[ConditionParameterTypeDef],
-        "StringLike": Sequence[ConditionParameterTypeDef],
-        "StringNotLike": Sequence[ConditionParameterTypeDef],
-    },
-    total=False,
-)
-
-_RequiredFrameworkControlTypeDef = TypedDict(
-    "_RequiredFrameworkControlTypeDef",
-    {
-        "ControlName": str,
-    },
-)
-_OptionalFrameworkControlTypeDef = TypedDict(
-    "_OptionalFrameworkControlTypeDef",
-    {
-        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeTypeDef,
-    },
-    total=False,
 )
 
-
-class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
-    pass
-
-
-CreateBackupPlanOutputTypeDef = TypedDict(
-    "CreateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBackupSelectionOutputTypeDef = TypedDict(
-    "CreateBackupSelectionOutputTypeDef",
-    {
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBackupVaultOutputTypeDef = TypedDict(
-    "CreateBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFrameworkOutputTypeDef = TypedDict(
-    "CreateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReportPlanOutputTypeDef = TypedDict(
-    "CreateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBackupPlanOutputTypeDef = TypedDict(
-    "DeleteBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "DeletionDate": datetime,
-        "VersionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupJobOutputTypeDef = TypedDict(
-    "DescribeBackupJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "BackupJobId": str,
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "State": BackupJobStateType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "ResourceType": str,
-        "BytesTransferred": int,
-        "ExpectedCompletionDate": datetime,
-        "StartBy": datetime,
-        "BackupOptions": Dict[str, str],
-        "BackupType": str,
-        "ParentJobId": str,
-        "IsParent": bool,
-        "NumberOfChildJobs": int,
-        "ChildJobsInState": Dict[BackupJobStateType, int],
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupVaultOutputTypeDef = TypedDict(
-    "DescribeBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "EncryptionKeyArn": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "NumberOfRecoveryPoints": int,
-        "Locked": bool,
-        "MinRetentionDays": int,
-        "MaxRetentionDays": int,
-        "LockDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGlobalSettingsOutputTypeDef = TypedDict(
-    "DescribeGlobalSettingsOutputTypeDef",
-    {
-        "GlobalSettings": Dict[str, str],
-        "LastUpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeProtectedResourceOutputTypeDef = TypedDict(
-    "DescribeProtectedResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceType": str,
-        "LastBackupTime": datetime,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRecoveryPointOutputTypeDef = TypedDict(
-    "DescribeRecoveryPointOutputTypeDef",
+RecoveryPointByBackupVaultTypeDef = TypedDict(
+    "RecoveryPointByBackupVaultTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1550,222 +1919,64 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
-        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRegionSettingsOutputTypeDef = TypedDict(
-    "DescribeRegionSettingsOutputTypeDef",
-    {
-        "ResourceTypeOptInPreference": Dict[str, bool],
-        "ResourceTypeManagementPreference": Dict[str, bool],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRestoreJobOutputTypeDef = TypedDict(
-    "DescribeRestoreJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "RestoreJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "Status": RestoreJobStatusType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "ExpectedCompletionTimeMinutes": int,
-        "CreatedResourceArn": str,
-        "ResourceType": str,
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
-ExportBackupPlanTemplateOutputTypeDef = TypedDict(
-    "ExportBackupPlanTemplateOutputTypeDef",
-    {
-        "BackupPlanTemplateJson": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBackupVaultNotificationsOutputTypeDef = TypedDict(
-    "GetBackupVaultNotificationsOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "SNSTopicArn": str,
-        "BackupVaultEvents": List[BackupVaultEventType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "RestoreMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSupportedResourceTypesOutputTypeDef = TypedDict(
-    "GetSupportedResourceTypesOutputTypeDef",
-    {
-        "ResourceTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupPlanTemplatesOutputTypeDef = TypedDict(
-    "ListBackupPlanTemplatesOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupSelectionsOutputTypeDef = TypedDict(
-    "ListBackupSelectionsOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupVaultsOutputTypeDef = TypedDict(
-    "ListBackupVaultsOutputTypeDef",
-    {
-        "BackupVaultList": List[BackupVaultListMemberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsOutputTypeDef = TypedDict(
-    "ListTagsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBackupJobOutputTypeDef = TypedDict(
-    "StartBackupJobOutputTypeDef",
-    {
-        "BackupJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartCopyJobOutputTypeDef = TypedDict(
-    "StartCopyJobOutputTypeDef",
-    {
-        "CopyJobId": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Lifecycle": LifecycleTypeDef,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartReportJobOutputTypeDef = TypedDict(
-    "StartReportJobOutputTypeDef",
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
     {
-        "ReportJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StringEquals": Sequence[ConditionParameterTypeDef],
+        "StringNotEquals": Sequence[ConditionParameterTypeDef],
+        "StringLike": Sequence[ConditionParameterTypeDef],
+        "StringNotLike": Sequence[ConditionParameterTypeDef],
     },
+    total=False,
 )
 
-StartRestoreJobOutputTypeDef = TypedDict(
-    "StartRestoreJobOutputTypeDef",
+_RequiredFrameworkControlTypeDef = TypedDict(
+    "_RequiredFrameworkControlTypeDef",
     {
-        "RestoreJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ControlName": str,
     },
 )
-
-UpdateBackupPlanOutputTypeDef = TypedDict(
-    "UpdateBackupPlanOutputTypeDef",
+_OptionalFrameworkControlTypeDef = TypedDict(
+    "_OptionalFrameworkControlTypeDef",
     {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeTypeDef,
     },
+    total=False,
 )
 
-UpdateFrameworkOutputTypeDef = TypedDict(
-    "UpdateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
-    {
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "Lifecycle": LifecycleTypeDef,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
+    pass
 
-UpdateReportPlanOutputTypeDef = TypedDict(
-    "UpdateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
         "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
         "ReportSetting": ReportSettingTypeDef,
@@ -1839,267 +2050,60 @@
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
         "Frameworks": List[FrameworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLegalHoldsOutputTypeDef = TypedDict(
     "ListLegalHoldsOutputTypeDef",
     {
         "NextToken": str,
         "LegalHolds": List[LegalHoldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
-    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    {
-        "IncludeDeleted": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
-    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-):
-    pass
-
-
-ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "LegalHoldId": str,
-    },
-)
-_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
-    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
-    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-):
-    pass
-
-
-ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    {
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
     {
         "Results": List[ProtectedResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryPointsByLegalHoldOutputTypeDef = TypedDict(
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     {
         "RecoveryPoints": List[RecoveryPointMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryPointsByResourceOutputTypeDef = TypedDict(
     "ListRecoveryPointsByResourceOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRestoreJobsOutputTypeDef = TypedDict(
     "ListRestoreJobsOutputTypeDef",
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
@@ -2115,50 +2119,50 @@
 )
 
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupPlansOutputTypeDef = TypedDict(
     "ListBackupPlansOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlansList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupJobsOutputTypeDef = TypedDict(
     "ListBackupJobsOutputTypeDef",
     {
         "BackupJobs": List[BackupJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCopyJobOutputTypeDef = TypedDict(
     "DescribeCopyJobOutputTypeDef",
     {
         "CopyJob": CopyJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCopyJobsOutputTypeDef = TypedDict(
     "ListCopyJobsOutputTypeDef",
     {
         "CopyJobs": List[CopyJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupRuleInputTypeDef = TypedDict(
     "_RequiredBackupRuleInputTypeDef",
     {
         "RuleName": str,
@@ -2212,15 +2216,15 @@
 
 
 ListRecoveryPointsByBackupVaultOutputTypeDef = TypedDict(
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupSelectionTypeDef = TypedDict(
     "_RequiredBackupSelectionTypeDef",
     {
         "SelectionName": str,
@@ -2274,15 +2278,15 @@
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "FrameworkControls": List[FrameworkControlTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
@@ -2305,24 +2309,24 @@
     pass
 
 
 DescribeReportPlanOutputTypeDef = TypedDict(
     "DescribeReportPlanOutputTypeDef",
     {
         "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReportPlansOutputTypeDef = TypedDict(
     "ListReportPlansOutputTypeDef",
     {
         "ReportPlans": List[ReportPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
         "Title": str,
@@ -2352,15 +2356,15 @@
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLegalHoldOutputTypeDef = TypedDict(
     "GetLegalHoldOutputTypeDef",
     {
         "Title": str,
@@ -2369,32 +2373,32 @@
         "CancelDescription": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReportJobsOutputTypeDef = TypedDict(
     "ListReportJobsOutputTypeDef",
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
@@ -2461,15 +2465,15 @@
     "GetBackupSelectionOutputTypeDef",
     {
         "BackupSelection": BackupSelectionTypeDef,
         "SelectionId": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "CreatorRequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
@@ -2499,23 +2503,23 @@
     },
 )
 
 GetBackupPlanFromJSONOutputTypeDef = TypedDict(
     "GetBackupPlanFromJSONOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBackupPlanFromTemplateOutputTypeDef = TypedDict(
     "GetBackupPlanFromTemplateOutputTypeDef",
     {
         "BackupPlanDocument": BackupPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBackupPlanOutputTypeDef = TypedDict(
     "GetBackupPlanOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
@@ -2523,10 +2527,10 @@
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup/type_defs.pyi` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -43,143 +43,143 @@
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
     "ConditionParameterTypeDef",
     "ControlInputParameterTypeDef",
     "ControlScopeTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBackupSelectionOutputTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
+    "CreateBackupVaultOutputTypeDef",
+    "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
+    "CreateReportPlanOutputTypeDef",
     "DateRangeTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
+    "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
     "DeleteRecoveryPointInputRequestTypeDef",
     "DeleteReportPlanInputRequestTypeDef",
     "DescribeBackupJobInputRequestTypeDef",
     "DescribeBackupVaultInputRequestTypeDef",
+    "DescribeBackupVaultOutputTypeDef",
     "DescribeCopyJobInputRequestTypeDef",
     "DescribeFrameworkInputRequestTypeDef",
+    "DescribeGlobalSettingsOutputTypeDef",
     "DescribeProtectedResourceInputRequestTypeDef",
+    "DescribeProtectedResourceOutputTypeDef",
     "DescribeRecoveryPointInputRequestTypeDef",
+    "DescribeRegionSettingsOutputTypeDef",
     "DescribeReportJobInputRequestTypeDef",
     "DescribeReportPlanInputRequestTypeDef",
     "DescribeRestoreJobInputRequestTypeDef",
+    "DescribeRestoreJobOutputTypeDef",
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     "DisassociateRecoveryPointInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportBackupPlanTemplateInputRequestTypeDef",
+    "ExportBackupPlanTemplateOutputTypeDef",
     "FrameworkTypeDef",
     "GetBackupPlanFromJSONInputRequestTypeDef",
     "GetBackupPlanFromTemplateInputRequestTypeDef",
     "GetBackupPlanInputRequestTypeDef",
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
+    "GetBackupVaultAccessPolicyOutputTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
+    "GetBackupVaultNotificationsOutputTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    "GetSupportedResourceTypesOutputTypeDef",
     "LegalHoldTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     "ListBackupJobsInputRequestTypeDef",
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
+    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupPlansInputRequestTypeDef",
+    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
     "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
+    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
     "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
+    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
     "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
+    "ListTagsOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
     "ReportDestinationTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartBackupJobOutputTypeDef",
+    "StartCopyJobOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
+    "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
+    "StartRestoreJobOutputTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateFrameworkOutputTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
+    "UpdateReportPlanOutputTypeDef",
     "BackupPlansListMemberTypeDef",
+    "CreateBackupPlanOutputTypeDef",
+    "UpdateBackupPlanOutputTypeDef",
     "BackupJobTypeDef",
     "CopyJobTypeDef",
+    "DescribeBackupJobOutputTypeDef",
+    "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
-    "RecoveryPointByBackupVaultTypeDef",
-    "ConditionsTypeDef",
-    "FrameworkControlTypeDef",
-    "CreateBackupPlanOutputTypeDef",
-    "CreateBackupSelectionOutputTypeDef",
-    "CreateBackupVaultOutputTypeDef",
-    "CreateFrameworkOutputTypeDef",
-    "CreateReportPlanOutputTypeDef",
-    "DeleteBackupPlanOutputTypeDef",
-    "DescribeBackupJobOutputTypeDef",
-    "DescribeBackupVaultOutputTypeDef",
-    "DescribeGlobalSettingsOutputTypeDef",
-    "DescribeProtectedResourceOutputTypeDef",
-    "DescribeRecoveryPointOutputTypeDef",
-    "DescribeRegionSettingsOutputTypeDef",
-    "DescribeRestoreJobOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportBackupPlanTemplateOutputTypeDef",
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    "GetBackupVaultNotificationsOutputTypeDef",
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    "GetSupportedResourceTypesOutputTypeDef",
-    "ListBackupPlanTemplatesOutputTypeDef",
     "ListBackupSelectionsOutputTypeDef",
     "ListBackupVaultsOutputTypeDef",
-    "ListTagsOutputTypeDef",
-    "StartBackupJobOutputTypeDef",
-    "StartCopyJobOutputTypeDef",
-    "StartReportJobOutputTypeDef",
-    "StartRestoreJobOutputTypeDef",
-    "UpdateBackupPlanOutputTypeDef",
-    "UpdateFrameworkOutputTypeDef",
+    "DescribeRecoveryPointOutputTypeDef",
+    "RecoveryPointByBackupVaultTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
-    "UpdateReportPlanOutputTypeDef",
+    "ConditionsTypeDef",
+    "FrameworkControlTypeDef",
     "CreateReportPlanInputRequestTypeDef",
     "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
     "RecoveryPointSelectionTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
-    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
     "ReportJobTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
@@ -341,22 +341,21 @@
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBackupSelectionOutputTypeDef = TypedDict(
+    "CreateBackupSelectionOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
@@ -373,14 +372,33 @@
 )
 
 class CreateBackupVaultInputRequestTypeDef(
     _RequiredCreateBackupVaultInputRequestTypeDef, _OptionalCreateBackupVaultInputRequestTypeDef
 ):
     pass
 
+CreateBackupVaultOutputTypeDef = TypedDict(
+    "CreateBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFrameworkOutputTypeDef = TypedDict(
+    "CreateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredReportDeliveryChannelTypeDef = TypedDict(
     "_RequiredReportDeliveryChannelTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalReportDeliveryChannelTypeDef = TypedDict(
@@ -414,14 +432,24 @@
     },
     total=False,
 )
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
+CreateReportPlanOutputTypeDef = TypedDict(
+    "CreateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "FromDate": Union[datetime, str],
         "ToDate": Union[datetime, str],
     },
 )
@@ -429,14 +457,25 @@
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
+DeleteBackupPlanOutputTypeDef = TypedDict(
+    "DeleteBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "DeletionDate": datetime,
+        "VersionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBackupSelectionInputRequestTypeDef = TypedDict(
     "DeleteBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "SelectionId": str,
     },
 )
@@ -501,43 +540,89 @@
 DescribeBackupVaultInputRequestTypeDef = TypedDict(
     "DescribeBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
+DescribeBackupVaultOutputTypeDef = TypedDict(
+    "DescribeBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "EncryptionKeyArn": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "NumberOfRecoveryPoints": int,
+        "Locked": bool,
+        "MinRetentionDays": int,
+        "MaxRetentionDays": int,
+        "LockDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeCopyJobInputRequestTypeDef = TypedDict(
     "DescribeCopyJobInputRequestTypeDef",
     {
         "CopyJobId": str,
     },
 )
 
 DescribeFrameworkInputRequestTypeDef = TypedDict(
     "DescribeFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 
+DescribeGlobalSettingsOutputTypeDef = TypedDict(
+    "DescribeGlobalSettingsOutputTypeDef",
+    {
+        "GlobalSettings": Dict[str, str],
+        "LastUpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProtectedResourceInputRequestTypeDef = TypedDict(
     "DescribeProtectedResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+DescribeProtectedResourceOutputTypeDef = TypedDict(
+    "DescribeProtectedResourceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceType": str,
+        "LastBackupTime": datetime,
+        "ResourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeRecoveryPointInputRequestTypeDef = TypedDict(
     "DescribeRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
+DescribeRegionSettingsOutputTypeDef = TypedDict(
+    "DescribeRegionSettingsOutputTypeDef",
+    {
+        "ResourceTypeOptInPreference": Dict[str, bool],
+        "ResourceTypeManagementPreference": Dict[str, bool],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeReportJobInputRequestTypeDef = TypedDict(
     "DescribeReportJobInputRequestTypeDef",
     {
         "ReportJobId": str,
     },
 )
 
@@ -551,14 +636,34 @@
 DescribeRestoreJobInputRequestTypeDef = TypedDict(
     "DescribeRestoreJobInputRequestTypeDef",
     {
         "RestoreJobId": str,
     },
 )
 
+DescribeRestoreJobOutputTypeDef = TypedDict(
+    "DescribeRestoreJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "RestoreJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "Status": RestoreJobStatusType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "ExpectedCompletionTimeMinutes": int,
+        "CreatedResourceArn": str,
+        "ResourceType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateRecoveryPointFromParentInputRequestTypeDef = TypedDict(
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
@@ -567,21 +672,36 @@
     "DisassociateRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportBackupPlanTemplateInputRequestTypeDef = TypedDict(
     "ExportBackupPlanTemplateInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
+ExportBackupPlanTemplateOutputTypeDef = TypedDict(
+    "ExportBackupPlanTemplateOutputTypeDef",
+    {
+        "BackupPlanTemplateJson": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FrameworkTypeDef = TypedDict(
     "FrameworkTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "NumberOfControls": int,
@@ -635,21 +755,42 @@
 GetBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
+GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBackupVaultNotificationsInputRequestTypeDef = TypedDict(
     "GetBackupVaultNotificationsInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
+GetBackupVaultNotificationsOutputTypeDef = TypedDict(
+    "GetBackupVaultNotificationsOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SNSTopicArn": str,
+        "BackupVaultEvents": List[BackupVaultEventType],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLegalHoldInputRequestTypeDef = TypedDict(
     "GetLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 
@@ -657,34 +798,60 @@
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
+GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "RestoreMetadata": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSupportedResourceTypesOutputTypeDef = TypedDict(
+    "GetSupportedResourceTypesOutputTypeDef",
+    {
+        "ResourceTypes": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LegalHoldTypeDef = TypedDict(
     "LegalHoldTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBackupJobsInputRequestTypeDef = TypedDict(
     "ListBackupJobsInputRequestTypeDef",
     {
@@ -700,23 +867,51 @@
         "ByCompleteAfter": Union[datetime, str],
         "ByCompleteBefore": Union[datetime, str],
         "ByParentJobId": str,
     },
     total=False,
 )
 
+ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
+    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBackupPlanVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupPlanVersionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupPlanVersionsInputRequestTypeDef = TypedDict(
@@ -730,24 +925,53 @@
 
 class ListBackupPlanVersionsInputRequestTypeDef(
     _RequiredListBackupPlanVersionsInputRequestTypeDef,
     _OptionalListBackupPlanVersionsInputRequestTypeDef,
 ):
     pass
 
+ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    {
+        "IncludeDeleted": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBackupPlansInputRequestTypeDef = TypedDict(
     "ListBackupPlansInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IncludeDeleted": bool,
     },
     total=False,
 )
 
+_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
+    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBackupSelectionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupSelectionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupSelectionsInputRequestTypeDef = TypedDict(
@@ -761,23 +985,49 @@
 
 class ListBackupSelectionsInputRequestTypeDef(
     _RequiredListBackupSelectionsInputRequestTypeDef,
     _OptionalListBackupSelectionsInputRequestTypeDef,
 ):
     pass
 
+ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBackupVaultsInputRequestTypeDef = TypedDict(
     "ListBackupVaultsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "ByParentJobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCopyJobsInputRequestTypeDef = TypedDict(
     "ListCopyJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByResourceArn": str,
         "ByState": CopyJobStateType,
@@ -798,23 +1048,39 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLegalHoldsInputRequestTypeDef = TypedDict(
     "ListLegalHoldsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProtectedResourcesInputRequestTypeDef = TypedDict(
     "ListProtectedResourcesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -827,14 +1093,40 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
+_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByParentRecoveryPointArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+):
+    pass
+
 _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
@@ -854,14 +1146,34 @@
 
 class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
     _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
     _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
 ):
     pass
 
+_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "LegalHoldId": str,
+    },
+)
+_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
+    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+):
+    pass
+
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -879,18 +1191,41 @@
 ):
     pass
 
 RecoveryPointMemberTypeDef = TypedDict(
     "RecoveryPointMemberTypeDef",
     {
         "RecoveryPointArn": str,
+        "ResourceArn": str,
+        "ResourceType": str,
+        "BackupVaultName": str,
     },
     total=False,
 )
 
+_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
+    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
@@ -943,14 +1278,28 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
+    {
+        "ByAccountId": str,
+        "ByCreatedBefore": Union[datetime, str],
+        "ByCreatedAfter": Union[datetime, str],
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRestoreJobsInputRequestTypeDef = TypedDict(
     "ListRestoreJobsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ByAccountId": str,
         "ByCreatedBefore": Union[datetime, str],
@@ -998,14 +1347,33 @@
 )
 
 class ListTagsInputRequestTypeDef(
     _RequiredListTagsInputRequestTypeDef, _OptionalListTagsInputRequestTypeDef
 ):
     pass
 
+ListTagsOutputTypeDef = TypedDict(
+    "ListTagsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
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
 _RequiredPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -1058,14 +1426,46 @@
     {
         "S3BucketName": str,
         "S3Keys": List[str],
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
+StartBackupJobOutputTypeDef = TypedDict(
+    "StartBackupJobOutputTypeDef",
+    {
+        "BackupJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartCopyJobOutputTypeDef = TypedDict(
+    "StartCopyJobOutputTypeDef",
+    {
+        "CopyJobId": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1077,36 +1477,53 @@
 )
 
 class StartReportJobInputRequestTypeDef(
     _RequiredStartReportJobInputRequestTypeDef, _OptionalStartReportJobInputRequestTypeDef
 ):
     pass
 
+StartReportJobOutputTypeDef = TypedDict(
+    "StartReportJobOutputTypeDef",
+    {
+        "ReportJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartRestoreJobInputRequestTypeDef = TypedDict(
     "_RequiredStartRestoreJobInputRequestTypeDef",
     {
         "RecoveryPointArn": str,
         "Metadata": Mapping[str, str],
     },
 )
 _OptionalStartRestoreJobInputRequestTypeDef = TypedDict(
     "_OptionalStartRestoreJobInputRequestTypeDef",
     {
         "IamRoleArn": str,
         "IdempotencyToken": str,
         "ResourceType": str,
+        "CopySourceTagsToRestoredResource": bool,
     },
     total=False,
 )
 
 class StartRestoreJobInputRequestTypeDef(
     _RequiredStartRestoreJobInputRequestTypeDef, _OptionalStartRestoreJobInputRequestTypeDef
 ):
     pass
 
+StartRestoreJobOutputTypeDef = TypedDict(
+    "StartRestoreJobOutputTypeDef",
+    {
+        "RestoreJobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopBackupJobInputRequestTypeDef = TypedDict(
     "StopBackupJobInputRequestTypeDef",
     {
         "BackupJobId": str,
     },
 )
 
@@ -1122,14 +1539,24 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeyList": Sequence[str],
     },
 )
 
+UpdateFrameworkOutputTypeDef = TypedDict(
+    "UpdateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "GlobalSettings": Mapping[str, str],
     },
     total=False,
 )
@@ -1139,14 +1566,24 @@
     {
         "ResourceTypeOptInPreference": Mapping[str, bool],
         "ResourceTypeManagementPreference": Mapping[str, bool],
     },
     total=False,
 )
 
+UpdateReportPlanOutputTypeDef = TypedDict(
+    "UpdateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BackupPlansListMemberTypeDef = TypedDict(
     "BackupPlansListMemberTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
@@ -1155,14 +1592,38 @@
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
     },
     total=False,
 )
 
+CreateBackupPlanOutputTypeDef = TypedDict(
+    "CreateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBackupPlanOutputTypeDef = TypedDict(
+    "UpdateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
         "AccountId": str,
         "BackupJobId": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
@@ -1213,14 +1674,55 @@
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
         "ResourceName": str,
     },
     total=False,
 )
 
+DescribeBackupJobOutputTypeDef = TypedDict(
+    "DescribeBackupJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "BackupJobId": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "ResourceArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "State": BackupJobStateType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "ResourceType": str,
+        "BytesTransferred": int,
+        "ExpectedCompletionDate": datetime,
+        "StartBy": datetime,
+        "BackupOptions": Dict[str, str],
+        "BackupType": str,
+        "ParentJobId": str,
+        "IsParent": bool,
+        "NumberOfChildJobs": int,
+        "ChildJobsInState": Dict[BackupJobStateType, int],
+        "ResourceName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupPlanTemplatesOutputTypeDef = TypedDict(
+    "ListBackupPlanTemplatesOutputTypeDef",
+    {
+        "NextToken": str,
+        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
         "DestinationBackupVaultArn": str,
     },
 )
 _OptionalCopyActionTypeDef = TypedDict(
@@ -1300,16 +1802,34 @@
 
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
-RecoveryPointByBackupVaultTypeDef = TypedDict(
-    "RecoveryPointByBackupVaultTypeDef",
+ListBackupSelectionsOutputTypeDef = TypedDict(
+    "ListBackupSelectionsOutputTypeDef",
+    {
+        "NextToken": str,
+        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupVaultsOutputTypeDef = TypedDict(
+    "ListBackupVaultsOutputTypeDef",
+    {
+        "BackupVaultList": List[BackupVaultListMemberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeRecoveryPointOutputTypeDef = TypedDict(
+    "DescribeRecoveryPointOutputTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1320,185 +1840,26 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
+        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
-    },
-    total=False,
-)
-
-ConditionsTypeDef = TypedDict(
-    "ConditionsTypeDef",
-    {
-        "StringEquals": Sequence[ConditionParameterTypeDef],
-        "StringNotEquals": Sequence[ConditionParameterTypeDef],
-        "StringLike": Sequence[ConditionParameterTypeDef],
-        "StringNotLike": Sequence[ConditionParameterTypeDef],
-    },
-    total=False,
-)
-
-_RequiredFrameworkControlTypeDef = TypedDict(
-    "_RequiredFrameworkControlTypeDef",
-    {
-        "ControlName": str,
-    },
-)
-_OptionalFrameworkControlTypeDef = TypedDict(
-    "_OptionalFrameworkControlTypeDef",
-    {
-        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeTypeDef,
-    },
-    total=False,
-)
-
-class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
-    pass
-
-CreateBackupPlanOutputTypeDef = TypedDict(
-    "CreateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBackupSelectionOutputTypeDef = TypedDict(
-    "CreateBackupSelectionOutputTypeDef",
-    {
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBackupVaultOutputTypeDef = TypedDict(
-    "CreateBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFrameworkOutputTypeDef = TypedDict(
-    "CreateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReportPlanOutputTypeDef = TypedDict(
-    "CreateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBackupPlanOutputTypeDef = TypedDict(
-    "DeleteBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "DeletionDate": datetime,
-        "VersionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupJobOutputTypeDef = TypedDict(
-    "DescribeBackupJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "BackupJobId": str,
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "State": BackupJobStateType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "ResourceType": str,
-        "BytesTransferred": int,
-        "ExpectedCompletionDate": datetime,
-        "StartBy": datetime,
-        "BackupOptions": Dict[str, str],
-        "BackupType": str,
-        "ParentJobId": str,
-        "IsParent": bool,
-        "NumberOfChildJobs": int,
-        "ChildJobsInState": Dict[BackupJobStateType, int],
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupVaultOutputTypeDef = TypedDict(
-    "DescribeBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "EncryptionKeyArn": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "NumberOfRecoveryPoints": int,
-        "Locked": bool,
-        "MinRetentionDays": int,
-        "MaxRetentionDays": int,
-        "LockDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGlobalSettingsOutputTypeDef = TypedDict(
-    "DescribeGlobalSettingsOutputTypeDef",
-    {
-        "GlobalSettings": Dict[str, str],
-        "LastUpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeProtectedResourceOutputTypeDef = TypedDict(
-    "DescribeProtectedResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceType": str,
-        "LastBackupTime": datetime,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeRecoveryPointOutputTypeDef = TypedDict(
-    "DescribeRecoveryPointOutputTypeDef",
+RecoveryPointByBackupVaultTypeDef = TypedDict(
+    "RecoveryPointByBackupVaultTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1509,222 +1870,62 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
-        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRegionSettingsOutputTypeDef = TypedDict(
-    "DescribeRegionSettingsOutputTypeDef",
-    {
-        "ResourceTypeOptInPreference": Dict[str, bool],
-        "ResourceTypeManagementPreference": Dict[str, bool],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRestoreJobOutputTypeDef = TypedDict(
-    "DescribeRestoreJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "RestoreJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "Status": RestoreJobStatusType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "ExpectedCompletionTimeMinutes": int,
-        "CreatedResourceArn": str,
-        "ResourceType": str,
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
-ExportBackupPlanTemplateOutputTypeDef = TypedDict(
-    "ExportBackupPlanTemplateOutputTypeDef",
-    {
-        "BackupPlanTemplateJson": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBackupVaultNotificationsOutputTypeDef = TypedDict(
-    "GetBackupVaultNotificationsOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "SNSTopicArn": str,
-        "BackupVaultEvents": List[BackupVaultEventType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "RestoreMetadata": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSupportedResourceTypesOutputTypeDef = TypedDict(
-    "GetSupportedResourceTypesOutputTypeDef",
-    {
-        "ResourceTypes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupPlanTemplatesOutputTypeDef = TypedDict(
-    "ListBackupPlanTemplatesOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupSelectionsOutputTypeDef = TypedDict(
-    "ListBackupSelectionsOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupVaultsOutputTypeDef = TypedDict(
-    "ListBackupVaultsOutputTypeDef",
-    {
-        "BackupVaultList": List[BackupVaultListMemberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsOutputTypeDef = TypedDict(
-    "ListTagsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBackupJobOutputTypeDef = TypedDict(
-    "StartBackupJobOutputTypeDef",
-    {
-        "BackupJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartCopyJobOutputTypeDef = TypedDict(
-    "StartCopyJobOutputTypeDef",
-    {
-        "CopyJobId": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartReportJobOutputTypeDef = TypedDict(
-    "StartReportJobOutputTypeDef",
-    {
-        "ReportJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRestoreJobOutputTypeDef = TypedDict(
-    "StartRestoreJobOutputTypeDef",
-    {
-        "RestoreJobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Lifecycle": LifecycleTypeDef,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateBackupPlanOutputTypeDef = TypedDict(
-    "UpdateBackupPlanOutputTypeDef",
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
     {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StringEquals": Sequence[ConditionParameterTypeDef],
+        "StringNotEquals": Sequence[ConditionParameterTypeDef],
+        "StringLike": Sequence[ConditionParameterTypeDef],
+        "StringNotLike": Sequence[ConditionParameterTypeDef],
     },
+    total=False,
 )
 
-UpdateFrameworkOutputTypeDef = TypedDict(
-    "UpdateFrameworkOutputTypeDef",
+_RequiredFrameworkControlTypeDef = TypedDict(
+    "_RequiredFrameworkControlTypeDef",
     {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ControlName": str,
     },
 )
-
-UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+_OptionalFrameworkControlTypeDef = TypedDict(
+    "_OptionalFrameworkControlTypeDef",
     {
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "Lifecycle": LifecycleTypeDef,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeTypeDef,
     },
+    total=False,
 )
 
-UpdateReportPlanOutputTypeDef = TypedDict(
-    "UpdateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
+    pass
 
 _RequiredCreateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
         "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
         "ReportSetting": ReportSettingTypeDef,
@@ -1794,257 +1995,60 @@
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
         "Frameworks": List[FrameworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLegalHoldsOutputTypeDef = TypedDict(
     "ListLegalHoldsOutputTypeDef",
     {
         "NextToken": str,
         "LegalHolds": List[LegalHoldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
-    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-):
-    pass
-
-ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    {
-        "IncludeDeleted": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
-    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-):
-    pass
-
-ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-):
-    pass
-
-_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "LegalHoldId": str,
-    },
-)
-_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
-    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-):
-    pass
-
-_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
-    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-):
-    pass
-
-ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    {
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
     {
         "Results": List[ProtectedResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryPointsByLegalHoldOutputTypeDef = TypedDict(
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     {
         "RecoveryPoints": List[RecoveryPointMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecoveryPointsByResourceOutputTypeDef = TypedDict(
     "ListRecoveryPointsByResourceOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRestoreJobsOutputTypeDef = TypedDict(
     "ListRestoreJobsOutputTypeDef",
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
@@ -2060,50 +2064,50 @@
 )
 
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupPlansOutputTypeDef = TypedDict(
     "ListBackupPlansOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlansList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupJobsOutputTypeDef = TypedDict(
     "ListBackupJobsOutputTypeDef",
     {
         "BackupJobs": List[BackupJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCopyJobOutputTypeDef = TypedDict(
     "DescribeCopyJobOutputTypeDef",
     {
         "CopyJob": CopyJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCopyJobsOutputTypeDef = TypedDict(
     "ListCopyJobsOutputTypeDef",
     {
         "CopyJobs": List[CopyJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupRuleInputTypeDef = TypedDict(
     "_RequiredBackupRuleInputTypeDef",
     {
         "RuleName": str,
@@ -2153,15 +2157,15 @@
     pass
 
 ListRecoveryPointsByBackupVaultOutputTypeDef = TypedDict(
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupSelectionTypeDef = TypedDict(
     "_RequiredBackupSelectionTypeDef",
     {
         "SelectionName": str,
@@ -2211,15 +2215,15 @@
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "FrameworkControls": List[FrameworkControlTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
@@ -2240,24 +2244,24 @@
 ):
     pass
 
 DescribeReportPlanOutputTypeDef = TypedDict(
     "DescribeReportPlanOutputTypeDef",
     {
         "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReportPlansOutputTypeDef = TypedDict(
     "ListReportPlansOutputTypeDef",
     {
         "ReportPlans": List[ReportPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
         "Title": str,
@@ -2285,15 +2289,15 @@
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLegalHoldOutputTypeDef = TypedDict(
     "GetLegalHoldOutputTypeDef",
     {
         "Title": str,
@@ -2302,32 +2306,32 @@
         "CancelDescription": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReportJobsOutputTypeDef = TypedDict(
     "ListReportJobsOutputTypeDef",
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
@@ -2388,15 +2392,15 @@
     "GetBackupSelectionOutputTypeDef",
     {
         "BackupSelection": BackupSelectionTypeDef,
         "SelectionId": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "CreatorRequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
@@ -2424,23 +2428,23 @@
     },
 )
 
 GetBackupPlanFromJSONOutputTypeDef = TypedDict(
     "GetBackupPlanFromJSONOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBackupPlanFromTemplateOutputTypeDef = TypedDict(
     "GetBackupPlanFromTemplateOutputTypeDef",
     {
         "BackupPlanDocument": BackupPlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBackupPlanOutputTypeDef = TypedDict(
     "GetBackupPlanOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
@@ -2448,10 +2452,10 @@
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
         "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/PKG-INFO` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.26.67
-Summary: Type annotations for boto3.Backup 1.26.67 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Backup 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-backup"></a>
 
 # mypy-boto3-backup
 
 [![PyPI - mypy-boto3-backup](https://img.shields.io/pypi/v/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.26.67](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,143 +390,143 @@
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
     ConditionParameterTypeDef,
     ControlInputParameterTypeDef,
     ControlScopeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultInputRequestTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
+    CreateReportPlanOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
+    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
+    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
+    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    PaginatorConfigTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
     ListBackupJobsInputRequestTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
     ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
     ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
     ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
+    ListTagsOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDestinationTypeDef,
+    ResponseMetadataTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
+    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
+    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
+    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    RecoveryPointByBackupVaultTypeDef,
-    ConditionsTypeDef,
-    FrameworkControlTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    CreateBackupSelectionOutputTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
-    CreateReportPlanOutputTypeDef,
-    DeleteBackupPlanOutputTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    DescribeBackupVaultOutputTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
-    DescribeRestoreJobOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     ListBackupSelectionsOutputTypeDef,
     ListBackupVaultsOutputTypeDef,
-    ListTagsOutputTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
-    StartReportJobOutputTypeDef,
-    StartRestoreJobOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
-    UpdateFrameworkOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    RecoveryPointByBackupVaultTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
-    UpdateReportPlanOutputTypeDef,
+    ConditionsTypeDef,
+    FrameworkControlTypeDef,
     CreateReportPlanInputRequestTypeDef,
     ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
@@ -566,42 +566,42 @@
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

### Comparing `mypy-boto3-backup-1.26.67/mypy_boto3_backup.egg-info/SOURCES.txt` & `mypy-boto3-backup-1.27.0/mypy_boto3_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.26.67/setup.py` & `mypy-boto3-backup-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-backup.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup",
-    version="1.26.67",
+    version="1.27.0",
     packages=["mypy_boto3_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Backup 1.26.67 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Backup 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/",
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


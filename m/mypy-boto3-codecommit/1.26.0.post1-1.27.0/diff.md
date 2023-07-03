# Comparing `tmp/mypy-boto3-codecommit-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codecommit-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecommit-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:14 2022, max compression
+gzip compressed data, was "mypy-boto3-codecommit-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-codecommit-1.26.0.post1.tar` & `mypy-boto3-codecommit-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.008818 mypy-boto3-codecommit-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22886 2022-11-01 21:43:14.008818 mypy-boto3-codecommit-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21433 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.000818 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    71776 2022-11-01 21:31:49.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    71685 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10145 2022-11-01 21:31:49.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10143 2022-11-01 21:31:49.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9450 2022-11-01 21:31:49.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-11-01 21:31:49.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    78709 2022-11-01 21:31:51.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    78614 2022-11-01 21:31:50.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.008818 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22886 2022-11-01 21:43:13.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-01 21:43:13.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:13.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:13.000000 mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:14.008818 mypy-boto3-codecommit-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-01 21:31:48.000000 mypy-boto3-codecommit-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.854986 mypy-boto3-codecommit-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-07-03 19:50:31.854986 mypy-boto3-codecommit-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.854986 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71776 2023-07-03 19:34:15.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71685 2023-07-03 19:34:15.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-03 19:34:15.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-03 19:34:15.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-03 19:34:15.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-03 19:34:15.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    78905 2023-07-03 19:34:17.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78810 2023-07-03 19:34:16.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:14.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.854986 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-07-03 19:50:31.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:31.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:31.000000 mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.854986 mypy-boto3-codecommit-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:34:13.000000 mypy-boto3-codecommit-1.27.0/setup.py
```

### Comparing `mypy-boto3-codecommit-1.26.0.post1/LICENSE` & `mypy-boto3-codecommit-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/PKG-INFO` & `mypy-boto3-codecommit-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeCommit 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeCommit 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
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
 
 <a id="mypy-boto3-codecommit"></a>
 
 # mypy-boto3-codecommit
 
 [![PyPI - mypy-boto3-codecommit](https://img.shields.io/pypi/v/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecommit?color=blue)](https://pypistats.org/packages/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,15 +368,14 @@
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
@@ -395,116 +395,124 @@
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
+    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
+    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
+    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
+    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
+    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
+    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
     RepositoryTriggerTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
+    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
-    ApprovalRuleTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
-    DeleteFileOutputTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
-    DeleteRepositoryOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
-    GetBlobOutputTypeDef,
-    GetFileOutputTypeDef,
-    GetMergeCommitOutputTypeDef,
-    GetMergeOptionsOutputTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsOutputTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
-    PutFileOutputTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
+    ApprovalRuleTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
@@ -519,21 +527,14 @@
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     PutRepositoryTriggersInputRequestTypeDef,
     TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
@@ -581,42 +582,42 @@
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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/README.md` & `mypy-boto3-codecommit-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codecommit"></a>
 
 # mypy-boto3-codecommit
 
 [![PyPI - mypy-boto3-codecommit](https://img.shields.io/pypi/v/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecommit?color=blue)](https://pypistats.org/packages/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,15 +336,14 @@
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
@@ -364,116 +363,124 @@
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
+    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
+    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
+    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
+    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
+    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
+    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
     RepositoryTriggerTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
+    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
-    ApprovalRuleTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
-    DeleteFileOutputTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
-    DeleteRepositoryOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
-    GetBlobOutputTypeDef,
-    GetFileOutputTypeDef,
-    GetMergeCommitOutputTypeDef,
-    GetMergeOptionsOutputTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsOutputTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
-    PutFileOutputTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
+    ApprovalRuleTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
@@ -488,21 +495,14 @@
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     PutRepositoryTriggersInputRequestTypeDef,
     TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
@@ -550,42 +550,42 @@
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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/__init__.py` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/__init__.pyi` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/__main__.py` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCommit 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CodeCommit 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/client.py` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/client.pyi` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/literals.py` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,23 +98,25 @@
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
@@ -124,30 +126,35 @@
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
@@ -173,14 +180,15 @@
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
@@ -225,51 +233,57 @@
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
@@ -282,14 +296,15 @@
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
@@ -301,28 +316,35 @@
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
@@ -331,14 +353,15 @@
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
@@ -349,55 +372,64 @@
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
@@ -431,23 +463,26 @@
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
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/literals.pyi` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,23 +96,25 @@
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
@@ -122,30 +124,35 @@
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
@@ -171,14 +178,15 @@
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
@@ -223,51 +231,57 @@
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
@@ -280,14 +294,15 @@
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
@@ -299,28 +314,35 @@
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
@@ -329,14 +351,15 @@
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
@@ -347,55 +370,64 @@
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
@@ -429,23 +461,26 @@
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
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/paginator.py` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,153 +58,144 @@
     "GetCommentsForPullRequestPaginator",
     "GetDifferencesPaginator",
     "ListBranchesPaginator",
     "ListPullRequestsPaginator",
     "ListRepositoriesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribePullRequestEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
-
 class GetCommentsForComparedCommitPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
-
 class GetCommentsForPullRequestPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
-
 class GetDifferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
         """
 
-
 class ListBranchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
     """
 
     def paginate(
-        self, *, repositoryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, repositoryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBranchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
         """
 
-
 class ListPullRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
         """
 
-
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/paginator.pyi` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,144 +58,153 @@
     "GetCommentsForPullRequestPaginator",
     "GetDifferencesPaginator",
     "ListBranchesPaginator",
     "ListPullRequestsPaginator",
     "ListRepositoriesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribePullRequestEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
+
 class GetCommentsForComparedCommitPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
+
 class GetCommentsForPullRequestPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
     """
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
+
 class GetDifferencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#getdifferencespaginator)
         """
 
+
 class ListBranchesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
     """
 
     def paginate(
-        self, *, repositoryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, repositoryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBranchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listbranchespaginator)
         """
 
+
 class ListPullRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listpullrequestspaginator)
         """
 
+
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/type_defs.py` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
     "AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDescribeMergeConflictsErrorTypeDef",
     "BatchDescribeMergeConflictsInputRequestTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
@@ -75,116 +74,124 @@
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
+    "CreateUnreferencedMergeCommitOutputTypeDef",
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
+    "DeleteApprovalRuleTemplateOutputTypeDef",
     "DeleteBranchInputRequestTypeDef",
     "DeleteCommentContentInputRequestTypeDef",
     "DeleteFileInputRequestTypeDef",
+    "DeleteFileOutputTypeDef",
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
+    "DeletePullRequestApprovalRuleOutputTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
+    "DeleteRepositoryOutputTypeDef",
     "DescribeMergeConflictsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     "DescribePullRequestEventsInputRequestTypeDef",
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     "EvaluationTypeDef",
     "FileTypeDef",
     "FolderTypeDef",
     "GetApprovalRuleTemplateInputRequestTypeDef",
     "GetBlobInputRequestTypeDef",
+    "GetBlobOutputTypeDef",
     "GetBranchInputRequestTypeDef",
     "GetCommentInputRequestTypeDef",
     "GetCommentReactionsInputRequestTypeDef",
+    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForComparedCommitInputRequestTypeDef",
+    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetCommentsForPullRequestInputRequestTypeDef",
     "GetCommitInputRequestTypeDef",
+    "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "GetDifferencesInputRequestTypeDef",
     "GetFileInputRequestTypeDef",
+    "GetFileOutputTypeDef",
     "GetFolderInputRequestTypeDef",
     "SubModuleTypeDef",
     "SymbolicLinkTypeDef",
     "GetMergeCommitInputRequestTypeDef",
+    "GetMergeCommitOutputTypeDef",
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
+    "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
+    "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
     "RepositoryTriggerTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
+    "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
+    "ListBranchesOutputTypeDef",
+    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListPullRequestsInputRequestTypeDef",
+    "ListPullRequestsOutputTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
+    "MergeBranchesByFastForwardOutputTypeDef",
+    "MergeBranchesBySquashOutputTypeDef",
+    "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "PutFileInputRequestTypeDef",
+    "PutFileOutputTypeDef",
+    "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
     "UpdatePullRequestApprovalRuleContentInputRequestTypeDef",
     "UpdatePullRequestApprovalStateInputRequestTypeDef",
     "UpdatePullRequestDescriptionInputRequestTypeDef",
     "UpdatePullRequestStatusInputRequestTypeDef",
     "UpdatePullRequestTitleInputRequestTypeDef",
     "UpdateRepositoryDescriptionInputRequestTypeDef",
     "UpdateRepositoryNameInputRequestTypeDef",
-    "ApprovalRuleTypeDef",
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "CreateApprovalRuleTemplateOutputTypeDef",
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    "DeleteFileOutputTypeDef",
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    "DeleteRepositoryOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApprovalRuleTemplateOutputTypeDef",
-    "GetBlobOutputTypeDef",
-    "GetFileOutputTypeDef",
-    "GetMergeCommitOutputTypeDef",
-    "GetMergeOptionsOutputTypeDef",
-    "GetPullRequestApprovalStatesOutputTypeDef",
-    "GetPullRequestOverrideStateOutputTypeDef",
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    "ListBranchesOutputTypeDef",
-    "ListPullRequestsOutputTypeDef",
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "MergeBranchesByFastForwardOutputTypeDef",
-    "MergeBranchesBySquashOutputTypeDef",
-    "MergeBranchesByThreeWayOutputTypeDef",
-    "PutFileOutputTypeDef",
-    "PutRepositoryTriggersOutputTypeDef",
     "UpdateApprovalRuleTemplateContentOutputTypeDef",
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
+    "ApprovalRuleTypeDef",
+    "GetPullRequestApprovalStatesOutputTypeDef",
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
@@ -199,21 +206,14 @@
     "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
     "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
-    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    "GetDifferencesInputGetDifferencesPaginateTypeDef",
-    "ListBranchesInputListBranchesPaginateTypeDef",
-    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
     "PutRepositoryTriggersInputRequestTypeDef",
     "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
@@ -336,25 +336,14 @@
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryNames": Sequence[str],
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
 BatchDescribeMergeConflictsErrorTypeDef = TypedDict(
     "BatchDescribeMergeConflictsErrorTypeDef",
     {
         "filePath": str,
         "exceptionName": str,
         "message": str,
     },
@@ -682,21 +671,38 @@
 
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
 
+CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 
+DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    {
+        "approvalRuleTemplateId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBranchInputRequestTypeDef = TypedDict(
     "DeleteBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
 )
@@ -731,29 +737,56 @@
 
 class DeleteFileInputRequestTypeDef(
     _RequiredDeleteFileInputRequestTypeDef, _OptionalDeleteFileInputRequestTypeDef
 ):
     pass
 
 
+DeleteFileOutputTypeDef = TypedDict(
+    "DeleteFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "filePath": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePullRequestApprovalRuleInputRequestTypeDef = TypedDict(
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
     {
         "pullRequestId": str,
         "approvalRuleName": str,
     },
 )
 
+DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    {
+        "approvalRuleId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRepositoryInputRequestTypeDef = TypedDict(
     "DeleteRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
+    {
+        "repositoryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -775,24 +808,38 @@
 class DescribeMergeConflictsInputRequestTypeDef(
     _RequiredDescribeMergeConflictsInputRequestTypeDef,
     _OptionalDescribeMergeConflictsInputRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "pullRequestId": str,
+    },
+)
+_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
+    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribePullRequestEventsInputRequestTypeDef = TypedDict(
     "_RequiredDescribePullRequestEventsInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalDescribePullRequestEventsInputRequestTypeDef = TypedDict(
@@ -818,14 +865,21 @@
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluatePullRequestApprovalRulesInputRequestTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -873,14 +927,22 @@
     "GetBlobInputRequestTypeDef",
     {
         "repositoryName": str,
         "blobId": str,
     },
 )
 
+GetBlobOutputTypeDef = TypedDict(
+    "GetBlobOutputTypeDef",
+    {
+        "content": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBranchInputRequestTypeDef = TypedDict(
     "GetBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
     total=False,
@@ -912,14 +974,38 @@
 
 class GetCommentReactionsInputRequestTypeDef(
     _RequiredGetCommentReactionsInputRequestTypeDef, _OptionalGetCommentReactionsInputRequestTypeDef
 ):
     pass
 
 
+_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitId": str,
+    },
+)
+_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "beforeCommitId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
+    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetCommentsForComparedCommitInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitId": str,
     },
 )
@@ -937,14 +1023,39 @@
 class GetCommentsForComparedCommitInputRequestTypeDef(
     _RequiredGetCommentsForComparedCommitInputRequestTypeDef,
     _OptionalGetCommentsForComparedCommitInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "pullRequestId": str,
+    },
+)
+_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
+    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
@@ -971,14 +1082,40 @@
     "GetCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "commitId": str,
     },
 )
 
+_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitSpecifier": str,
+    },
+)
+_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "beforeCommitSpecifier": str,
+        "beforePath": str,
+        "afterPath": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetDifferencesInputGetDifferencesPaginateTypeDef(
+    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
+    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetDifferencesInputRequestTypeDef = TypedDict(
     "_RequiredGetDifferencesInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitSpecifier": str,
     },
 )
@@ -1019,14 +1156,27 @@
 
 class GetFileInputRequestTypeDef(
     _RequiredGetFileInputRequestTypeDef, _OptionalGetFileInputRequestTypeDef
 ):
     pass
 
 
+GetFileOutputTypeDef = TypedDict(
+    "GetFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "filePath": str,
+        "fileMode": FileModeTypeEnumType,
+        "fileSize": int,
+        "fileContent": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetFolderInputRequestTypeDef = TypedDict(
     "_RequiredGetFolderInputRequestTypeDef",
     {
         "repositoryName": str,
         "folderPath": str,
     },
 )
@@ -1086,14 +1236,25 @@
 
 class GetMergeCommitInputRequestTypeDef(
     _RequiredGetMergeCommitInputRequestTypeDef, _OptionalGetMergeCommitInputRequestTypeDef
 ):
     pass
 
 
+GetMergeCommitOutputTypeDef = TypedDict(
+    "GetMergeCommitOutputTypeDef",
+    {
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "mergedCommitId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredGetMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -1137,14 +1298,25 @@
 
 class GetMergeOptionsInputRequestTypeDef(
     _RequiredGetMergeOptionsInputRequestTypeDef, _OptionalGetMergeOptionsInputRequestTypeDef
 ):
     pass
 
 
+GetMergeOptionsOutputTypeDef = TypedDict(
+    "GetMergeOptionsOutputTypeDef",
+    {
+        "mergeOptions": List[MergeOptionTypeEnumType],
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPullRequestApprovalStatesInputRequestTypeDef = TypedDict(
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -1160,14 +1332,23 @@
     "GetPullRequestOverrideStateInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
 
+GetPullRequestOverrideStateOutputTypeDef = TypedDict(
+    "GetPullRequestOverrideStateOutputTypeDef",
+    {
+        "overridden": bool,
+        "overrider": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRepositoryInputRequestTypeDef = TypedDict(
     "GetRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
@@ -1207,14 +1388,23 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
@@ -1230,14 +1420,45 @@
 class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(
     _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
 ):
     pass
 
 
+ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBranchesInputListBranchesPaginateTypeDef(
+    _RequiredListBranchesInputListBranchesPaginateTypeDef,
+    _OptionalListBranchesInputListBranchesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBranchesInputRequestTypeDef = TypedDict(
     "_RequiredListBranchesInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListBranchesInputRequestTypeDef = TypedDict(
@@ -1251,14 +1472,47 @@
 
 class ListBranchesInputRequestTypeDef(
     _RequiredListBranchesInputRequestTypeDef, _OptionalListBranchesInputRequestTypeDef
 ):
     pass
 
 
+ListBranchesOutputTypeDef = TypedDict(
+    "ListBranchesOutputTypeDef",
+    {
+        "branches": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "authorArn": str,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPullRequestsInputListPullRequestsPaginateTypeDef(
+    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
+    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPullRequestsInputRequestTypeDef = TypedDict(
     "_RequiredListPullRequestsInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListPullRequestsInputRequestTypeDef = TypedDict(
@@ -1275,14 +1529,23 @@
 
 class ListPullRequestsInputRequestTypeDef(
     _RequiredListPullRequestsInputRequestTypeDef, _OptionalListPullRequestsInputRequestTypeDef
 ):
     pass
 
 
+ListPullRequestsOutputTypeDef = TypedDict(
+    "ListPullRequestsOutputTypeDef",
+    {
+        "pullRequestIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
@@ -1298,14 +1561,33 @@
 class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(
     _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
 ):
     pass
 
 
+ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    {
+        "repositoryNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "sortBy": SortByEnumType,
+        "order": OrderEnumType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "nextToken": str,
         "sortBy": SortByEnumType,
         "order": OrderEnumType,
     },
@@ -1338,14 +1620,23 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1362,14 +1653,41 @@
 class MergeBranchesByFastForwardInputRequestTypeDef(
     _RequiredMergeBranchesByFastForwardInputRequestTypeDef,
     _OptionalMergeBranchesByFastForwardInputRequestTypeDef,
 ):
     pass
 
 
+MergeBranchesByFastForwardOutputTypeDef = TypedDict(
+    "MergeBranchesByFastForwardOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+MergeBranchesBySquashOutputTypeDef = TypedDict(
+    "MergeBranchesBySquashOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+MergeBranchesByThreeWayOutputTypeDef = TypedDict(
+    "MergeBranchesByThreeWayOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MergeHunkDetailTypeDef = TypedDict(
     "MergeHunkDetailTypeDef",
     {
         "startLine": int,
         "endLine": int,
         "hunkContent": str,
     },
@@ -1415,14 +1733,24 @@
     {
         "pullRequestId": str,
         "revisionId": str,
         "overrideStatus": OverrideStatusType,
     },
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
 _RequiredPostCommentReplyInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentReplyInputRequestTypeDef",
     {
         "inReplyTo": str,
         "content": str,
     },
 )
@@ -1524,14 +1852,32 @@
 
 class PutFileInputRequestTypeDef(
     _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
 ):
     pass
 
 
+PutFileOutputTypeDef = TypedDict(
+    "PutFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutRepositoryTriggersOutputTypeDef = TypedDict(
+    "PutRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReactionValueFormatsTypeDef = TypedDict(
     "ReactionValueFormatsTypeDef",
     {
         "emoji": str,
         "shortCode": str,
         "unicode": str,
     },
@@ -1543,14 +1889,25 @@
     {
         "trigger": str,
         "failureMessage": str,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1701,319 +2058,117 @@
     "UpdateRepositoryNameInputRequestTypeDef",
     {
         "oldName": str,
         "newName": str,
     },
 )
 
-ApprovalRuleTypeDef = TypedDict(
-    "ApprovalRuleTypeDef",
-    {
-        "approvalRuleId": str,
-        "approvalRuleName": str,
-        "approvalRuleContent": str,
-        "ruleContentSha256": str,
-        "lastModifiedDate": datetime,
-        "creationDate": datetime,
-        "lastModifiedUser": str,
-        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
-    },
-    total=False,
-)
-
-BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
-    {
-        "associatedRepositoryNames": List[str],
-        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateApprovalRuleTemplateOutputTypeDef = TypedDict(
     "CreateApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    {
-        "approvalRuleTemplateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFileOutputTypeDef = TypedDict(
-    "DeleteFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "filePath": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    {
-        "approvalRuleId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
-    {
-        "repositoryId": str,
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
 
 GetApprovalRuleTemplateOutputTypeDef = TypedDict(
     "GetApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBlobOutputTypeDef = TypedDict(
-    "GetBlobOutputTypeDef",
+UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateContentOutputTypeDef",
     {
-        "content": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetFileOutputTypeDef = TypedDict(
-    "GetFileOutputTypeDef",
+UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     {
-        "commitId": str,
-        "blobId": str,
-        "filePath": str,
-        "fileMode": FileModeTypeEnumType,
-        "fileSize": int,
-        "fileContent": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetMergeCommitOutputTypeDef = TypedDict(
-    "GetMergeCommitOutputTypeDef",
+UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateNameOutputTypeDef",
     {
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "mergedCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetMergeOptionsOutputTypeDef = TypedDict(
-    "GetMergeOptionsOutputTypeDef",
+ApprovalRuleTypeDef = TypedDict(
+    "ApprovalRuleTypeDef",
     {
-        "mergeOptions": List[MergeOptionTypeEnumType],
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleId": str,
+        "approvalRuleName": str,
+        "approvalRuleContent": str,
+        "ruleContentSha256": str,
+        "lastModifiedDate": datetime,
+        "creationDate": datetime,
+        "lastModifiedUser": str,
+        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
     },
+    total=False,
 )
 
 GetPullRequestApprovalStatesOutputTypeDef = TypedDict(
     "GetPullRequestApprovalStatesOutputTypeDef",
     {
         "approvals": List[ApprovalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPullRequestOverrideStateOutputTypeDef = TypedDict(
-    "GetPullRequestOverrideStateOutputTypeDef",
-    {
-        "overridden": bool,
-        "overrider": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBranchesOutputTypeDef = TypedDict(
-    "ListBranchesOutputTypeDef",
-    {
-        "branches": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPullRequestsOutputTypeDef = TypedDict(
-    "ListPullRequestsOutputTypeDef",
-    {
-        "pullRequestIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    {
-        "repositoryNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeBranchesByFastForwardOutputTypeDef = TypedDict(
-    "MergeBranchesByFastForwardOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MergeBranchesBySquashOutputTypeDef = TypedDict(
-    "MergeBranchesBySquashOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeBranchesByThreeWayOutputTypeDef = TypedDict(
-    "MergeBranchesByThreeWayOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutFileOutputTypeDef = TypedDict(
-    "PutFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRepositoryTriggersOutputTypeDef = TypedDict(
-    "PutRepositoryTriggersOutputTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateContentOutputTypeDef",
-    {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
-    {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "associatedRepositoryNames": List[str],
+        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef = TypedDict(
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     {
         "disassociatedRepositoryNames": List[str],
         "errors": List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetRepositoriesOutputTypeDef = TypedDict(
     "BatchGetRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryMetadataTypeDef],
         "repositoriesNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DifferenceTypeDef = TypedDict(
     "DifferenceTypeDef",
     {
         "beforeBlob": BlobMetadataTypeDef,
@@ -2023,55 +2178,55 @@
     total=False,
 )
 
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBranchOutputTypeDef = TypedDict(
     "GetBranchOutputTypeDef",
     {
         "branch": BranchInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCommentContentOutputTypeDef = TypedDict(
     "DeleteCommentContentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommentOutputTypeDef = TypedDict(
     "GetCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PostCommentReplyOutputTypeDef = TypedDict(
     "PostCommentReplyOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCommentOutputTypeDef = TypedDict(
     "UpdateCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommentsForComparedCommitTypeDef = TypedDict(
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
@@ -2132,15 +2287,15 @@
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
@@ -2174,15 +2329,15 @@
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
     {
         "commitId": str,
@@ -2227,15 +2382,15 @@
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
         "filesDeleted": List[FileMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePullRequestInputRequestTypeDef = TypedDict(
     "_RequiredCreatePullRequestInputRequestTypeDef",
     {
         "title": str,
@@ -2254,197 +2409,42 @@
 
 class CreatePullRequestInputRequestTypeDef(
     _RequiredCreatePullRequestInputRequestTypeDef, _OptionalCreatePullRequestInputRequestTypeDef
 ):
     pass
 
 
-_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
-    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-    },
-)
-_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "beforeCommitId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
-    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
-    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitSpecifier": str,
-    },
-)
-_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "beforeCommitSpecifier": str,
-        "beforePath": str,
-        "afterPath": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetDifferencesInputGetDifferencesPaginateTypeDef(
-    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
-    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBranchesInputListBranchesPaginateTypeDef(
-    _RequiredListBranchesInputListBranchesPaginateTypeDef,
-    _OptionalListBranchesInputListBranchesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "authorArn": str,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPullRequestsInputListPullRequestsPaginateTypeDef(
-    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
-    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
-):
-    pass
-
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "sortBy": SortByEnumType,
-        "order": OrderEnumType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     {
         "evaluation": EvaluationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFolderOutputTypeDef = TypedDict(
     "GetFolderOutputTypeDef",
     {
         "commitId": str,
         "folderPath": str,
         "treeId": str,
         "subFolders": List[FolderTypeDef],
         "files": List[FileTypeDef],
         "symbolicLinks": List[SymbolicLinkTypeDef],
         "subModules": List[SubModuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
         "triggers": List[RepositoryTriggerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRepositoryTriggersInputRequestTypeDef = TypedDict(
     "PutRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2461,15 +2461,15 @@
 )
 
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryNameIdPairTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
@@ -2536,88 +2536,88 @@
 )
 
 TestRepositoryTriggersOutputTypeDef = TypedDict(
     "TestRepositoryTriggersOutputTypeDef",
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestApprovalRuleContentOutputTypeDef = TypedDict(
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDifferencesOutputTypeDef = TypedDict(
     "GetDifferencesOutputTypeDef",
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommentsForPullRequestOutputTypeDef = TypedDict(
     "GetCommentsForPullRequestOutputTypeDef",
     {
         "commentsForPullRequestData": List[CommentsForPullRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetCommitsOutputTypeDef = TypedDict(
     "BatchGetCommitsOutputTypeDef",
     {
         "commits": List[CommitTypeDef],
         "errors": List[BatchGetCommitsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommitOutputTypeDef = TypedDict(
     "GetCommitOutputTypeDef",
     {
         "commit": CommitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMergeConflictsOutputTypeDef = TypedDict(
     "GetMergeConflictsOutputTypeDef",
     {
         "mergeable": bool,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2784,29 +2784,33 @@
     {
         "conflictMetadata": ConflictMetadataTypeDef,
         "mergeHunks": List[MergeHunkTypeDef],
         "nextToken": str,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PullRequestEventTypeDef = TypedDict(
     "PullRequestEventTypeDef",
     {
         "pullRequestId": str,
         "eventDate": datetime,
         "pullRequestEventType": PullRequestEventTypeType,
         "actorArn": str,
         "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
         "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
-        "pullRequestSourceReferenceUpdatedEventMetadata": PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
-        "pullRequestMergedStateChangedEventMetadata": PullRequestMergedStateChangedEventMetadataTypeDef,
+        "pullRequestSourceReferenceUpdatedEventMetadata": (
+            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
+        ),
+        "pullRequestMergedStateChangedEventMetadata": (
+            PullRequestMergedStateChangedEventMetadataTypeDef
+        ),
         "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
         "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
         "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
     },
     total=False,
 )
 
@@ -2858,96 +2862,96 @@
 
 
 GetCommentReactionsOutputTypeDef = TypedDict(
     "GetCommentReactionsOutputTypeDef",
     {
         "reactionsForComment": List[ReactionForCommentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePullRequestEventsOutputTypeDef = TypedDict(
     "DescribePullRequestEventsOutputTypeDef",
     {
         "pullRequestEvents": List[PullRequestEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePullRequestOutputTypeDef = TypedDict(
     "CreatePullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPullRequestOutputTypeDef = TypedDict(
     "GetPullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergePullRequestByFastForwardOutputTypeDef = TypedDict(
     "MergePullRequestByFastForwardOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergePullRequestBySquashOutputTypeDef = TypedDict(
     "MergePullRequestBySquashOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergePullRequestByThreeWayOutputTypeDef = TypedDict(
     "MergePullRequestByThreeWayOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestDescriptionOutputTypeDef = TypedDict(
     "UpdatePullRequestDescriptionOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestStatusOutputTypeDef = TypedDict(
     "UpdatePullRequestStatusOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestTitleOutputTypeDef = TypedDict(
     "UpdatePullRequestTitleOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit/type_defs.pyi` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
     "AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDescribeMergeConflictsErrorTypeDef",
     "BatchDescribeMergeConflictsInputRequestTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
@@ -74,116 +73,124 @@
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
+    "CreateUnreferencedMergeCommitOutputTypeDef",
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
+    "DeleteApprovalRuleTemplateOutputTypeDef",
     "DeleteBranchInputRequestTypeDef",
     "DeleteCommentContentInputRequestTypeDef",
     "DeleteFileInputRequestTypeDef",
+    "DeleteFileOutputTypeDef",
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
+    "DeletePullRequestApprovalRuleOutputTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
+    "DeleteRepositoryOutputTypeDef",
     "DescribeMergeConflictsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     "DescribePullRequestEventsInputRequestTypeDef",
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     "EvaluationTypeDef",
     "FileTypeDef",
     "FolderTypeDef",
     "GetApprovalRuleTemplateInputRequestTypeDef",
     "GetBlobInputRequestTypeDef",
+    "GetBlobOutputTypeDef",
     "GetBranchInputRequestTypeDef",
     "GetCommentInputRequestTypeDef",
     "GetCommentReactionsInputRequestTypeDef",
+    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForComparedCommitInputRequestTypeDef",
+    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetCommentsForPullRequestInputRequestTypeDef",
     "GetCommitInputRequestTypeDef",
+    "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "GetDifferencesInputRequestTypeDef",
     "GetFileInputRequestTypeDef",
+    "GetFileOutputTypeDef",
     "GetFolderInputRequestTypeDef",
     "SubModuleTypeDef",
     "SymbolicLinkTypeDef",
     "GetMergeCommitInputRequestTypeDef",
+    "GetMergeCommitOutputTypeDef",
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
+    "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
+    "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
     "RepositoryTriggerTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
+    "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
+    "ListBranchesOutputTypeDef",
+    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListPullRequestsInputRequestTypeDef",
+    "ListPullRequestsOutputTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
+    "MergeBranchesByFastForwardOutputTypeDef",
+    "MergeBranchesBySquashOutputTypeDef",
+    "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "PutFileInputRequestTypeDef",
+    "PutFileOutputTypeDef",
+    "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
     "UpdatePullRequestApprovalRuleContentInputRequestTypeDef",
     "UpdatePullRequestApprovalStateInputRequestTypeDef",
     "UpdatePullRequestDescriptionInputRequestTypeDef",
     "UpdatePullRequestStatusInputRequestTypeDef",
     "UpdatePullRequestTitleInputRequestTypeDef",
     "UpdateRepositoryDescriptionInputRequestTypeDef",
     "UpdateRepositoryNameInputRequestTypeDef",
-    "ApprovalRuleTypeDef",
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "CreateApprovalRuleTemplateOutputTypeDef",
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    "DeleteFileOutputTypeDef",
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    "DeleteRepositoryOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApprovalRuleTemplateOutputTypeDef",
-    "GetBlobOutputTypeDef",
-    "GetFileOutputTypeDef",
-    "GetMergeCommitOutputTypeDef",
-    "GetMergeOptionsOutputTypeDef",
-    "GetPullRequestApprovalStatesOutputTypeDef",
-    "GetPullRequestOverrideStateOutputTypeDef",
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    "ListBranchesOutputTypeDef",
-    "ListPullRequestsOutputTypeDef",
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "MergeBranchesByFastForwardOutputTypeDef",
-    "MergeBranchesBySquashOutputTypeDef",
-    "MergeBranchesByThreeWayOutputTypeDef",
-    "PutFileOutputTypeDef",
-    "PutRepositoryTriggersOutputTypeDef",
     "UpdateApprovalRuleTemplateContentOutputTypeDef",
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
+    "ApprovalRuleTypeDef",
+    "GetPullRequestApprovalStatesOutputTypeDef",
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
@@ -198,21 +205,14 @@
     "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
     "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
-    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    "GetDifferencesInputGetDifferencesPaginateTypeDef",
-    "ListBranchesInputListBranchesPaginateTypeDef",
-    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
     "PutRepositoryTriggersInputRequestTypeDef",
     "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
@@ -335,25 +335,14 @@
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryNames": Sequence[str],
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
 BatchDescribeMergeConflictsErrorTypeDef = TypedDict(
     "BatchDescribeMergeConflictsErrorTypeDef",
     {
         "filePath": str,
         "exceptionName": str,
         "message": str,
     },
@@ -671,21 +660,38 @@
 )
 
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
+CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 
+DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    {
+        "approvalRuleTemplateId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBranchInputRequestTypeDef = TypedDict(
     "DeleteBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
 )
@@ -718,29 +724,56 @@
 )
 
 class DeleteFileInputRequestTypeDef(
     _RequiredDeleteFileInputRequestTypeDef, _OptionalDeleteFileInputRequestTypeDef
 ):
     pass
 
+DeleteFileOutputTypeDef = TypedDict(
+    "DeleteFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "filePath": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePullRequestApprovalRuleInputRequestTypeDef = TypedDict(
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
     {
         "pullRequestId": str,
         "approvalRuleName": str,
     },
 )
 
+DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    {
+        "approvalRuleId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRepositoryInputRequestTypeDef = TypedDict(
     "DeleteRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
+    {
+        "repositoryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -760,24 +793,36 @@
 
 class DescribeMergeConflictsInputRequestTypeDef(
     _RequiredDescribeMergeConflictsInputRequestTypeDef,
     _OptionalDescribeMergeConflictsInputRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "pullRequestId": str,
+    },
+)
+_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
+    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribePullRequestEventsInputRequestTypeDef = TypedDict(
     "_RequiredDescribePullRequestEventsInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalDescribePullRequestEventsInputRequestTypeDef = TypedDict(
@@ -801,14 +846,21 @@
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluatePullRequestApprovalRulesInputRequestTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -856,14 +908,22 @@
     "GetBlobInputRequestTypeDef",
     {
         "repositoryName": str,
         "blobId": str,
     },
 )
 
+GetBlobOutputTypeDef = TypedDict(
+    "GetBlobOutputTypeDef",
+    {
+        "content": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBranchInputRequestTypeDef = TypedDict(
     "GetBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
     total=False,
@@ -893,14 +953,36 @@
 )
 
 class GetCommentReactionsInputRequestTypeDef(
     _RequiredGetCommentReactionsInputRequestTypeDef, _OptionalGetCommentReactionsInputRequestTypeDef
 ):
     pass
 
+_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitId": str,
+    },
+)
+_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "beforeCommitId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
+    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+):
+    pass
+
 _RequiredGetCommentsForComparedCommitInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitId": str,
     },
 )
@@ -916,14 +998,37 @@
 
 class GetCommentsForComparedCommitInputRequestTypeDef(
     _RequiredGetCommentsForComparedCommitInputRequestTypeDef,
     _OptionalGetCommentsForComparedCommitInputRequestTypeDef,
 ):
     pass
 
+_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "pullRequestId": str,
+    },
+)
+_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
+    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+):
+    pass
+
 _RequiredGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
@@ -948,14 +1053,38 @@
     "GetCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "commitId": str,
     },
 )
 
+_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitSpecifier": str,
+    },
+)
+_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "beforeCommitSpecifier": str,
+        "beforePath": str,
+        "afterPath": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetDifferencesInputGetDifferencesPaginateTypeDef(
+    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
+    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetDifferencesInputRequestTypeDef = TypedDict(
     "_RequiredGetDifferencesInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitSpecifier": str,
     },
 )
@@ -992,14 +1121,27 @@
 )
 
 class GetFileInputRequestTypeDef(
     _RequiredGetFileInputRequestTypeDef, _OptionalGetFileInputRequestTypeDef
 ):
     pass
 
+GetFileOutputTypeDef = TypedDict(
+    "GetFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "filePath": str,
+        "fileMode": FileModeTypeEnumType,
+        "fileSize": int,
+        "fileContent": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetFolderInputRequestTypeDef = TypedDict(
     "_RequiredGetFolderInputRequestTypeDef",
     {
         "repositoryName": str,
         "folderPath": str,
     },
 )
@@ -1055,14 +1197,25 @@
 )
 
 class GetMergeCommitInputRequestTypeDef(
     _RequiredGetMergeCommitInputRequestTypeDef, _OptionalGetMergeCommitInputRequestTypeDef
 ):
     pass
 
+GetMergeCommitOutputTypeDef = TypedDict(
+    "GetMergeCommitOutputTypeDef",
+    {
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "mergedCommitId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredGetMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -1102,14 +1255,25 @@
 )
 
 class GetMergeOptionsInputRequestTypeDef(
     _RequiredGetMergeOptionsInputRequestTypeDef, _OptionalGetMergeOptionsInputRequestTypeDef
 ):
     pass
 
+GetMergeOptionsOutputTypeDef = TypedDict(
+    "GetMergeOptionsOutputTypeDef",
+    {
+        "mergeOptions": List[MergeOptionTypeEnumType],
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPullRequestApprovalStatesInputRequestTypeDef = TypedDict(
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -1125,14 +1289,23 @@
     "GetPullRequestOverrideStateInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
 
+GetPullRequestOverrideStateOutputTypeDef = TypedDict(
+    "GetPullRequestOverrideStateOutputTypeDef",
+    {
+        "overridden": bool,
+        "overrider": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRepositoryInputRequestTypeDef = TypedDict(
     "GetRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
@@ -1170,14 +1343,23 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
@@ -1191,14 +1373,43 @@
 
 class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(
     _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
 ):
     pass
 
+ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBranchesInputListBranchesPaginateTypeDef(
+    _RequiredListBranchesInputListBranchesPaginateTypeDef,
+    _OptionalListBranchesInputListBranchesPaginateTypeDef,
+):
+    pass
+
 _RequiredListBranchesInputRequestTypeDef = TypedDict(
     "_RequiredListBranchesInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListBranchesInputRequestTypeDef = TypedDict(
@@ -1210,14 +1421,45 @@
 )
 
 class ListBranchesInputRequestTypeDef(
     _RequiredListBranchesInputRequestTypeDef, _OptionalListBranchesInputRequestTypeDef
 ):
     pass
 
+ListBranchesOutputTypeDef = TypedDict(
+    "ListBranchesOutputTypeDef",
+    {
+        "branches": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "authorArn": str,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPullRequestsInputListPullRequestsPaginateTypeDef(
+    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
+    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPullRequestsInputRequestTypeDef = TypedDict(
     "_RequiredListPullRequestsInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListPullRequestsInputRequestTypeDef = TypedDict(
@@ -1232,14 +1474,23 @@
 )
 
 class ListPullRequestsInputRequestTypeDef(
     _RequiredListPullRequestsInputRequestTypeDef, _OptionalListPullRequestsInputRequestTypeDef
 ):
     pass
 
+ListPullRequestsOutputTypeDef = TypedDict(
+    "ListPullRequestsOutputTypeDef",
+    {
+        "pullRequestIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
@@ -1253,14 +1504,33 @@
 
 class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(
     _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
 ):
     pass
 
+ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    {
+        "repositoryNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "sortBy": SortByEnumType,
+        "order": OrderEnumType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "nextToken": str,
         "sortBy": SortByEnumType,
         "order": OrderEnumType,
     },
@@ -1291,14 +1561,23 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1313,14 +1592,41 @@
 
 class MergeBranchesByFastForwardInputRequestTypeDef(
     _RequiredMergeBranchesByFastForwardInputRequestTypeDef,
     _OptionalMergeBranchesByFastForwardInputRequestTypeDef,
 ):
     pass
 
+MergeBranchesByFastForwardOutputTypeDef = TypedDict(
+    "MergeBranchesByFastForwardOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+MergeBranchesBySquashOutputTypeDef = TypedDict(
+    "MergeBranchesBySquashOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+MergeBranchesByThreeWayOutputTypeDef = TypedDict(
+    "MergeBranchesByThreeWayOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MergeHunkDetailTypeDef = TypedDict(
     "MergeHunkDetailTypeDef",
     {
         "startLine": int,
         "endLine": int,
         "hunkContent": str,
     },
@@ -1364,14 +1670,24 @@
     {
         "pullRequestId": str,
         "revisionId": str,
         "overrideStatus": OverrideStatusType,
     },
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
 _RequiredPostCommentReplyInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentReplyInputRequestTypeDef",
     {
         "inReplyTo": str,
         "content": str,
     },
 )
@@ -1467,14 +1783,32 @@
 )
 
 class PutFileInputRequestTypeDef(
     _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
 ):
     pass
 
+PutFileOutputTypeDef = TypedDict(
+    "PutFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutRepositoryTriggersOutputTypeDef = TypedDict(
+    "PutRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReactionValueFormatsTypeDef = TypedDict(
     "ReactionValueFormatsTypeDef",
     {
         "emoji": str,
         "shortCode": str,
         "unicode": str,
     },
@@ -1486,14 +1820,25 @@
     {
         "trigger": str,
         "failureMessage": str,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1638,319 +1983,117 @@
     "UpdateRepositoryNameInputRequestTypeDef",
     {
         "oldName": str,
         "newName": str,
     },
 )
 
-ApprovalRuleTypeDef = TypedDict(
-    "ApprovalRuleTypeDef",
-    {
-        "approvalRuleId": str,
-        "approvalRuleName": str,
-        "approvalRuleContent": str,
-        "ruleContentSha256": str,
-        "lastModifiedDate": datetime,
-        "creationDate": datetime,
-        "lastModifiedUser": str,
-        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
-    },
-    total=False,
-)
-
-BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
-    {
-        "associatedRepositoryNames": List[str],
-        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateApprovalRuleTemplateOutputTypeDef = TypedDict(
     "CreateApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    {
-        "approvalRuleTemplateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFileOutputTypeDef = TypedDict(
-    "DeleteFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "filePath": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    {
-        "approvalRuleId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
-    {
-        "repositoryId": str,
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
 
 GetApprovalRuleTemplateOutputTypeDef = TypedDict(
     "GetApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBlobOutputTypeDef = TypedDict(
-    "GetBlobOutputTypeDef",
+UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateContentOutputTypeDef",
     {
-        "content": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetFileOutputTypeDef = TypedDict(
-    "GetFileOutputTypeDef",
+UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     {
-        "commitId": str,
-        "blobId": str,
-        "filePath": str,
-        "fileMode": FileModeTypeEnumType,
-        "fileSize": int,
-        "fileContent": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetMergeCommitOutputTypeDef = TypedDict(
-    "GetMergeCommitOutputTypeDef",
+UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateNameOutputTypeDef",
     {
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "mergedCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetMergeOptionsOutputTypeDef = TypedDict(
-    "GetMergeOptionsOutputTypeDef",
+ApprovalRuleTypeDef = TypedDict(
+    "ApprovalRuleTypeDef",
     {
-        "mergeOptions": List[MergeOptionTypeEnumType],
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "approvalRuleId": str,
+        "approvalRuleName": str,
+        "approvalRuleContent": str,
+        "ruleContentSha256": str,
+        "lastModifiedDate": datetime,
+        "creationDate": datetime,
+        "lastModifiedUser": str,
+        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
     },
+    total=False,
 )
 
 GetPullRequestApprovalStatesOutputTypeDef = TypedDict(
     "GetPullRequestApprovalStatesOutputTypeDef",
     {
         "approvals": List[ApprovalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPullRequestOverrideStateOutputTypeDef = TypedDict(
-    "GetPullRequestOverrideStateOutputTypeDef",
-    {
-        "overridden": bool,
-        "overrider": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBranchesOutputTypeDef = TypedDict(
-    "ListBranchesOutputTypeDef",
-    {
-        "branches": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPullRequestsOutputTypeDef = TypedDict(
-    "ListPullRequestsOutputTypeDef",
-    {
-        "pullRequestIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    {
-        "repositoryNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeBranchesByFastForwardOutputTypeDef = TypedDict(
-    "MergeBranchesByFastForwardOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeBranchesBySquashOutputTypeDef = TypedDict(
-    "MergeBranchesBySquashOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeBranchesByThreeWayOutputTypeDef = TypedDict(
-    "MergeBranchesByThreeWayOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutFileOutputTypeDef = TypedDict(
-    "PutFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRepositoryTriggersOutputTypeDef = TypedDict(
-    "PutRepositoryTriggersOutputTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateContentOutputTypeDef",
-    {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
-    {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "associatedRepositoryNames": List[str],
+        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef = TypedDict(
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     {
         "disassociatedRepositoryNames": List[str],
         "errors": List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetRepositoriesOutputTypeDef = TypedDict(
     "BatchGetRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryMetadataTypeDef],
         "repositoriesNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DifferenceTypeDef = TypedDict(
     "DifferenceTypeDef",
     {
         "beforeBlob": BlobMetadataTypeDef,
@@ -1960,55 +2103,55 @@
     total=False,
 )
 
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBranchOutputTypeDef = TypedDict(
     "GetBranchOutputTypeDef",
     {
         "branch": BranchInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCommentContentOutputTypeDef = TypedDict(
     "DeleteCommentContentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommentOutputTypeDef = TypedDict(
     "GetCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PostCommentReplyOutputTypeDef = TypedDict(
     "PostCommentReplyOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCommentOutputTypeDef = TypedDict(
     "UpdateCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommentsForComparedCommitTypeDef = TypedDict(
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
@@ -2067,15 +2210,15 @@
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
@@ -2107,15 +2250,15 @@
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
     {
         "commitId": str,
@@ -2160,15 +2303,15 @@
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
         "filesDeleted": List[FileMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePullRequestInputRequestTypeDef = TypedDict(
     "_RequiredCreatePullRequestInputRequestTypeDef",
     {
         "title": str,
@@ -2185,185 +2328,42 @@
 )
 
 class CreatePullRequestInputRequestTypeDef(
     _RequiredCreatePullRequestInputRequestTypeDef, _OptionalCreatePullRequestInputRequestTypeDef
 ):
     pass
 
-_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
-    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-    },
-)
-_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "beforeCommitId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
-    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-):
-    pass
-
-_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
-    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-):
-    pass
-
-_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitSpecifier": str,
-    },
-)
-_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "beforeCommitSpecifier": str,
-        "beforePath": str,
-        "afterPath": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetDifferencesInputGetDifferencesPaginateTypeDef(
-    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
-    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
-):
-    pass
-
-_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBranchesInputListBranchesPaginateTypeDef(
-    _RequiredListBranchesInputListBranchesPaginateTypeDef,
-    _OptionalListBranchesInputListBranchesPaginateTypeDef,
-):
-    pass
-
-_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "authorArn": str,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPullRequestsInputListPullRequestsPaginateTypeDef(
-    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
-    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
-):
-    pass
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "sortBy": SortByEnumType,
-        "order": OrderEnumType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     {
         "evaluation": EvaluationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFolderOutputTypeDef = TypedDict(
     "GetFolderOutputTypeDef",
     {
         "commitId": str,
         "folderPath": str,
         "treeId": str,
         "subFolders": List[FolderTypeDef],
         "files": List[FileTypeDef],
         "symbolicLinks": List[SymbolicLinkTypeDef],
         "subModules": List[SubModuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
         "triggers": List[RepositoryTriggerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRepositoryTriggersInputRequestTypeDef = TypedDict(
     "PutRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2380,15 +2380,15 @@
 )
 
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryNameIdPairTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
@@ -2453,88 +2453,88 @@
 )
 
 TestRepositoryTriggersOutputTypeDef = TypedDict(
     "TestRepositoryTriggersOutputTypeDef",
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestApprovalRuleContentOutputTypeDef = TypedDict(
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDifferencesOutputTypeDef = TypedDict(
     "GetDifferencesOutputTypeDef",
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommentsForPullRequestOutputTypeDef = TypedDict(
     "GetCommentsForPullRequestOutputTypeDef",
     {
         "commentsForPullRequestData": List[CommentsForPullRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetCommitsOutputTypeDef = TypedDict(
     "BatchGetCommitsOutputTypeDef",
     {
         "commits": List[CommitTypeDef],
         "errors": List[BatchGetCommitsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCommitOutputTypeDef = TypedDict(
     "GetCommitOutputTypeDef",
     {
         "commit": CommitTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMergeConflictsOutputTypeDef = TypedDict(
     "GetMergeConflictsOutputTypeDef",
     {
         "mergeable": bool,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2691,29 +2691,33 @@
     {
         "conflictMetadata": ConflictMetadataTypeDef,
         "mergeHunks": List[MergeHunkTypeDef],
         "nextToken": str,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PullRequestEventTypeDef = TypedDict(
     "PullRequestEventTypeDef",
     {
         "pullRequestId": str,
         "eventDate": datetime,
         "pullRequestEventType": PullRequestEventTypeType,
         "actorArn": str,
         "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
         "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
-        "pullRequestSourceReferenceUpdatedEventMetadata": PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
-        "pullRequestMergedStateChangedEventMetadata": PullRequestMergedStateChangedEventMetadataTypeDef,
+        "pullRequestSourceReferenceUpdatedEventMetadata": (
+            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
+        ),
+        "pullRequestMergedStateChangedEventMetadata": (
+            PullRequestMergedStateChangedEventMetadataTypeDef
+        ),
         "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
         "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
         "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
     },
     total=False,
 )
 
@@ -2763,96 +2767,96 @@
     pass
 
 GetCommentReactionsOutputTypeDef = TypedDict(
     "GetCommentReactionsOutputTypeDef",
     {
         "reactionsForComment": List[ReactionForCommentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePullRequestEventsOutputTypeDef = TypedDict(
     "DescribePullRequestEventsOutputTypeDef",
     {
         "pullRequestEvents": List[PullRequestEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePullRequestOutputTypeDef = TypedDict(
     "CreatePullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPullRequestOutputTypeDef = TypedDict(
     "GetPullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergePullRequestByFastForwardOutputTypeDef = TypedDict(
     "MergePullRequestByFastForwardOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergePullRequestBySquashOutputTypeDef = TypedDict(
     "MergePullRequestBySquashOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MergePullRequestByThreeWayOutputTypeDef = TypedDict(
     "MergePullRequestByThreeWayOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestDescriptionOutputTypeDef = TypedDict(
     "UpdatePullRequestDescriptionOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestStatusOutputTypeDef = TypedDict(
     "UpdatePullRequestStatusOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePullRequestTitleOutputTypeDef = TypedDict(
     "UpdatePullRequestTitleOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/PKG-INFO` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeCommit 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeCommit 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
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
 
 <a id="mypy-boto3-codecommit"></a>
 
 # mypy-boto3-codecommit
 
 [![PyPI - mypy-boto3-codecommit](https://img.shields.io/pypi/v/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecommit?color=blue)](https://pypistats.org/packages/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,15 +368,14 @@
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
@@ -395,116 +395,124 @@
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
+    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
+    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
+    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
+    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
+    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
+    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
     RepositoryTriggerTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
+    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
-    ApprovalRuleTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
-    DeleteFileOutputTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
-    DeleteRepositoryOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
-    GetBlobOutputTypeDef,
-    GetFileOutputTypeDef,
-    GetMergeCommitOutputTypeDef,
-    GetMergeOptionsOutputTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsOutputTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
-    PutFileOutputTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
+    ApprovalRuleTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
@@ -519,21 +527,14 @@
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     PutRepositoryTriggersInputRequestTypeDef,
     TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
@@ -581,42 +582,42 @@
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

### Comparing `mypy-boto3-codecommit-1.26.0.post1/mypy_boto3_codecommit.egg-info/SOURCES.txt` & `mypy-boto3-codecommit-1.27.0/mypy_boto3_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.26.0.post1/setup.py` & `mypy-boto3-codecommit-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codecommit.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecommit",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCommit 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CodeCommit 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 codecommit type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codecommit": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codecommit": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/",
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


# Comparing `tmp/mypy-boto3-dataexchange-1.26.91.tar.gz` & `tmp/mypy-boto3-dataexchange-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dataexchange-1.26.91.tar", last modified: Tue Mar 14 19:48:00 2023, max compression
+gzip compressed data, was "mypy-boto3-dataexchange-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-dataexchange-1.26.91.tar` & `mypy-boto3-dataexchange-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.353219 mypy-boto3-dataexchange-1.26.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18176 2023-03-14 19:48:00.353219 mypy-boto3-dataexchange-1.26.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.337218 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-03-14 19:46:53.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-03-14 19:46:53.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-03-14 19:46:53.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-03-14 19:46:53.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-03-14 19:46:53.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45158 2023-03-14 19:46:54.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45091 2023-03-14 19:46:54.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:48:00.353219 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18176 2023-03-14 19:48:00.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-14 19:48:00.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:48:00.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 19:48:00.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-14 19:48:00.000000 mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:48:00.353219 mypy-boto3-dataexchange-1.26.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-14 19:46:52.000000 mypy-boto3-dataexchange-1.26.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.119099 mypy-boto3-dataexchange-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-07-03 19:50:38.119099 mypy-boto3-dataexchange-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.111099 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45212 2023-07-03 19:35:18.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45145 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:17.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.119099 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-07-03 19:50:37.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:37.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:37.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:37.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:37.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:37.000000 mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.119099 mypy-boto3-dataexchange-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:35:16.000000 mypy-boto3-dataexchange-1.27.0/setup.py
```

### Comparing `mypy-boto3-dataexchange-1.26.91/LICENSE` & `mypy-boto3-dataexchange-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-dataexchange-1.26.91/PKG-INFO` & `mypy-boto3-dataexchange-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dataexchange
-Version: 1.26.91
-Summary: Type annotations for boto3.DataExchange 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.DataExchange 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dataexchange"></a>
 
 # mypy-boto3-dataexchange
 
 [![PyPI - mypy-boto3-dataexchange](https://img.shields.io/pypi/v/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dataexchange?color=blue)](https://pypistats.org/packages/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,86 +361,86 @@
     S3SnapshotAssetTypeDef,
     AssetSourceEntryTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
-    ResponseMetadataTypeDef,
     CreateRevisionRequestRequestTypeDef,
+    CreateRevisionResponseTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
+    GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
     KmsKeyToGrantTypeDef,
-    PaginatorConfigTypeDef,
+    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListEventActionsRequestListEventActionsPaginateTypeDef,
     ListEventActionsRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListRevisionAssetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RevokeRevisionRequestRequestTypeDef,
+    RevokeRevisionResponseTypeDef,
     SendApiAssetRequestRequestTypeDef,
+    SendApiAssetResponseTypeDef,
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
+    UpdateRevisionResponseTypeDef,
     ImportAssetsFromS3RequestDetailsTypeDef,
     ImportAssetsFromS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
     ExportAssetsToS3ResponseDetailsTypeDef,
-    DataSetEntryTypeDef,
     CreateDataSetResponseTypeDef,
-    CreateRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    DataSetEntryTypeDef,
     GetDataSetResponseTypeDef,
-    GetRevisionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RevokeRevisionResponseTypeDef,
-    SendApiAssetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
-    UpdateRevisionResponseTypeDef,
     DatabaseLFTagPolicyAndPermissionsTypeDef,
     DatabaseLFTagPolicyTypeDef,
     TableLFTagPolicyAndPermissionsTypeDef,
     TableLFTagPolicyTypeDef,
     DetailsTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
     S3DataAccessAssetSourceEntryTypeDef,
     S3DataAccessAssetTypeDef,
-    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListEventActionsRequestListEventActionsPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListDataSetRevisionsResponseTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
     ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
     JobErrorTypeDef,
@@ -478,42 +478,42 @@
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

### Comparing `mypy-boto3-dataexchange-1.26.91/README.md` & `mypy-boto3-dataexchange-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dataexchange"></a>
 
 # mypy-boto3-dataexchange
 
 [![PyPI - mypy-boto3-dataexchange](https://img.shields.io/pypi/v/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dataexchange?color=blue)](https://pypistats.org/packages/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,86 +329,86 @@
     S3SnapshotAssetTypeDef,
     AssetSourceEntryTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
-    ResponseMetadataTypeDef,
     CreateRevisionRequestRequestTypeDef,
+    CreateRevisionResponseTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
+    GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
     KmsKeyToGrantTypeDef,
-    PaginatorConfigTypeDef,
+    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListEventActionsRequestListEventActionsPaginateTypeDef,
     ListEventActionsRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListRevisionAssetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RevokeRevisionRequestRequestTypeDef,
+    RevokeRevisionResponseTypeDef,
     SendApiAssetRequestRequestTypeDef,
+    SendApiAssetResponseTypeDef,
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
+    UpdateRevisionResponseTypeDef,
     ImportAssetsFromS3RequestDetailsTypeDef,
     ImportAssetsFromS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
     ExportAssetsToS3ResponseDetailsTypeDef,
-    DataSetEntryTypeDef,
     CreateDataSetResponseTypeDef,
-    CreateRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    DataSetEntryTypeDef,
     GetDataSetResponseTypeDef,
-    GetRevisionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RevokeRevisionResponseTypeDef,
-    SendApiAssetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
-    UpdateRevisionResponseTypeDef,
     DatabaseLFTagPolicyAndPermissionsTypeDef,
     DatabaseLFTagPolicyTypeDef,
     TableLFTagPolicyAndPermissionsTypeDef,
     TableLFTagPolicyTypeDef,
     DetailsTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
     S3DataAccessAssetSourceEntryTypeDef,
     S3DataAccessAssetTypeDef,
-    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListEventActionsRequestListEventActionsPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListDataSetRevisionsResponseTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
     ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
     JobErrorTypeDef,
@@ -446,42 +446,42 @@
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

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/__init__.py` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/__init__.pyi` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/__main__.py` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataExchange 1.26.91\nVersion:         1.26.91\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.DataExchange 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.91")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/client.py` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/client.pyi` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/literals.py` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/literals.pyi`

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
     "AssetTypeType",
     "CodeType",
     "DatabaseLFTagPolicyPermissionType",
     "JobErrorLimitNameType",
     "JobErrorResourceTypesType",
     "LFPermissionType",
@@ -42,15 +41,14 @@
     "DataExchangeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssetTypeType = Literal[
     "API_GATEWAY_API",
     "LAKE_FORMATION_DATA_PERMISSION",
     "REDSHIFT_DATA_SHARE",
     "S3_DATA_ACCESS",
     "S3_SNAPSHOT",
 ]
@@ -108,14 +106,15 @@
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
@@ -155,14 +154,15 @@
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
@@ -260,14 +260,15 @@
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
@@ -303,14 +304,15 @@
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
@@ -329,16 +331,19 @@
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
@@ -422,15 +427,17 @@
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

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/literals.pyi` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/literals.py`

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
     "AssetTypeType",
     "CodeType",
     "DatabaseLFTagPolicyPermissionType",
     "JobErrorLimitNameType",
     "JobErrorResourceTypesType",
     "LFPermissionType",
@@ -41,14 +42,15 @@
     "DataExchangeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AssetTypeType = Literal[
     "API_GATEWAY_API",
     "LAKE_FORMATION_DATA_PERMISSION",
     "REDSHIFT_DATA_SHARE",
     "S3_DATA_ACCESS",
     "S3_SNAPSHOT",
 ]
@@ -106,14 +108,15 @@
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
@@ -153,14 +156,15 @@
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
@@ -258,14 +262,15 @@
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
@@ -301,14 +306,15 @@
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
@@ -327,16 +333,19 @@
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
@@ -420,15 +429,17 @@
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

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/paginator.py` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,95 +44,88 @@
     "ListDataSetRevisionsPaginator",
     "ListDataSetsPaginator",
     "ListEventActionsPaginator",
     "ListJobsPaginator",
     "ListRevisionAssetsPaginator",
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
 class ListDataSetRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DataSetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
         """
 
-
 class ListDataSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, Origin: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Origin: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
         """
 
-
 class ListEventActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
     """
 
     def paginate(
-        self, *, EventSourceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EventSourceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
         """
 
-
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listjobspaginator)
     """
 
     def paginate(
         self,
         *,
         DataSetId: str = ...,
         RevisionId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listjobspaginator)
         """
 
-
 class ListRevisionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, RevisionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DataSetId: str, RevisionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRevisionAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
         """
```

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/paginator.pyi` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,88 +44,95 @@
     "ListDataSetRevisionsPaginator",
     "ListDataSetsPaginator",
     "ListEventActionsPaginator",
     "ListJobsPaginator",
     "ListRevisionAssetsPaginator",
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
 class ListDataSetRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DataSetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSetRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetrevisionspaginator)
         """
 
+
 class ListDataSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, Origin: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Origin: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listdatasetspaginator)
         """
 
+
 class ListEventActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
     """
 
     def paginate(
-        self, *, EventSourceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EventSourceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListEventActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listeventactionspaginator)
         """
 
+
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listjobspaginator)
     """
 
     def paginate(
         self,
         *,
         DataSetId: str = ...,
         RevisionId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listjobspaginator)
         """
 
+
 class ListRevisionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
     """
 
     def paginate(
-        self, *, DataSetId: str, RevisionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DataSetId: str, RevisionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRevisionAssetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange.Paginator.ListRevisionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/paginators/#listrevisionassetspaginator)
         """
```

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/type_defs.py` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,86 +46,86 @@
     "S3SnapshotAssetTypeDef",
     "AssetSourceEntryTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateRevisionRequestRequestTypeDef",
+    "CreateRevisionResponseTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "RevisionPublishedTypeDef",
     "ExportAssetToSignedUrlRequestDetailsTypeDef",
     "ExportAssetToSignedUrlResponseDetailsTypeDef",
     "RevisionDestinationEntryTypeDef",
     "GetAssetRequestRequestTypeDef",
     "GetDataSetRequestRequestTypeDef",
     "GetEventActionRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetRevisionRequestRequestTypeDef",
+    "GetRevisionResponseTypeDef",
     "ImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     "ImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     "ImportAssetFromSignedUrlResponseDetailsTypeDef",
     "RedshiftDataShareAssetSourceEntryTypeDef",
     "KmsKeyToGrantTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     "ListDataSetRevisionsRequestRequestTypeDef",
     "RevisionEntryTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
     "ListEventActionsRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListRevisionAssetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeRevisionRequestRequestTypeDef",
+    "RevokeRevisionResponseTypeDef",
     "SendApiAssetRequestRequestTypeDef",
+    "SendApiAssetResponseTypeDef",
     "StartJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "UpdateRevisionRequestRequestTypeDef",
+    "UpdateRevisionResponseTypeDef",
     "ImportAssetsFromS3RequestDetailsTypeDef",
     "ImportAssetsFromS3ResponseDetailsTypeDef",
     "AutoExportRevisionToS3RequestDetailsTypeDef",
     "ExportAssetsToS3RequestDetailsTypeDef",
     "ExportAssetsToS3ResponseDetailsTypeDef",
-    "DataSetEntryTypeDef",
     "CreateDataSetResponseTypeDef",
-    "CreateRevisionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "DataSetEntryTypeDef",
     "GetDataSetResponseTypeDef",
-    "GetRevisionResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RevokeRevisionResponseTypeDef",
-    "SendApiAssetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
-    "UpdateRevisionResponseTypeDef",
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
     "DatabaseLFTagPolicyTypeDef",
     "TableLFTagPolicyAndPermissionsTypeDef",
     "TableLFTagPolicyTypeDef",
     "DetailsTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     "S3DataAccessAssetSourceEntryTypeDef",
     "S3DataAccessAssetTypeDef",
-    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
     "JobErrorTypeDef",
@@ -291,25 +291,14 @@
 OriginDetailsTypeDef = TypedDict(
     "OriginDetailsTypeDef",
     {
         "ProductId": str,
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
 _RequiredCreateRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalCreateRevisionRequestRequestTypeDef = TypedDict(
@@ -324,14 +313,33 @@
 
 class CreateRevisionRequestRequestTypeDef(
     _RequiredCreateRevisionRequestRequestTypeDef, _OptionalCreateRevisionRequestRequestTypeDef
 ):
     pass
 
 
+CreateRevisionResponseTypeDef = TypedDict(
+    "CreateRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -370,14 +378,21 @@
 ImportAssetFromSignedUrlJobErrorDetailsTypeDef = TypedDict(
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     {
         "AssetName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RevisionPublishedTypeDef = TypedDict(
     "RevisionPublishedTypeDef",
     {
         "DataSetId": str,
     },
 )
 
@@ -471,14 +486,33 @@
     "GetRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
+GetRevisionResponseTypeDef = TypedDict(
+    "GetRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef = TypedDict(
     "_RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     {
         "ApiId": str,
         "ApiName": str,
         "ApiSpecificationMd5Hash": str,
         "DataSetId": str,
@@ -581,24 +615,36 @@
 KmsKeyToGrantTypeDef = TypedDict(
     "KmsKeyToGrantTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DataSetId": str,
+    },
+)
+_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
+    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDataSetRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetRevisionsRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalListDataSetRevisionsRequestRequestTypeDef = TypedDict(
@@ -642,45 +688,96 @@
 )
 
 
 class RevisionEntryTypeDef(_RequiredRevisionEntryTypeDef, _OptionalRevisionEntryTypeDef):
     pass
 
 
+ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "Origin": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDataSetsRequestRequestTypeDef = TypedDict(
     "ListDataSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Origin": str,
     },
     total=False,
 )
 
+ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
+    {
+        "EventSourceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEventActionsRequestRequestTypeDef = TypedDict(
     "ListEventActionsRequestRequestTypeDef",
     {
         "EventSourceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "DataSetId": str,
+        "RevisionId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "MaxResults": int,
         "NextToken": str,
         "RevisionId": str,
     },
     total=False,
 )
 
+_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
+    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRevisionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListRevisionAssetsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
@@ -704,23 +801,70 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
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
 RevokeRevisionRequestRequestTypeDef = TypedDict(
     "RevokeRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
         "RevocationComment": str,
     },
 )
 
+RevokeRevisionResponseTypeDef = TypedDict(
+    "RevokeRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendApiAssetRequestRequestTypeDef = TypedDict(
     "_RequiredSendApiAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -740,14 +884,23 @@
 
 class SendApiAssetRequestRequestTypeDef(
     _RequiredSendApiAssetRequestRequestTypeDef, _OptionalSendApiAssetRequestRequestTypeDef
 ):
     pass
 
 
+SendApiAssetResponseTypeDef = TypedDict(
+    "SendApiAssetResponseTypeDef",
+    {
+        "Body": str,
+        "ResponseHeaders": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartJobRequestRequestTypeDef = TypedDict(
     "StartJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -818,14 +971,32 @@
 
 class UpdateRevisionRequestRequestTypeDef(
     _RequiredUpdateRevisionRequestRequestTypeDef, _OptionalUpdateRevisionRequestRequestTypeDef
 ):
     pass
 
 
+UpdateRevisionResponseTypeDef = TypedDict(
+    "UpdateRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImportAssetsFromS3RequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromS3RequestDetailsTypeDef",
     {
         "AssetSources": Sequence[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -904,84 +1075,58 @@
 
 class ExportAssetsToS3ResponseDetailsTypeDef(
     _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
 ):
     pass
 
 
-_RequiredDataSetEntryTypeDef = TypedDict(
-    "_RequiredDataSetEntryTypeDef",
+CreateDataSetResponseTypeDef = TypedDict(
+    "CreateDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
-        "UpdatedAt": datetime,
-    },
-)
-_OptionalDataSetEntryTypeDef = TypedDict(
-    "_OptionalDataSetEntryTypeDef",
-    {
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
-    pass
-
-
-CreateDataSetResponseTypeDef = TypedDict(
-    "CreateDataSetResponseTypeDef",
+_RequiredDataSetEntryTypeDef = TypedDict(
+    "_RequiredDataSetEntryTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
-        "OriginDetails": OriginDetailsTypeDef,
-        "SourceId": str,
-        "Tags": Dict[str, str],
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateRevisionResponseTypeDef = TypedDict(
-    "CreateRevisionResponseTypeDef",
+_OptionalDataSetEntryTypeDef = TypedDict(
+    "_OptionalDataSetEntryTypeDef",
     {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
+        "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+
+class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
+    pass
+
 
 GetDataSetResponseTypeDef = TypedDict(
     "GetDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
@@ -989,69 +1134,15 @@
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "Tags": Dict[str, str],
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRevisionResponseTypeDef = TypedDict(
-    "GetRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevokeRevisionResponseTypeDef = TypedDict(
-    "RevokeRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendApiAssetResponseTypeDef = TypedDict(
-    "SendApiAssetResponseTypeDef",
-    {
-        "Body": str,
-        "ResponseHeaders": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataSetResponseTypeDef = TypedDict(
     "UpdateDataSetResponseTypeDef",
     {
         "Arn": str,
@@ -1060,33 +1151,15 @@
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRevisionResponseTypeDef = TypedDict(
-    "UpdateRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
     {
         "Expression": Sequence[LFTagTypeDef],
@@ -1242,93 +1315,20 @@
 
 class S3DataAccessAssetTypeDef(
     _RequiredS3DataAccessAssetTypeDef, _OptionalS3DataAccessAssetTypeDef
 ):
     pass
 
 
-_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
-    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-):
-    pass
-
-
-ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "Origin": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
-    {
-        "EventSourceId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
-    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-):
-    pass
-
-
 ListDataSetRevisionsResponseTypeDef = TypedDict(
     "ListDataSetRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[RevisionEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsTypeDef,
@@ -1337,15 +1337,15 @@
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
     "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "CatalogId": str,
@@ -1461,15 +1461,15 @@
     {
         "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
         "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventActionEntryTypeDef = TypedDict(
     "EventActionEntryTypeDef",
     {
         "Action": ActionTypeDef,
@@ -1486,15 +1486,15 @@
     {
         "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
         "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateEventActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventActionRequestRequestTypeDef",
     {
         "EventActionId": str,
@@ -1520,15 +1520,15 @@
     {
         "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
         "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LFTagPolicyDetailsTypeDef = TypedDict(
     "LFTagPolicyDetailsTypeDef",
     {
         "CatalogId": str,
@@ -1578,15 +1578,15 @@
 )
 
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LakeFormationDataPermissionDetailsTypeDef = TypedDict(
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
@@ -1609,30 +1609,30 @@
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJobEntryTypeDef = TypedDict(
     "_RequiredJobEntryTypeDef",
     {
         "Arn": str,
@@ -1682,15 +1682,15 @@
 
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssetDetailsTypeDef = TypedDict(
     "AssetDetailsTypeDef",
     {
         "S3SnapshotAsset": S3SnapshotAssetTypeDef,
@@ -1738,15 +1738,15 @@
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssetResponseTypeDef = TypedDict(
     "UpdateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -1755,19 +1755,19 @@
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRevisionAssetsResponseTypeDef = TypedDict(
     "ListRevisionAssetsResponseTypeDef",
     {
         "Assets": List[AssetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange/type_defs.pyi` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,86 +45,86 @@
     "S3SnapshotAssetTypeDef",
     "AssetSourceEntryTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateRevisionRequestRequestTypeDef",
+    "CreateRevisionResponseTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "RevisionPublishedTypeDef",
     "ExportAssetToSignedUrlRequestDetailsTypeDef",
     "ExportAssetToSignedUrlResponseDetailsTypeDef",
     "RevisionDestinationEntryTypeDef",
     "GetAssetRequestRequestTypeDef",
     "GetDataSetRequestRequestTypeDef",
     "GetEventActionRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetRevisionRequestRequestTypeDef",
+    "GetRevisionResponseTypeDef",
     "ImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     "ImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     "ImportAssetFromSignedUrlResponseDetailsTypeDef",
     "RedshiftDataShareAssetSourceEntryTypeDef",
     "KmsKeyToGrantTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     "ListDataSetRevisionsRequestRequestTypeDef",
     "RevisionEntryTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
     "ListEventActionsRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListRevisionAssetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeRevisionRequestRequestTypeDef",
+    "RevokeRevisionResponseTypeDef",
     "SendApiAssetRequestRequestTypeDef",
+    "SendApiAssetResponseTypeDef",
     "StartJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "UpdateRevisionRequestRequestTypeDef",
+    "UpdateRevisionResponseTypeDef",
     "ImportAssetsFromS3RequestDetailsTypeDef",
     "ImportAssetsFromS3ResponseDetailsTypeDef",
     "AutoExportRevisionToS3RequestDetailsTypeDef",
     "ExportAssetsToS3RequestDetailsTypeDef",
     "ExportAssetsToS3ResponseDetailsTypeDef",
-    "DataSetEntryTypeDef",
     "CreateDataSetResponseTypeDef",
-    "CreateRevisionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "DataSetEntryTypeDef",
     "GetDataSetResponseTypeDef",
-    "GetRevisionResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RevokeRevisionResponseTypeDef",
-    "SendApiAssetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
-    "UpdateRevisionResponseTypeDef",
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
     "DatabaseLFTagPolicyTypeDef",
     "TableLFTagPolicyAndPermissionsTypeDef",
     "TableLFTagPolicyTypeDef",
     "DetailsTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     "S3DataAccessAssetSourceEntryTypeDef",
     "S3DataAccessAssetTypeDef",
-    "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
     "JobErrorTypeDef",
@@ -282,25 +282,14 @@
 OriginDetailsTypeDef = TypedDict(
     "OriginDetailsTypeDef",
     {
         "ProductId": str,
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
 _RequiredCreateRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalCreateRevisionRequestRequestTypeDef = TypedDict(
@@ -313,14 +302,33 @@
 )
 
 class CreateRevisionRequestRequestTypeDef(
     _RequiredCreateRevisionRequestRequestTypeDef, _OptionalCreateRevisionRequestRequestTypeDef
 ):
     pass
 
+CreateRevisionResponseTypeDef = TypedDict(
+    "CreateRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -359,14 +367,21 @@
 ImportAssetFromSignedUrlJobErrorDetailsTypeDef = TypedDict(
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     {
         "AssetName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RevisionPublishedTypeDef = TypedDict(
     "RevisionPublishedTypeDef",
     {
         "DataSetId": str,
     },
 )
 
@@ -456,14 +471,33 @@
     "GetRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
+GetRevisionResponseTypeDef = TypedDict(
+    "GetRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef = TypedDict(
     "_RequiredImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     {
         "ApiId": str,
         "ApiName": str,
         "ApiSpecificationMd5Hash": str,
         "DataSetId": str,
@@ -560,24 +594,34 @@
 KmsKeyToGrantTypeDef = TypedDict(
     "KmsKeyToGrantTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DataSetId": str,
+    },
+)
+_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
+    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDataSetRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetRevisionsRequestRequestTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalListDataSetRevisionsRequestRequestTypeDef = TypedDict(
@@ -617,45 +661,94 @@
     },
     total=False,
 )
 
 class RevisionEntryTypeDef(_RequiredRevisionEntryTypeDef, _OptionalRevisionEntryTypeDef):
     pass
 
+ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "Origin": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDataSetsRequestRequestTypeDef = TypedDict(
     "ListDataSetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Origin": str,
     },
     total=False,
 )
 
+ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
+    "ListEventActionsRequestListEventActionsPaginateTypeDef",
+    {
+        "EventSourceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEventActionsRequestRequestTypeDef = TypedDict(
     "ListEventActionsRequestRequestTypeDef",
     {
         "EventSourceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "DataSetId": str,
+        "RevisionId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "MaxResults": int,
         "NextToken": str,
         "RevisionId": str,
     },
     total=False,
 )
 
+_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
+    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRevisionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListRevisionAssetsRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
     },
 )
@@ -677,23 +770,70 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
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
 RevokeRevisionRequestRequestTypeDef = TypedDict(
     "RevokeRevisionRequestRequestTypeDef",
     {
         "DataSetId": str,
         "RevisionId": str,
         "RevocationComment": str,
     },
 )
 
+RevokeRevisionResponseTypeDef = TypedDict(
+    "RevokeRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendApiAssetRequestRequestTypeDef = TypedDict(
     "_RequiredSendApiAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -711,14 +851,23 @@
 )
 
 class SendApiAssetRequestRequestTypeDef(
     _RequiredSendApiAssetRequestRequestTypeDef, _OptionalSendApiAssetRequestRequestTypeDef
 ):
     pass
 
+SendApiAssetResponseTypeDef = TypedDict(
+    "SendApiAssetResponseTypeDef",
+    {
+        "Body": str,
+        "ResponseHeaders": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartJobRequestRequestTypeDef = TypedDict(
     "StartJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -785,14 +934,32 @@
 )
 
 class UpdateRevisionRequestRequestTypeDef(
     _RequiredUpdateRevisionRequestRequestTypeDef, _OptionalUpdateRevisionRequestRequestTypeDef
 ):
     pass
 
+UpdateRevisionResponseTypeDef = TypedDict(
+    "UpdateRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "Comment": str,
+        "CreatedAt": datetime,
+        "DataSetId": str,
+        "Finalized": bool,
+        "Id": str,
+        "SourceId": str,
+        "UpdatedAt": datetime,
+        "RevocationComment": str,
+        "Revoked": bool,
+        "RevokedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImportAssetsFromS3RequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromS3RequestDetailsTypeDef",
     {
         "AssetSources": Sequence[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -865,82 +1032,56 @@
 )
 
 class ExportAssetsToS3ResponseDetailsTypeDef(
     _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
 ):
     pass
 
-_RequiredDataSetEntryTypeDef = TypedDict(
-    "_RequiredDataSetEntryTypeDef",
+CreateDataSetResponseTypeDef = TypedDict(
+    "CreateDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
-        "UpdatedAt": datetime,
-    },
-)
-_OptionalDataSetEntryTypeDef = TypedDict(
-    "_OptionalDataSetEntryTypeDef",
-    {
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
+        "Tags": Dict[str, str],
+        "UpdatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
-    pass
-
-CreateDataSetResponseTypeDef = TypedDict(
-    "CreateDataSetResponseTypeDef",
+_RequiredDataSetEntryTypeDef = TypedDict(
+    "_RequiredDataSetEntryTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
-        "OriginDetails": OriginDetailsTypeDef,
-        "SourceId": str,
-        "Tags": Dict[str, str],
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateRevisionResponseTypeDef = TypedDict(
-    "CreateRevisionResponseTypeDef",
+_OptionalDataSetEntryTypeDef = TypedDict(
+    "_OptionalDataSetEntryTypeDef",
     {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
+        "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class DataSetEntryTypeDef(_RequiredDataSetEntryTypeDef, _OptionalDataSetEntryTypeDef):
+    pass
 
 GetDataSetResponseTypeDef = TypedDict(
     "GetDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
@@ -948,69 +1089,15 @@
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "Tags": Dict[str, str],
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRevisionResponseTypeDef = TypedDict(
-    "GetRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "Tags": Dict[str, str],
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevokeRevisionResponseTypeDef = TypedDict(
-    "RevokeRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendApiAssetResponseTypeDef = TypedDict(
-    "SendApiAssetResponseTypeDef",
-    {
-        "Body": str,
-        "ResponseHeaders": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataSetResponseTypeDef = TypedDict(
     "UpdateDataSetResponseTypeDef",
     {
         "Arn": str,
@@ -1019,33 +1106,15 @@
         "Description": str,
         "Id": str,
         "Name": str,
         "Origin": OriginType,
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRevisionResponseTypeDef = TypedDict(
-    "UpdateRevisionResponseTypeDef",
-    {
-        "Arn": str,
-        "Comment": str,
-        "CreatedAt": datetime,
-        "DataSetId": str,
-        "Finalized": bool,
-        "Id": str,
-        "SourceId": str,
-        "UpdatedAt": datetime,
-        "RevocationComment": str,
-        "Revoked": bool,
-        "RevokedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
     {
         "Expression": Sequence[LFTagTypeDef],
@@ -1193,89 +1262,20 @@
 )
 
 class S3DataAccessAssetTypeDef(
     _RequiredS3DataAccessAssetTypeDef, _OptionalS3DataAccessAssetTypeDef
 ):
     pass
 
-_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(
-    _RequiredListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    _OptionalListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-):
-    pass
-
-ListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "Origin": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventActionsRequestListEventActionsPaginateTypeDef = TypedDict(
-    "ListEventActionsRequestListEventActionsPaginateTypeDef",
-    {
-        "EventSourceId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(
-    _RequiredListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-    _OptionalListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
-):
-    pass
-
 ListDataSetRevisionsResponseTypeDef = TypedDict(
     "ListDataSetRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[RevisionEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsTypeDef,
@@ -1284,15 +1284,15 @@
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
     "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "CatalogId": str,
@@ -1402,15 +1402,15 @@
     {
         "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
         "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventActionEntryTypeDef = TypedDict(
     "EventActionEntryTypeDef",
     {
         "Action": ActionTypeDef,
@@ -1427,15 +1427,15 @@
     {
         "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
         "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateEventActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventActionRequestRequestTypeDef",
     {
         "EventActionId": str,
@@ -1459,15 +1459,15 @@
     {
         "Action": ActionTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
         "Event": EventTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LFTagPolicyDetailsTypeDef = TypedDict(
     "LFTagPolicyDetailsTypeDef",
     {
         "CatalogId": str,
@@ -1517,15 +1517,15 @@
 )
 
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LakeFormationDataPermissionDetailsTypeDef = TypedDict(
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
@@ -1548,30 +1548,30 @@
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
         "Id": str,
         "State": StateType,
         "Type": TypeType,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredJobEntryTypeDef = TypedDict(
     "_RequiredJobEntryTypeDef",
     {
         "Arn": str,
@@ -1617,15 +1617,15 @@
     pass
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssetDetailsTypeDef = TypedDict(
     "AssetDetailsTypeDef",
     {
         "S3SnapshotAsset": S3SnapshotAssetTypeDef,
@@ -1671,15 +1671,15 @@
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssetResponseTypeDef = TypedDict(
     "UpdateAssetResponseTypeDef",
     {
         "Arn": str,
@@ -1688,19 +1688,19 @@
         "CreatedAt": datetime,
         "DataSetId": str,
         "Id": str,
         "Name": str,
         "RevisionId": str,
         "SourceId": str,
         "UpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRevisionAssetsResponseTypeDef = TypedDict(
     "ListRevisionAssetsResponseTypeDef",
     {
         "Assets": List[AssetEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/PKG-INFO` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dataexchange
-Version: 1.26.91
-Summary: Type annotations for boto3.DataExchange 1.26.91 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.DataExchange 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dataexchange"></a>
 
 # mypy-boto3-dataexchange
 
 [![PyPI - mypy-boto3-dataexchange](https://img.shields.io/pypi/v/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dataexchange?color=blue)](https://pypistats.org/packages/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.26.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,86 +361,86 @@
     S3SnapshotAssetTypeDef,
     AssetSourceEntryTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
-    ResponseMetadataTypeDef,
     CreateRevisionRequestRequestTypeDef,
+    CreateRevisionResponseTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
+    GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
     KmsKeyToGrantTypeDef,
-    PaginatorConfigTypeDef,
+    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListEventActionsRequestListEventActionsPaginateTypeDef,
     ListEventActionsRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListRevisionAssetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RevokeRevisionRequestRequestTypeDef,
+    RevokeRevisionResponseTypeDef,
     SendApiAssetRequestRequestTypeDef,
+    SendApiAssetResponseTypeDef,
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
+    UpdateRevisionResponseTypeDef,
     ImportAssetsFromS3RequestDetailsTypeDef,
     ImportAssetsFromS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
     ExportAssetsToS3ResponseDetailsTypeDef,
-    DataSetEntryTypeDef,
     CreateDataSetResponseTypeDef,
-    CreateRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    DataSetEntryTypeDef,
     GetDataSetResponseTypeDef,
-    GetRevisionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RevokeRevisionResponseTypeDef,
-    SendApiAssetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
-    UpdateRevisionResponseTypeDef,
     DatabaseLFTagPolicyAndPermissionsTypeDef,
     DatabaseLFTagPolicyTypeDef,
     TableLFTagPolicyAndPermissionsTypeDef,
     TableLFTagPolicyTypeDef,
     DetailsTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
     S3DataAccessAssetSourceEntryTypeDef,
     S3DataAccessAssetTypeDef,
-    ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListEventActionsRequestListEventActionsPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef,
     ListDataSetRevisionsResponseTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
     ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
     JobErrorTypeDef,
@@ -478,42 +478,42 @@
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

### Comparing `mypy-boto3-dataexchange-1.26.91/mypy_boto3_dataexchange.egg-info/SOURCES.txt` & `mypy-boto3-dataexchange-1.27.0/mypy_boto3_dataexchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.26.91/setup.py` & `mypy-boto3-dataexchange-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-dataexchange.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dataexchange",
-    version="1.26.91",
+    version="1.27.0",
     packages=["mypy_boto3_dataexchange"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataExchange 1.26.91 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.DataExchange 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/",
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


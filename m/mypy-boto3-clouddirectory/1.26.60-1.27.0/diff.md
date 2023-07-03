# Comparing `tmp/mypy-boto3-clouddirectory-1.26.60.tar.gz` & `tmp/mypy-boto3-clouddirectory-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-clouddirectory-1.26.60.tar", last modified: Mon Jan 30 21:06:23 2023, max compression
+gzip compressed data, was "mypy-boto3-clouddirectory-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-clouddirectory-1.26.60.tar` & `mypy-boto3-clouddirectory-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.478471 mypy-boto3-clouddirectory-1.26.60/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25888 2023-01-30 21:06:23.478471 mypy-boto3-clouddirectory-1.26.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.474471 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56756 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56664 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-01-30 21:05:11.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-01-30 21:05:11.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-01-30 21:05:11.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86355 2023-01-30 21:05:12.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86228 2023-01-30 21:05:12.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.478471 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25888 2023-01-30 21:06:23.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-30 21:06:23.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 21:06:23.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-30 21:06:23.000000 mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:06:23.478471 mypy-boto3-clouddirectory-1.26.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-30 21:05:10.000000 mypy-boto3-clouddirectory-1.26.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.426943 mypy-boto3-clouddirectory-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25871 2023-07-03 19:50:29.422943 mypy-boto3-clouddirectory-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24358 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.414943 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56752 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56660 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-03 19:33:39.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-03 19:33:39.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-07-03 19:33:39.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-03 19:33:39.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86497 2023-07-03 19:33:41.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86370 2023-07-03 19:33:40.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.422943 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25871 2023-07-03 19:50:29.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:29.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:29.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:29.000000 mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.426943 mypy-boto3-clouddirectory-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:33:38.000000 mypy-boto3-clouddirectory-1.27.0/setup.py
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/LICENSE` & `mypy-boto3-clouddirectory-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-clouddirectory-1.26.60/PKG-INFO` & `mypy-boto3-clouddirectory-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.26.60
-Summary: Type annotations for boto3.CloudDirectory 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudDirectory 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-clouddirectory"></a>
 
 # mypy-boto3-clouddirectory
 
 [![PyPI - mypy-boto3-clouddirectory](https://img.shields.io/pypi/v/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-clouddirectory?color=blue)](https://pypistats.org/packages/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -419,15 +419,17 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
@@ -437,49 +439,89 @@
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
     CreateDirectoryRequestRequestTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
+    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
+    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
+    EnableDirectoryResponseTypeDef,
     RuleTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
+    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -495,61 +537,35 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
     BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
+    GetObjectInformationResponseTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DeleteDirectoryResponseTypeDef,
-    DeleteSchemaResponseTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableDirectoryResponseTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
-    GetObjectInformationResponseTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    PublishSchemaResponseTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
@@ -558,30 +574,14 @@
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
     AddFacetToObjectRequestRequestTypeDef,
     BatchAddFacetToObjectTypeDef,
     BatchCreateObjectTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
@@ -657,42 +657,42 @@
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

### Comparing `mypy-boto3-clouddirectory-1.26.60/README.md` & `mypy-boto3-clouddirectory-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-clouddirectory"></a>
 
 # mypy-boto3-clouddirectory
 
 [![PyPI - mypy-boto3-clouddirectory](https://img.shields.io/pypi/v/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-clouddirectory?color=blue)](https://pypistats.org/packages/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,15 +387,17 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
@@ -405,49 +407,89 @@
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
     CreateDirectoryRequestRequestTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
+    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
+    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
+    EnableDirectoryResponseTypeDef,
     RuleTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
+    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -463,61 +505,35 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
     BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
+    GetObjectInformationResponseTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DeleteDirectoryResponseTypeDef,
-    DeleteSchemaResponseTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableDirectoryResponseTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
-    GetObjectInformationResponseTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    PublishSchemaResponseTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
@@ -526,30 +542,14 @@
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
     AddFacetToObjectRequestRequestTypeDef,
     BatchAddFacetToObjectTypeDef,
     BatchCreateObjectTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
@@ -625,42 +625,42 @@
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

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/__init__.py` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/__init__.pyi` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/__main__.py` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudDirectory 1.26.60\nVersion:         1.26.60\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.CloudDirectory 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.60")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/client.py` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_directory)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_directory)
         """
 
     def get_facet(self, *, SchemaArn: str, Name: str) -> GetFacetResponseTypeDef:
         """
-        Gets details of the  Facet, such as facet name, attributes,  Rule s, or
+        Gets details of the  Facet, such as facet name, attributes,  Rules, or
         `ObjectType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_facet)
         """
 
     def get_link_attributes(
@@ -943,15 +943,15 @@
         *,
         SchemaArn: str,
         Name: str,
         AttributeUpdates: Sequence[FacetAttributeUpdateTypeDef] = ...,
         ObjectType: ObjectTypeType = ...
     ) -> Dict[str, Any]:
         """
-        Does the following * Adds new `Attributes` , `Rules` , or `ObjectTypes` .
+        Does the following: * Adds new `Attributes`, `Rules`, or `ObjectTypes`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_facet)
         """
 
     def update_link_attributes(
         self,
@@ -1021,15 +1021,15 @@
         DevelopmentSchemaArn: str,
         PublishedSchemaArn: str,
         MinorVersion: str,
         DryRun: bool = ...
     ) -> UpgradePublishedSchemaResponseTypeDef:
         """
         Upgrades a published schema under a new minor version revision using the current
-        contents of `DevelopmentSchemaArn` .
+        contents of `DevelopmentSchemaArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.upgrade_published_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#upgrade_published_schema)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/client.pyi` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         Retrieves metadata about a directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_directory)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_directory)
         """
     def get_facet(self, *, SchemaArn: str, Name: str) -> GetFacetResponseTypeDef:
         """
-        Gets details of the  Facet, such as facet name, attributes,  Rule s, or
+        Gets details of the  Facet, such as facet name, attributes,  Rules, or
         `ObjectType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_facet)
         """
     def get_link_attributes(
         self,
@@ -876,15 +876,15 @@
         *,
         SchemaArn: str,
         Name: str,
         AttributeUpdates: Sequence[FacetAttributeUpdateTypeDef] = ...,
         ObjectType: ObjectTypeType = ...
     ) -> Dict[str, Any]:
         """
-        Does the following * Adds new `Attributes` , `Rules` , or `ObjectTypes` .
+        Does the following: * Adds new `Attributes`, `Rules`, or `ObjectTypes`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_facet)
         """
     def update_link_attributes(
         self,
         *,
@@ -948,15 +948,15 @@
         DevelopmentSchemaArn: str,
         PublishedSchemaArn: str,
         MinorVersion: str,
         DryRun: bool = ...
     ) -> UpgradePublishedSchemaResponseTypeDef:
         """
         Upgrades a published schema under a new minor version revision using the current
-        contents of `DevelopmentSchemaArn` .
+        contents of `DevelopmentSchemaArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.upgrade_published_schema)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#upgrade_published_schema)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applied_schema_arns"]
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/literals.py` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/literals.py`

 * *Files 4% similar despite different names*

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

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/literals.pyi` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/literals.pyi`

 * *Files 4% similar despite different names*

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

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/paginator.py` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 
@@ -148,75 +148,75 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttachedIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 
 class ListDevelopmentSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevelopmentSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
         """
 
 
 class ListDirectoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
     """
 
     def paginate(
-        self, *, state: DirectoryStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, state: DirectoryStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDirectoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
         """
 
 
 class ListFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
         """
 
 
 class ListFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
         """
 
 
@@ -230,15 +230,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIncomingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 
@@ -251,30 +251,30 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIndexResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listindexpaginator)
         """
 
 
 class ListManagedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
         """
 
 
@@ -287,15 +287,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListObjectAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 
@@ -326,15 +326,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 
@@ -348,15 +348,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOutgoingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 
@@ -368,75 +368,75 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 
 class ListPublishedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPublishedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTypedLinkFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypedLinkFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
         """
 
 
 class ListTypedLinkFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypedLinkFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
         """
 
 
@@ -447,13 +447,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/paginator.pyi` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 class ListAttachedIndicesPaginator(Paginator):
@@ -144,71 +144,71 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttachedIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 class ListDevelopmentSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevelopmentSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
         """
 
 class ListDirectoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
     """
 
     def paginate(
-        self, *, state: DirectoryStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, state: DirectoryStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDirectoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listdirectoriespaginator)
         """
 
 class ListFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetattributespaginator)
         """
 
 class ListFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listfacetnamespaginator)
         """
 
 class ListIncomingTypedLinksPaginator(Paginator):
@@ -221,15 +221,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIncomingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 class ListIndexPaginator(Paginator):
@@ -241,29 +241,29 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIndexResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listindexpaginator)
         """
 
 class ListManagedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listmanagedschemaarnspaginator)
         """
 
 class ListObjectAttributesPaginator(Paginator):
@@ -275,15 +275,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListObjectAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 class ListObjectParentPathsPaginator(Paginator):
@@ -293,15 +293,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 class ListObjectPoliciesPaginator(Paginator):
@@ -312,15 +312,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 class ListOutgoingTypedLinksPaginator(Paginator):
@@ -333,15 +333,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOutgoingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 class ListPolicyAttachmentsPaginator(Paginator):
@@ -352,71 +352,71 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 class ListPublishedSchemaArnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPublishedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listpublishedschemaarnspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTypedLinkFacetAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypedLinkFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
         """
 
 class ListTypedLinkFacetNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypedLinkFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
         """
 
 class LookupPolicyPaginator(Paginator):
@@ -426,13 +426,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/type_defs.py` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ApplySchemaResponseTypeDef",
+    "AttachObjectResponseTypeDef",
+    "AttachToIndexResponseTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
     "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
@@ -54,49 +56,89 @@
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
+    "CreateDirectoryResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateObjectResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "CreateSchemaResponseTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
+    "DeleteDirectoryResponseTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
+    "DeleteSchemaResponseTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
+    "DetachFromIndexResponseTypeDef",
+    "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
+    "DisableDirectoryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
+    "EnableDirectoryResponseTypeDef",
     "RuleTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
+    "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
+    "GetSchemaAsJsonResponseTypeDef",
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     "ListAppliedSchemaArnsRequestRequestTypeDef",
+    "ListAppliedSchemaArnsResponseTypeDef",
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListDirectoriesRequestRequestTypeDef",
+    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetAttributesRequestRequestTypeDef",
+    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
     "ListFacetNamesRequestRequestTypeDef",
+    "ListFacetNamesResponseTypeDef",
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
     "ListManagedSchemaArnsRequestRequestTypeDef",
+    "ListManagedSchemaArnsResponseTypeDef",
+    "ListObjectChildrenResponseTypeDef",
+    "ListObjectPoliciesResponseTypeDef",
+    "ListPolicyAttachmentsResponseTypeDef",
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
+    "ListPublishedSchemaArnsResponseTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
+    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
+    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
+    "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
+    "PutSchemaFromJsonResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
+    "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
+    "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
+    "UpgradePublishedSchemaResponseTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
     "BatchAttachObjectTypeDef",
     "BatchAttachPolicyTypeDef",
     "BatchAttachToIndexTypeDef",
     "BatchDeleteObjectTypeDef",
@@ -112,61 +154,35 @@
     "BatchListPolicyAttachmentsTypeDef",
     "BatchLookupPolicyTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DetachFromIndexRequestRequestTypeDef",
     "DetachObjectRequestRequestTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "GetObjectInformationRequestRequestTypeDef",
+    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListAttachedIndicesRequestRequestTypeDef",
     "ListObjectChildrenRequestRequestTypeDef",
+    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     "ListObjectParentPathsRequestRequestTypeDef",
     "ListObjectParentsRequestRequestTypeDef",
+    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
+    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
+    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
     "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
+    "GetObjectInformationResponseTypeDef",
+    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
-    "ApplySchemaResponseTypeDef",
-    "AttachObjectResponseTypeDef",
-    "AttachToIndexResponseTypeDef",
-    "CreateDirectoryResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateObjectResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "DeleteDirectoryResponseTypeDef",
-    "DeleteSchemaResponseTypeDef",
-    "DetachFromIndexResponseTypeDef",
-    "DetachObjectResponseTypeDef",
-    "DisableDirectoryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnableDirectoryResponseTypeDef",
-    "GetAppliedSchemaVersionResponseTypeDef",
-    "GetObjectInformationResponseTypeDef",
-    "GetSchemaAsJsonResponseTypeDef",
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    "ListAppliedSchemaArnsResponseTypeDef",
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    "ListFacetNamesResponseTypeDef",
-    "ListManagedSchemaArnsResponseTypeDef",
-    "ListObjectChildrenResponseTypeDef",
-    "ListObjectPoliciesResponseTypeDef",
-    "ListPolicyAttachmentsResponseTypeDef",
-    "ListPublishedSchemaArnsResponseTypeDef",
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    "PublishSchemaResponseTypeDef",
-    "PutSchemaFromJsonResponseTypeDef",
-    "UpdateObjectAttributesResponseTypeDef",
-    "UpdateSchemaResponseTypeDef",
-    "UpgradeAppliedSchemaResponseTypeDef",
-    "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
@@ -175,30 +191,14 @@
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
-    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
     "AddFacetToObjectRequestRequestTypeDef",
     "BatchAddFacetToObjectTypeDef",
     "BatchCreateObjectTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
@@ -287,22 +287,36 @@
     "ApplySchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ApplySchemaResponseTypeDef = TypedDict(
+    "ApplySchemaResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AppliedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AttachObjectResponseTypeDef = TypedDict(
+    "AttachObjectResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AttachToIndexResponseTypeDef = TypedDict(
+    "AttachToIndexResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TypedLinkSchemaAndFacetNameTypeDef = TypedDict(
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
@@ -445,28 +459,71 @@
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
 
+CreateDirectoryResponseTypeDef = TypedDict(
+    "CreateDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "Name": str,
+        "ObjectIdentifier": str,
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateObjectResponseTypeDef = TypedDict(
+    "CreateObjectResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateSchemaRequestRequestTypeDef = TypedDict(
     "CreateSchemaRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
+DeleteDirectoryResponseTypeDef = TypedDict(
+    "DeleteDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFacetRequestRequestTypeDef = TypedDict(
     "DeleteFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -474,22 +531,46 @@
 DeleteSchemaRequestRequestTypeDef = TypedDict(
     "DeleteSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
+DetachFromIndexResponseTypeDef = TypedDict(
+    "DetachFromIndexResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DetachObjectResponseTypeDef = TypedDict(
+    "DetachObjectResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DirectoryTypeDef = TypedDict(
     "DirectoryTypeDef",
     {
         "Name": str,
         "DirectoryArn": str,
         "State": DirectoryStateType,
         "CreationDateTime": datetime,
@@ -500,21 +581,44 @@
 DisableDirectoryRequestRequestTypeDef = TypedDict(
     "DisableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
+DisableDirectoryResponseTypeDef = TypedDict(
+    "DisableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
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
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
+EnableDirectoryResponseTypeDef = TypedDict(
+    "EnableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
@@ -541,14 +645,22 @@
 GetAppliedSchemaVersionRequestRequestTypeDef = TypedDict(
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
+GetAppliedSchemaVersionResponseTypeDef = TypedDict(
+    "GetAppliedSchemaVersionResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDirectoryRequestRequestTypeDef = TypedDict(
     "GetDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
@@ -563,32 +675,62 @@
 GetSchemaAsJsonRequestRequestTypeDef = TypedDict(
     "GetSchemaAsJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
+GetSchemaAsJsonResponseTypeDef = TypedDict(
+    "GetSchemaAsJsonResponseTypeDef",
+    {
+        "Name": str,
+        "Document": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTypedLinkFacetInformationRequestRequestTypeDef = TypedDict(
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
+    "GetTypedLinkFacetInformationResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "IdentityAttributeOrder": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+    },
+)
+_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
+    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppliedSchemaArnsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 _OptionalListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
@@ -605,33 +747,91 @@
 class ListAppliedSchemaArnsRequestRequestTypeDef(
     _RequiredListAppliedSchemaArnsRequestRequestTypeDef,
     _OptionalListAppliedSchemaArnsRequestRequestTypeDef,
 ):
     pass
 
 
+ListAppliedSchemaArnsResponseTypeDef = TypedDict(
+    "ListAppliedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevelopmentSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    {
+        "state": DirectoryStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDirectoriesRequestRequestTypeDef = TypedDict(
     "ListDirectoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "state": DirectoryStateType,
     },
     total=False,
 )
 
+_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
+    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -648,14 +848,36 @@
 class ListFacetAttributesRequestRequestTypeDef(
     _RequiredListFacetAttributesRequestRequestTypeDef,
     _OptionalListFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
+    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListFacetNamesRequestRequestTypeDef = TypedDict(
@@ -670,34 +892,128 @@
 
 class ListFacetNamesRequestRequestTypeDef(
     _RequiredListFacetNamesRequestRequestTypeDef, _OptionalListFacetNamesRequestRequestTypeDef
 ):
     pass
 
 
+ListFacetNamesResponseTypeDef = TypedDict(
+    "ListFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListManagedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListManagedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListManagedSchemaArnsResponseTypeDef = TypedDict(
+    "ListManagedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListObjectChildrenResponseTypeDef = TypedDict(
+    "ListObjectChildrenResponseTypeDef",
+    {
+        "Children": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListObjectPoliciesResponseTypeDef = TypedDict(
+    "ListObjectPoliciesResponseTypeDef",
+    {
+        "AttachedPolicyIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPolicyAttachmentsResponseTypeDef = TypedDict(
+    "ListPolicyAttachmentsResponseTypeDef",
+    {
+        "ObjectIdentifiers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPublishedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListPublishedSchemaArnsResponseTypeDef = TypedDict(
+    "ListPublishedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -722,14 +1038,37 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
+    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -746,14 +1085,36 @@
 class ListTypedLinkFacetAttributesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
+    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
@@ -769,14 +1130,33 @@
 class ListTypedLinkFacetNamesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetNamesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetNamesRequestRequestTypeDef,
 ):
     pass
 
 
+ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
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
 PolicyAttachmentTypeDef = TypedDict(
     "PolicyAttachmentTypeDef",
     {
         "PolicyId": str,
         "ObjectIdentifier": str,
         "PolicyType": str,
     },
@@ -802,38 +1182,81 @@
 
 class PublishSchemaRequestRequestTypeDef(
     _RequiredPublishSchemaRequestRequestTypeDef, _OptionalPublishSchemaRequestRequestTypeDef
 ):
     pass
 
 
+PublishSchemaResponseTypeDef = TypedDict(
+    "PublishSchemaResponseTypeDef",
+    {
+        "PublishedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutSchemaFromJsonRequestRequestTypeDef = TypedDict(
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
+PutSchemaFromJsonResponseTypeDef = TypedDict(
+    "PutSchemaFromJsonResponseTypeDef",
+    {
+        "Arn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateObjectAttributesResponseTypeDef = TypedDict(
+    "UpdateObjectAttributesResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSchemaRequestRequestTypeDef = TypedDict(
     "UpdateSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpgradeAppliedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
@@ -849,14 +1272,23 @@
 class UpgradeAppliedSchemaRequestRequestTypeDef(
     _RequiredUpgradeAppliedSchemaRequestRequestTypeDef,
     _OptionalUpgradeAppliedSchemaRequestRequestTypeDef,
 ):
     pass
 
 
+UpgradeAppliedSchemaResponseTypeDef = TypedDict(
+    "UpgradeAppliedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpgradePublishedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DevelopmentSchemaArn": str,
         "PublishedSchemaArn": str,
         "MinorVersion": str,
     },
@@ -873,14 +1305,22 @@
 class UpgradePublishedSchemaRequestRequestTypeDef(
     _RequiredUpgradePublishedSchemaRequestRequestTypeDef,
     _OptionalUpgradePublishedSchemaRequestRequestTypeDef,
 ):
     pass
 
 
+UpgradePublishedSchemaResponseTypeDef = TypedDict(
+    "UpgradePublishedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttachObjectRequestRequestTypeDef = TypedDict(
     "AttachObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ParentReference": ObjectReferenceTypeDef,
         "ChildReference": ObjectReferenceTypeDef,
         "LinkName": str,
@@ -1190,14 +1630,38 @@
 class GetObjectInformationRequestRequestTypeDef(
     _RequiredGetObjectInformationRequestRequestTypeDef,
     _OptionalGetObjectInformationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "TargetReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
+    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAttachedIndicesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedIndicesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TargetReference": ObjectReferenceTypeDef,
     },
 )
@@ -1240,14 +1704,37 @@
 class ListObjectChildrenRequestRequestTypeDef(
     _RequiredListObjectChildrenRequestRequestTypeDef,
     _OptionalListObjectChildrenRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
+    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListObjectParentPathsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentPathsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1289,14 +1776,38 @@
 
 class ListObjectParentsRequestRequestTypeDef(
     _RequiredListObjectParentsRequestRequestTypeDef, _OptionalListObjectParentsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
+    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListObjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectPoliciesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1314,14 +1825,38 @@
 class ListObjectPoliciesRequestRequestTypeDef(
     _RequiredListObjectPoliciesRequestRequestTypeDef,
     _OptionalListObjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "PolicyReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
+    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPolicyAttachmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyAttachmentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
@@ -1339,14 +1874,37 @@
 class ListPolicyAttachmentsRequestRequestTypeDef(
     _RequiredListPolicyAttachmentsRequestRequestTypeDef,
     _OptionalListPolicyAttachmentsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class LookupPolicyRequestLookupPolicyPaginateTypeDef(
+    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
+    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
+):
+    pass
+
+
 _RequiredLookupPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredLookupPolicyRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1436,325 +1994,80 @@
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestRequestTypeDef",
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalListObjectAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestRequestTypeDef",
+_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
         "FacetFilter": SchemaFacetTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListObjectAttributesRequestRequestTypeDef(
-    _RequiredListObjectAttributesRequestRequestTypeDef,
-    _OptionalListObjectAttributesRequestRequestTypeDef,
+class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
+    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
 ):
     pass
 
 
-RemoveFacetFromObjectRequestRequestTypeDef = TypedDict(
-    "RemoveFacetFromObjectRequestRequestTypeDef",
+_RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-
-ApplySchemaResponseTypeDef = TypedDict(
-    "ApplySchemaResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachObjectResponseTypeDef = TypedDict(
-    "AttachObjectResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachToIndexResponseTypeDef = TypedDict(
-    "AttachToIndexResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDirectoryResponseTypeDef = TypedDict(
-    "CreateDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "Name": str,
-        "ObjectIdentifier": str,
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateObjectResponseTypeDef = TypedDict(
-    "CreateObjectResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDirectoryResponseTypeDef = TypedDict(
-    "DeleteDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachFromIndexResponseTypeDef = TypedDict(
-    "DetachFromIndexResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachObjectResponseTypeDef = TypedDict(
-    "DetachObjectResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableDirectoryResponseTypeDef = TypedDict(
-    "DisableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
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
-EnableDirectoryResponseTypeDef = TypedDict(
-    "EnableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppliedSchemaVersionResponseTypeDef = TypedDict(
-    "GetAppliedSchemaVersionResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaAsJsonResponseTypeDef = TypedDict(
-    "GetSchemaAsJsonResponseTypeDef",
-    {
-        "Name": str,
-        "Document": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    {
-        "IdentityAttributeOrder": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppliedSchemaArnsResponseTypeDef = TypedDict(
-    "ListAppliedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFacetNamesResponseTypeDef = TypedDict(
-    "ListFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListManagedSchemaArnsResponseTypeDef = TypedDict(
-    "ListManagedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListObjectChildrenResponseTypeDef = TypedDict(
-    "ListObjectChildrenResponseTypeDef",
-    {
-        "Children": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListObjectPoliciesResponseTypeDef = TypedDict(
-    "ListObjectPoliciesResponseTypeDef",
-    {
-        "AttachedPolicyIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPolicyAttachmentsResponseTypeDef = TypedDict(
-    "ListPolicyAttachmentsResponseTypeDef",
-    {
-        "ObjectIdentifiers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPublishedSchemaArnsResponseTypeDef = TypedDict(
-    "ListPublishedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetNamesResponseTypeDef",
+_OptionalListObjectAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestRequestTypeDef",
     {
-        "FacetNames": List[str],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishSchemaResponseTypeDef = TypedDict(
-    "PublishSchemaResponseTypeDef",
-    {
-        "PublishedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxResults": int,
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
     },
+    total=False,
 )
 
-PutSchemaFromJsonResponseTypeDef = TypedDict(
-    "PutSchemaFromJsonResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateObjectAttributesResponseTypeDef = TypedDict(
-    "UpdateObjectAttributesResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ListObjectAttributesRequestRequestTypeDef(
+    _RequiredListObjectAttributesRequestRequestTypeDef,
+    _OptionalListObjectAttributesRequestRequestTypeDef,
+):
+    pass
 
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpgradeAppliedSchemaResponseTypeDef = TypedDict(
-    "UpgradeAppliedSchemaResponseTypeDef",
+RemoveFacetFromObjectRequestRequestTypeDef = TypedDict(
+    "RemoveFacetFromObjectRequestRequestTypeDef",
     {
-        "UpgradedSchemaArn": str,
         "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpgradePublishedSchemaResponseTypeDef = TypedDict(
-    "UpgradePublishedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
@@ -1867,15 +2180,15 @@
 )
 
 ListObjectParentPathsResponseTypeDef = TypedDict(
     "ListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchListObjectParentsResponseTypeDef = TypedDict(
     "BatchListObjectParentsResponseTypeDef",
     {
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
@@ -1886,32 +2199,32 @@
 
 ListObjectParentsResponseTypeDef = TypedDict(
     "ListObjectParentsResponseTypeDef",
     {
         "Parents": Dict[str, str],
         "NextToken": str,
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDirectoryResponseTypeDef = TypedDict(
     "GetDirectoryResponseTypeDef",
     {
         "Directory": DirectoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDirectoriesResponseTypeDef = TypedDict(
     "ListDirectoriesResponseTypeDef",
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFacetAttributeDefinitionTypeDef = TypedDict(
     "_RequiredFacetAttributeDefinitionTypeDef",
     {
         "Type": FacetAttributeTypeType,
@@ -1959,337 +2272,24 @@
     pass
 
 
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-    },
-)
-_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
-    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "TargetReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
-    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-):
-    pass
-
-
-ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    {
-        "state": DirectoryStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
-    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
-    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
-):
-    pass
-
-
-ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
-    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
-    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
-    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "PolicyReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
-    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-):
-    pass
-
-
-ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
-    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
-    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class LookupPolicyRequestLookupPolicyPaginateTypeDef(
-    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
-    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
-):
-    pass
-
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -2411,23 +2411,23 @@
     pass
 
 
 GetLinkAttributesResponseTypeDef = TypedDict(
     "GetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetObjectAttributesResponseTypeDef = TypedDict(
     "GetObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IndexAttachmentTypeDef = TypedDict(
     "IndexAttachmentTypeDef",
     {
         "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
@@ -2437,15 +2437,15 @@
 )
 
 ListObjectAttributesResponseTypeDef = TypedDict(
     "ListObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachTypedLinkRequestRequestTypeDef = TypedDict(
     "AttachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
@@ -2546,15 +2546,15 @@
 
 
 ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
     "ListTypedLinkFacetAttributesResponseTypeDef",
     {
         "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
@@ -2581,15 +2581,15 @@
 )
 
 LookupPolicyResponseTypeDef = TypedDict(
     "LookupPolicyResponseTypeDef",
     {
         "PolicyToPathList": List[PolicyToPathTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchListAttachedIndicesResponseTypeDef = TypedDict(
     "BatchListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
@@ -2608,32 +2608,32 @@
 )
 
 ListAttachedIndicesResponseTypeDef = TypedDict(
     "ListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIndexResponseTypeDef = TypedDict(
     "ListIndexResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachTypedLinkResponseTypeDef = TypedDict(
     "AttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchAttachTypedLinkResponseTypeDef = TypedDict(
     "BatchAttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2706,24 +2706,24 @@
 
 
 ListIncomingTypedLinksResponseTypeDef = TypedDict(
     "ListIncomingTypedLinksResponseTypeDef",
     {
         "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOutgoingTypedLinksResponseTypeDef = TypedDict(
     "ListOutgoingTypedLinksResponseTypeDef",
     {
         "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2786,15 +2786,15 @@
     },
 )
 _OptionalListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_OptionalListIndexRequestListIndexPaginateTypeDef",
     {
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListIndexRequestListIndexPaginateTypeDef(
     _RequiredListIndexRequestListIndexPaginateTypeDef,
@@ -2885,15 +2885,15 @@
 )
 _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef(
     _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
@@ -2938,15 +2938,15 @@
 )
 _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef(
     _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
@@ -3016,15 +3016,15 @@
 )
 
 ListFacetAttributesResponseTypeDef = TypedDict(
     "ListFacetAttributesResponseTypeDef",
     {
         "Attributes": List[FacetAttributeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
@@ -3151,15 +3151,15 @@
     pass
 
 
 BatchWriteResponseTypeDef = TypedDict(
     "BatchWriteResponseTypeDef",
     {
         "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchReadOperationResponseTypeDef = TypedDict(
     "BatchReadOperationResponseTypeDef",
     {
         "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
@@ -3198,10 +3198,10 @@
     pass
 
 
 BatchReadResponseTypeDef = TypedDict(
     "BatchReadResponseTypeDef",
     {
         "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory/type_defs.pyi` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ApplySchemaResponseTypeDef",
+    "AttachObjectResponseTypeDef",
+    "AttachToIndexResponseTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
     "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
@@ -53,49 +55,89 @@
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
+    "CreateDirectoryResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateObjectResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "CreateSchemaResponseTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
+    "DeleteDirectoryResponseTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
+    "DeleteSchemaResponseTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
+    "DetachFromIndexResponseTypeDef",
+    "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
+    "DisableDirectoryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
+    "EnableDirectoryResponseTypeDef",
     "RuleTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
+    "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
+    "GetSchemaAsJsonResponseTypeDef",
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     "ListAppliedSchemaArnsRequestRequestTypeDef",
+    "ListAppliedSchemaArnsResponseTypeDef",
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListDirectoriesRequestRequestTypeDef",
+    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetAttributesRequestRequestTypeDef",
+    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
     "ListFacetNamesRequestRequestTypeDef",
+    "ListFacetNamesResponseTypeDef",
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
     "ListManagedSchemaArnsRequestRequestTypeDef",
+    "ListManagedSchemaArnsResponseTypeDef",
+    "ListObjectChildrenResponseTypeDef",
+    "ListObjectPoliciesResponseTypeDef",
+    "ListPolicyAttachmentsResponseTypeDef",
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
+    "ListPublishedSchemaArnsResponseTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
+    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
+    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
+    "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
+    "PutSchemaFromJsonResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
+    "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
+    "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
+    "UpgradePublishedSchemaResponseTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
     "BatchAttachObjectTypeDef",
     "BatchAttachPolicyTypeDef",
     "BatchAttachToIndexTypeDef",
     "BatchDeleteObjectTypeDef",
@@ -111,61 +153,35 @@
     "BatchListPolicyAttachmentsTypeDef",
     "BatchLookupPolicyTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DetachFromIndexRequestRequestTypeDef",
     "DetachObjectRequestRequestTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "GetObjectInformationRequestRequestTypeDef",
+    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListAttachedIndicesRequestRequestTypeDef",
     "ListObjectChildrenRequestRequestTypeDef",
+    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     "ListObjectParentPathsRequestRequestTypeDef",
     "ListObjectParentsRequestRequestTypeDef",
+    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
+    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
+    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
     "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
+    "GetObjectInformationResponseTypeDef",
+    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
-    "ApplySchemaResponseTypeDef",
-    "AttachObjectResponseTypeDef",
-    "AttachToIndexResponseTypeDef",
-    "CreateDirectoryResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateObjectResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "DeleteDirectoryResponseTypeDef",
-    "DeleteSchemaResponseTypeDef",
-    "DetachFromIndexResponseTypeDef",
-    "DetachObjectResponseTypeDef",
-    "DisableDirectoryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnableDirectoryResponseTypeDef",
-    "GetAppliedSchemaVersionResponseTypeDef",
-    "GetObjectInformationResponseTypeDef",
-    "GetSchemaAsJsonResponseTypeDef",
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    "ListAppliedSchemaArnsResponseTypeDef",
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    "ListFacetNamesResponseTypeDef",
-    "ListManagedSchemaArnsResponseTypeDef",
-    "ListObjectChildrenResponseTypeDef",
-    "ListObjectPoliciesResponseTypeDef",
-    "ListPolicyAttachmentsResponseTypeDef",
-    "ListPublishedSchemaArnsResponseTypeDef",
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    "PublishSchemaResponseTypeDef",
-    "PutSchemaFromJsonResponseTypeDef",
-    "UpdateObjectAttributesResponseTypeDef",
-    "UpdateSchemaResponseTypeDef",
-    "UpgradeAppliedSchemaResponseTypeDef",
-    "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
@@ -174,30 +190,14 @@
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
-    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
     "AddFacetToObjectRequestRequestTypeDef",
     "BatchAddFacetToObjectTypeDef",
     "BatchCreateObjectTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
@@ -286,22 +286,36 @@
     "ApplySchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ApplySchemaResponseTypeDef = TypedDict(
+    "ApplySchemaResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AppliedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AttachObjectResponseTypeDef = TypedDict(
+    "AttachObjectResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AttachToIndexResponseTypeDef = TypedDict(
+    "AttachToIndexResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TypedLinkSchemaAndFacetNameTypeDef = TypedDict(
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
@@ -444,28 +458,71 @@
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
 
+CreateDirectoryResponseTypeDef = TypedDict(
+    "CreateDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "Name": str,
+        "ObjectIdentifier": str,
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateObjectResponseTypeDef = TypedDict(
+    "CreateObjectResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateSchemaRequestRequestTypeDef = TypedDict(
     "CreateSchemaRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
+DeleteDirectoryResponseTypeDef = TypedDict(
+    "DeleteDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteFacetRequestRequestTypeDef = TypedDict(
     "DeleteFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -473,22 +530,46 @@
 DeleteSchemaRequestRequestTypeDef = TypedDict(
     "DeleteSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
+DetachFromIndexResponseTypeDef = TypedDict(
+    "DetachFromIndexResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DetachObjectResponseTypeDef = TypedDict(
+    "DetachObjectResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DirectoryTypeDef = TypedDict(
     "DirectoryTypeDef",
     {
         "Name": str,
         "DirectoryArn": str,
         "State": DirectoryStateType,
         "CreationDateTime": datetime,
@@ -499,21 +580,44 @@
 DisableDirectoryRequestRequestTypeDef = TypedDict(
     "DisableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
+DisableDirectoryResponseTypeDef = TypedDict(
+    "DisableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
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
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
+EnableDirectoryResponseTypeDef = TypedDict(
+    "EnableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
@@ -540,14 +644,22 @@
 GetAppliedSchemaVersionRequestRequestTypeDef = TypedDict(
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
+GetAppliedSchemaVersionResponseTypeDef = TypedDict(
+    "GetAppliedSchemaVersionResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDirectoryRequestRequestTypeDef = TypedDict(
     "GetDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
@@ -562,32 +674,60 @@
 GetSchemaAsJsonRequestRequestTypeDef = TypedDict(
     "GetSchemaAsJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
+GetSchemaAsJsonResponseTypeDef = TypedDict(
+    "GetSchemaAsJsonResponseTypeDef",
+    {
+        "Name": str,
+        "Document": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTypedLinkFacetInformationRequestRequestTypeDef = TypedDict(
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
+    "GetTypedLinkFacetInformationResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "IdentityAttributeOrder": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+    },
+)
+_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
+    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppliedSchemaArnsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 _OptionalListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
@@ -602,33 +742,89 @@
 
 class ListAppliedSchemaArnsRequestRequestTypeDef(
     _RequiredListAppliedSchemaArnsRequestRequestTypeDef,
     _OptionalListAppliedSchemaArnsRequestRequestTypeDef,
 ):
     pass
 
+ListAppliedSchemaArnsResponseTypeDef = TypedDict(
+    "ListAppliedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevelopmentSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    {
+        "state": DirectoryStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDirectoriesRequestRequestTypeDef = TypedDict(
     "ListDirectoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "state": DirectoryStateType,
     },
     total=False,
 )
 
+_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
+    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+):
+    pass
+
 _RequiredListFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -643,14 +839,34 @@
 
 class ListFacetAttributesRequestRequestTypeDef(
     _RequiredListFacetAttributesRequestRequestTypeDef,
     _OptionalListFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
+    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
+):
+    pass
+
 _RequiredListFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListFacetNamesRequestRequestTypeDef = TypedDict(
@@ -663,34 +879,126 @@
 )
 
 class ListFacetNamesRequestRequestTypeDef(
     _RequiredListFacetNamesRequestRequestTypeDef, _OptionalListFacetNamesRequestRequestTypeDef
 ):
     pass
 
+ListFacetNamesResponseTypeDef = TypedDict(
+    "ListFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListManagedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListManagedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListManagedSchemaArnsResponseTypeDef = TypedDict(
+    "ListManagedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListObjectChildrenResponseTypeDef = TypedDict(
+    "ListObjectChildrenResponseTypeDef",
+    {
+        "Children": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListObjectPoliciesResponseTypeDef = TypedDict(
+    "ListObjectPoliciesResponseTypeDef",
+    {
+        "AttachedPolicyIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPolicyAttachmentsResponseTypeDef = TypedDict(
+    "ListPolicyAttachmentsResponseTypeDef",
+    {
+        "ObjectIdentifiers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPublishedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListPublishedSchemaArnsResponseTypeDef = TypedDict(
+    "ListPublishedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -713,14 +1021,35 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
+    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+):
+    pass
+
 _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -735,14 +1064,34 @@
 
 class ListTypedLinkFacetAttributesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
+    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+):
+    pass
+
 _RequiredListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
@@ -756,14 +1105,33 @@
 
 class ListTypedLinkFacetNamesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetNamesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetNamesRequestRequestTypeDef,
 ):
     pass
 
+ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
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
 PolicyAttachmentTypeDef = TypedDict(
     "PolicyAttachmentTypeDef",
     {
         "PolicyId": str,
         "ObjectIdentifier": str,
         "PolicyType": str,
     },
@@ -787,38 +1155,81 @@
 )
 
 class PublishSchemaRequestRequestTypeDef(
     _RequiredPublishSchemaRequestRequestTypeDef, _OptionalPublishSchemaRequestRequestTypeDef
 ):
     pass
 
+PublishSchemaResponseTypeDef = TypedDict(
+    "PublishSchemaResponseTypeDef",
+    {
+        "PublishedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutSchemaFromJsonRequestRequestTypeDef = TypedDict(
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
+PutSchemaFromJsonResponseTypeDef = TypedDict(
+    "PutSchemaFromJsonResponseTypeDef",
+    {
+        "Arn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateObjectAttributesResponseTypeDef = TypedDict(
+    "UpdateObjectAttributesResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSchemaRequestRequestTypeDef = TypedDict(
     "UpdateSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpgradeAppliedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
@@ -832,14 +1243,23 @@
 
 class UpgradeAppliedSchemaRequestRequestTypeDef(
     _RequiredUpgradeAppliedSchemaRequestRequestTypeDef,
     _OptionalUpgradeAppliedSchemaRequestRequestTypeDef,
 ):
     pass
 
+UpgradeAppliedSchemaResponseTypeDef = TypedDict(
+    "UpgradeAppliedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpgradePublishedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DevelopmentSchemaArn": str,
         "PublishedSchemaArn": str,
         "MinorVersion": str,
     },
@@ -854,14 +1274,22 @@
 
 class UpgradePublishedSchemaRequestRequestTypeDef(
     _RequiredUpgradePublishedSchemaRequestRequestTypeDef,
     _OptionalUpgradePublishedSchemaRequestRequestTypeDef,
 ):
     pass
 
+UpgradePublishedSchemaResponseTypeDef = TypedDict(
+    "UpgradePublishedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttachObjectRequestRequestTypeDef = TypedDict(
     "AttachObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ParentReference": ObjectReferenceTypeDef,
         "ChildReference": ObjectReferenceTypeDef,
         "LinkName": str,
@@ -1153,14 +1581,36 @@
 
 class GetObjectInformationRequestRequestTypeDef(
     _RequiredGetObjectInformationRequestRequestTypeDef,
     _OptionalGetObjectInformationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "TargetReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
+    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+):
+    pass
+
 _RequiredListAttachedIndicesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedIndicesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TargetReference": ObjectReferenceTypeDef,
     },
 )
@@ -1199,14 +1649,35 @@
 
 class ListObjectChildrenRequestRequestTypeDef(
     _RequiredListObjectChildrenRequestRequestTypeDef,
     _OptionalListObjectChildrenRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
+    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+):
+    pass
+
 _RequiredListObjectParentPathsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentPathsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1244,14 +1715,36 @@
 )
 
 class ListObjectParentsRequestRequestTypeDef(
     _RequiredListObjectParentsRequestRequestTypeDef, _OptionalListObjectParentsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
+    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+):
+    pass
+
 _RequiredListObjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectPoliciesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1267,14 +1760,36 @@
 
 class ListObjectPoliciesRequestRequestTypeDef(
     _RequiredListObjectPoliciesRequestRequestTypeDef,
     _OptionalListObjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "PolicyReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
+    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPolicyAttachmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyAttachmentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
@@ -1290,14 +1805,35 @@
 
 class ListPolicyAttachmentsRequestRequestTypeDef(
     _RequiredListPolicyAttachmentsRequestRequestTypeDef,
     _OptionalListPolicyAttachmentsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class LookupPolicyRequestLookupPolicyPaginateTypeDef(
+    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
+    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
+):
+    pass
+
 _RequiredLookupPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredLookupPolicyRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1381,14 +1917,46 @@
 
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
+    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+):
+    pass
+
 _RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectAttributesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1414,293 +1982,14 @@
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
-ApplySchemaResponseTypeDef = TypedDict(
-    "ApplySchemaResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachObjectResponseTypeDef = TypedDict(
-    "AttachObjectResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachToIndexResponseTypeDef = TypedDict(
-    "AttachToIndexResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDirectoryResponseTypeDef = TypedDict(
-    "CreateDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "Name": str,
-        "ObjectIdentifier": str,
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateObjectResponseTypeDef = TypedDict(
-    "CreateObjectResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDirectoryResponseTypeDef = TypedDict(
-    "DeleteDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachFromIndexResponseTypeDef = TypedDict(
-    "DetachFromIndexResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachObjectResponseTypeDef = TypedDict(
-    "DetachObjectResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableDirectoryResponseTypeDef = TypedDict(
-    "DisableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
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
-EnableDirectoryResponseTypeDef = TypedDict(
-    "EnableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppliedSchemaVersionResponseTypeDef = TypedDict(
-    "GetAppliedSchemaVersionResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaAsJsonResponseTypeDef = TypedDict(
-    "GetSchemaAsJsonResponseTypeDef",
-    {
-        "Name": str,
-        "Document": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    {
-        "IdentityAttributeOrder": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppliedSchemaArnsResponseTypeDef = TypedDict(
-    "ListAppliedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFacetNamesResponseTypeDef = TypedDict(
-    "ListFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListManagedSchemaArnsResponseTypeDef = TypedDict(
-    "ListManagedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListObjectChildrenResponseTypeDef = TypedDict(
-    "ListObjectChildrenResponseTypeDef",
-    {
-        "Children": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListObjectPoliciesResponseTypeDef = TypedDict(
-    "ListObjectPoliciesResponseTypeDef",
-    {
-        "AttachedPolicyIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPolicyAttachmentsResponseTypeDef = TypedDict(
-    "ListPolicyAttachmentsResponseTypeDef",
-    {
-        "ObjectIdentifiers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPublishedSchemaArnsResponseTypeDef = TypedDict(
-    "ListPublishedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishSchemaResponseTypeDef = TypedDict(
-    "PublishSchemaResponseTypeDef",
-    {
-        "PublishedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSchemaFromJsonResponseTypeDef = TypedDict(
-    "PutSchemaFromJsonResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateObjectAttributesResponseTypeDef = TypedDict(
-    "UpdateObjectAttributesResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpgradeAppliedSchemaResponseTypeDef = TypedDict(
-    "UpgradeAppliedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpgradePublishedSchemaResponseTypeDef = TypedDict(
-    "UpgradePublishedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
         "IsUnique": bool,
     },
 )
@@ -1804,15 +2093,15 @@
 )
 
 ListObjectParentPathsResponseTypeDef = TypedDict(
     "ListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchListObjectParentsResponseTypeDef = TypedDict(
     "BatchListObjectParentsResponseTypeDef",
     {
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
@@ -1823,32 +2112,32 @@
 
 ListObjectParentsResponseTypeDef = TypedDict(
     "ListObjectParentsResponseTypeDef",
     {
         "Parents": Dict[str, str],
         "NextToken": str,
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDirectoryResponseTypeDef = TypedDict(
     "GetDirectoryResponseTypeDef",
     {
         "Directory": DirectoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDirectoriesResponseTypeDef = TypedDict(
     "ListDirectoriesResponseTypeDef",
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFacetAttributeDefinitionTypeDef = TypedDict(
     "_RequiredFacetAttributeDefinitionTypeDef",
     {
         "Type": FacetAttributeTypeType,
@@ -1892,313 +2181,24 @@
 ):
     pass
 
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-    },
-)
-_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
-    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-):
-    pass
-
-_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "TargetReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
-    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-):
-    pass
-
-ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    {
-        "state": DirectoryStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
-    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-):
-    pass
-
-_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
-    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
-):
-    pass
-
-ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
-    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-):
-    pass
-
-_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
-    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-):
-    pass
-
-_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
-    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-):
-    pass
-
-_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "PolicyReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
-    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-):
-    pass
-
-ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
-    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-):
-    pass
-
-_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
-    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-):
-    pass
-
-_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class LookupPolicyRequestLookupPolicyPaginateTypeDef(
-    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
-    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
-):
-    pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -2314,23 +2314,23 @@
 ):
     pass
 
 GetLinkAttributesResponseTypeDef = TypedDict(
     "GetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetObjectAttributesResponseTypeDef = TypedDict(
     "GetObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IndexAttachmentTypeDef = TypedDict(
     "IndexAttachmentTypeDef",
     {
         "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
@@ -2340,15 +2340,15 @@
 )
 
 ListObjectAttributesResponseTypeDef = TypedDict(
     "ListObjectAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachTypedLinkRequestRequestTypeDef = TypedDict(
     "AttachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
@@ -2445,15 +2445,15 @@
     pass
 
 ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
     "ListTypedLinkFacetAttributesResponseTypeDef",
     {
         "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
@@ -2480,15 +2480,15 @@
 )
 
 LookupPolicyResponseTypeDef = TypedDict(
     "LookupPolicyResponseTypeDef",
     {
         "PolicyToPathList": List[PolicyToPathTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchListAttachedIndicesResponseTypeDef = TypedDict(
     "BatchListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
@@ -2507,32 +2507,32 @@
 )
 
 ListAttachedIndicesResponseTypeDef = TypedDict(
     "ListAttachedIndicesResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIndexResponseTypeDef = TypedDict(
     "ListIndexResponseTypeDef",
     {
         "IndexAttachments": List[IndexAttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachTypedLinkResponseTypeDef = TypedDict(
     "AttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchAttachTypedLinkResponseTypeDef = TypedDict(
     "BatchAttachTypedLinkResponseTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2603,24 +2603,24 @@
     pass
 
 ListIncomingTypedLinksResponseTypeDef = TypedDict(
     "ListIncomingTypedLinksResponseTypeDef",
     {
         "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOutgoingTypedLinksResponseTypeDef = TypedDict(
     "ListOutgoingTypedLinksResponseTypeDef",
     {
         "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2681,15 +2681,15 @@
     },
 )
 _OptionalListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_OptionalListIndexRequestListIndexPaginateTypeDef",
     {
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListIndexRequestListIndexPaginateTypeDef(
     _RequiredListIndexRequestListIndexPaginateTypeDef,
     _OptionalListIndexRequestListIndexPaginateTypeDef,
@@ -2772,15 +2772,15 @@
 )
 _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef(
     _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
@@ -2821,15 +2821,15 @@
 )
 _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef(
     _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
@@ -2893,15 +2893,15 @@
 )
 
 ListFacetAttributesResponseTypeDef = TypedDict(
     "ListFacetAttributesResponseTypeDef",
     {
         "Attributes": List[FacetAttributeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
@@ -3026,15 +3026,15 @@
 ):
     pass
 
 BatchWriteResponseTypeDef = TypedDict(
     "BatchWriteResponseTypeDef",
     {
         "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchReadOperationResponseTypeDef = TypedDict(
     "BatchReadOperationResponseTypeDef",
     {
         "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
@@ -3071,10 +3071,10 @@
 ):
     pass
 
 BatchReadResponseTypeDef = TypedDict(
     "BatchReadResponseTypeDef",
     {
         "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/PKG-INFO` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.26.60
-Summary: Type annotations for boto3.CloudDirectory 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudDirectory 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-clouddirectory"></a>
 
 # mypy-boto3-clouddirectory
 
 [![PyPI - mypy-boto3-clouddirectory](https://img.shields.io/pypi/v/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-clouddirectory?color=blue)](https://pypistats.org/packages/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -419,15 +419,17 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
@@ -437,49 +439,89 @@
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
     CreateDirectoryRequestRequestTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
+    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
+    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
+    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
+    EnableDirectoryResponseTypeDef,
     RuleTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
+    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -495,61 +537,35 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
     BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
+    GetObjectInformationResponseTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    DeleteDirectoryResponseTypeDef,
-    DeleteSchemaResponseTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableDirectoryResponseTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
-    GetObjectInformationResponseTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    PublishSchemaResponseTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
@@ -558,30 +574,14 @@
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
     AddFacetToObjectRequestRequestTypeDef,
     BatchAddFacetToObjectTypeDef,
     BatchCreateObjectTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
@@ -657,42 +657,42 @@
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

### Comparing `mypy-boto3-clouddirectory-1.26.60/mypy_boto3_clouddirectory.egg-info/SOURCES.txt` & `mypy-boto3-clouddirectory-1.27.0/mypy_boto3_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.26.60/setup.py` & `mypy-boto3-clouddirectory-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-clouddirectory.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-clouddirectory",
-    version="1.26.60",
+    version="1.27.0",
     packages=["mypy_boto3_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudDirectory 1.26.60 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.CloudDirectory 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/",
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


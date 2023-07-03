# Comparing `tmp/mypy-boto3-efs-1.26.72.tar.gz` & `tmp/mypy-boto3-efs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-efs-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
+gzip compressed data, was "mypy-boto3-efs-1.27.0.tar", last modified: Mon Jul  3 19:50:43 2023, max compression
```

## Comparing `mypy-boto3-efs-1.26.72.tar` & `mypy-boto3-efs-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/mypy_boto3_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-02-15 22:27:06.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-15 22:27:56.000000 mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.842126 mypy-boto3-efs-1.26.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-15 22:27:05.000000 mypy-boto3-efs-1.26.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.135190 mypy-boto3-efs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-03 19:50:43.135190 mypy-boto3-efs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14219 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.123190 mypy-boto3-efs-1.27.0/mypy_boto3_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-07-03 19:37:05.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-07-03 19:37:05.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-03 19:37:06.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-03 19:37:05.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 19:37:05.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-03 19:37:05.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-07-03 19:37:06.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-07-03 19:37:06.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.135190 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-03 19:50:42.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:42.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:42.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:42.000000 mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:43.135190 mypy-boto3-efs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:04.000000 mypy-boto3-efs-1.27.0/setup.py
```

### Comparing `mypy-boto3-efs-1.26.72/LICENSE` & `mypy-boto3-efs-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-efs-1.26.72/PKG-INFO` & `mypy-boto3-efs-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.26.72
-Summary: Type annotations for boto3.EFS 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EFS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-efs"></a>
 
 # mypy-boto3-efs
 
 [![PyPI - mypy-boto3-efs](https://img.shields.io/pypi/v/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,15 +339,14 @@
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
@@ -356,49 +355,50 @@
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
+    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
+    MountTargetDescriptionResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
     ReplicationConfigurationDescriptionResponseMetadataTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
     FileSystemDescriptionResponseMetadataTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
@@ -418,42 +418,42 @@
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

### Comparing `mypy-boto3-efs-1.26.72/README.md` & `mypy-boto3-efs-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-efs"></a>
 
 # mypy-boto3-efs
 
 [![PyPI - mypy-boto3-efs](https://img.shields.io/pypi/v/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,15 +307,14 @@
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
@@ -324,49 +323,50 @@
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
+    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
+    MountTargetDescriptionResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
     ReplicationConfigurationDescriptionResponseMetadataTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
     FileSystemDescriptionResponseMetadataTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
@@ -386,42 +386,42 @@
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

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.py` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/__init__.pyi` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/__main__.py` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EFS 1.26.72\nVersion:         1.26.72\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.EFS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.72")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.py` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/client.pyi` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.py` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeFileSystemsPaginatorName",
     "DescribeMountTargetsPaginatorName",
     "DescribeTagsPaginatorName",
     "LifeCycleStateType",
     "PerformanceModeType",
     "ReplicationStatusType",
@@ -35,21 +34,20 @@
     "EFSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeFileSystemsPaginatorName = Literal["describe_file_systems"]
 DescribeMountTargetsPaginatorName = Literal["describe_mount_targets"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
 LifeCycleStateType = Literal["available", "creating", "deleted", "deleting", "error", "updating"]
 PerformanceModeType = Literal["generalPurpose", "maxIO"]
-ReplicationStatusType = Literal["DELETING", "ENABLED", "ENABLING", "ERROR"]
+ReplicationStatusType = Literal["DELETING", "ENABLED", "ENABLING", "ERROR", "PAUSED", "PAUSING"]
 ResourceIdTypeType = Literal["LONG_ID", "SHORT_ID"]
 ResourceType = Literal["FILE_SYSTEM", "MOUNT_TARGET"]
 StatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING"]
 ThroughputModeType = Literal["bursting", "elastic", "provisioned"]
 TransitionToIARulesType = Literal[
     "AFTER_14_DAYS",
     "AFTER_1_DAY",
@@ -71,14 +69,15 @@
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
@@ -118,14 +117,15 @@
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
@@ -204,14 +204,15 @@
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
@@ -222,14 +223,15 @@
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
@@ -265,14 +267,15 @@
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
@@ -291,16 +294,19 @@
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
@@ -380,18 +386,21 @@
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
@@ -417,17 +426,19 @@
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
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/literals.pyi` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/literals.py`

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
     "DescribeFileSystemsPaginatorName",
     "DescribeMountTargetsPaginatorName",
     "DescribeTagsPaginatorName",
     "LifeCycleStateType",
     "PerformanceModeType",
     "ReplicationStatusType",
@@ -34,20 +35,21 @@
     "EFSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeFileSystemsPaginatorName = Literal["describe_file_systems"]
 DescribeMountTargetsPaginatorName = Literal["describe_mount_targets"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
 LifeCycleStateType = Literal["available", "creating", "deleted", "deleting", "error", "updating"]
 PerformanceModeType = Literal["generalPurpose", "maxIO"]
-ReplicationStatusType = Literal["DELETING", "ENABLED", "ENABLING", "ERROR"]
+ReplicationStatusType = Literal["DELETING", "ENABLED", "ENABLING", "ERROR", "PAUSED", "PAUSING"]
 ResourceIdTypeType = Literal["LONG_ID", "SHORT_ID"]
 ResourceType = Literal["FILE_SYSTEM", "MOUNT_TARGET"]
 StatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING"]
 ThroughputModeType = Literal["bursting", "elastic", "provisioned"]
 TransitionToIARulesType = Literal[
     "AFTER_14_DAYS",
     "AFTER_1_DAY",
@@ -69,14 +71,15 @@
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
@@ -116,14 +119,15 @@
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
@@ -202,14 +206,15 @@
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
@@ -220,14 +225,15 @@
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
@@ -263,14 +269,15 @@
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
@@ -289,16 +296,19 @@
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
@@ -378,18 +388,21 @@
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
@@ -415,17 +428,19 @@
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
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.py` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describefilesystemspaginator)
         """
 
 
@@ -74,28 +74,28 @@
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describemounttargetspaginator)
         """
 
 
 class DescribeTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
-        self, *, FileSystemId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FileSystemId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
         """
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/paginator.pyi` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describefilesystemspaginator)
         """
 
 class DescribeMountTargetsPaginator(Paginator):
@@ -70,27 +70,27 @@
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describemounttargetspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
-        self, *, FileSystemId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FileSystemId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/paginators/#describetagspaginator)
         """
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.py` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "PosixUserTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "BackupPolicyTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
@@ -51,49 +50,50 @@
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DescribeAccessPointsRequestRequestTypeDef",
     "DescribeAccountPreferencesRequestRequestTypeDef",
     "ResourceIdPreferenceTypeDef",
     "DescribeBackupPolicyRequestRequestTypeDef",
     "DescribeFileSystemPolicyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
     "DescribeLifecycleConfigurationRequestRequestTypeDef",
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeMountTargetsRequestRequestTypeDef",
     "MountTargetDescriptionTypeDef",
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
+    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
+    "FileSystemPolicyDescriptionTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
+    "MountTargetDescriptionResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FileSystemPolicyDescriptionTypeDef",
-    "MountTargetDescriptionResponseMetadataTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeMountTargetsResponseTypeDef",
     "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
     "FileSystemDescriptionResponseMetadataTypeDef",
     "FileSystemDescriptionTypeDef",
     "LifecycleConfigurationDescriptionTypeDef",
     "PutLifecycleConfigurationRequestRequestTypeDef",
@@ -121,25 +121,14 @@
 )
 
 
 class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
 
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -275,20 +264,20 @@
 DescribeFileSystemPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CreationToken": str,
+        "FileSystemId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
@@ -310,14 +299,33 @@
 DescribeMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 
+DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+        "MountTargetId": str,
+        "AccessPointId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMountTargetsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "Marker": str,
         "FileSystemId": str,
         "MountTargetId": str,
@@ -361,14 +369,36 @@
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+    },
+)
+_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeTagsRequestDescribeTagsPaginateTypeDef(
+    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
+    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -404,14 +434,21 @@
 )
 
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFileSystemSizeTypeDef = TypedDict(
     "_RequiredFileSystemSizeTypeDef",
     {
         "Value": int,
     },
 )
 _OptionalFileSystemSizeTypeDef = TypedDict(
@@ -425,14 +462,23 @@
 )
 
 
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
 
+FileSystemPolicyDescriptionTypeDef = TypedDict(
+    "FileSystemPolicyDescriptionTypeDef",
+    {
+        "FileSystemId": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -479,14 +525,41 @@
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
 
+MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
+    "MountTargetDescriptionResponseMetadataTypeDef",
+    {
+        "OwnerId": str,
+        "MountTargetId": str,
+        "FileSystemId": str,
+        "SubnetId": str,
+        "LifeCycleState": LifeCycleStateType,
+        "IpAddress": str,
+        "NetworkInterfaceId": str,
+        "AvailabilityZoneId": str,
+        "AvailabilityZoneName": str,
+        "VpcId": str,
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
 PutAccountPreferencesRequestRequestTypeDef = TypedDict(
     "PutAccountPreferencesRequestRequestTypeDef",
     {
         "ResourceIdType": ResourceIdTypeType,
     },
 )
 
@@ -509,14 +582,25 @@
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
 ):
     pass
 
 
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
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -539,55 +623,14 @@
 
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
 
-DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    {
-        "SecurityGroups": List[str],
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
-FileSystemPolicyDescriptionTypeDef = TypedDict(
-    "FileSystemPolicyDescriptionTypeDef",
-    {
-        "FileSystemId": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    {
-        "OwnerId": str,
-        "MountTargetId": str,
-        "FileSystemId": str,
-        "SubnetId": str,
-        "LifeCycleState": LifeCycleStateType,
-        "IpAddress": str,
-        "NetworkInterfaceId": str,
-        "AvailabilityZoneId": str,
-        "AvailabilityZoneName": str,
-        "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
     },
 )
 _OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
@@ -622,24 +665,24 @@
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "Marker": str,
         "Tags": List[TagTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
         "ResourceId": str,
@@ -647,15 +690,15 @@
     },
 )
 
 BackupPolicyDescriptionTypeDef = TypedDict(
     "BackupPolicyDescriptionTypeDef",
     {
         "BackupPolicy": BackupPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBackupPolicyRequestRequestTypeDef = TypedDict(
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -681,89 +724,46 @@
 )
 
 DescribeAccountPreferencesResponseTypeDef = TypedDict(
     "DescribeAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountPreferencesResponseTypeDef = TypedDict(
     "PutAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    {
-        "CreationToken": str,
-        "FileSystemId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-        "MountTargetId": str,
-        "AccessPointId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-    },
-)
-_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeTagsRequestDescribeTagsPaginateTypeDef(
-    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
-    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
-):
-    pass
-
-
 DescribeMountTargetsResponseTypeDef = TypedDict(
     "DescribeMountTargetsResponseTypeDef",
     {
         "Marker": str,
         "MountTargets": List[MountTargetDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationConfigurationDescriptionResponseMetadataTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
     {
         "SourceFileSystemId": str,
         "SourceFileSystemRegion": str,
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationConfigurationDescriptionTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionTypeDef",
     {
         "SourceFileSystemId": str,
@@ -791,15 +791,15 @@
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
         "OwnerId": str,
@@ -835,15 +835,15 @@
     pass
 
 
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
         "LifecyclePolicies": List[LifecyclePolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -860,15 +860,15 @@
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
         "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
@@ -910,29 +910,29 @@
 
 
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileSystemsResponseTypeDef = TypedDict(
     "DescribeFileSystemsResponseTypeDef",
     {
         "Marker": str,
         "FileSystems": List[FileSystemDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccessPointsResponseTypeDef = TypedDict(
     "DescribeAccessPointsResponseTypeDef",
     {
         "AccessPoints": List[AccessPointDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs/type_defs.pyi` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "PosixUserTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "BackupPolicyTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
@@ -50,49 +49,50 @@
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DescribeAccessPointsRequestRequestTypeDef",
     "DescribeAccountPreferencesRequestRequestTypeDef",
     "ResourceIdPreferenceTypeDef",
     "DescribeBackupPolicyRequestRequestTypeDef",
     "DescribeFileSystemPolicyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
     "DescribeLifecycleConfigurationRequestRequestTypeDef",
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeMountTargetsRequestRequestTypeDef",
     "MountTargetDescriptionTypeDef",
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
+    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
+    "FileSystemPolicyDescriptionTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
+    "MountTargetDescriptionResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FileSystemPolicyDescriptionTypeDef",
-    "MountTargetDescriptionResponseMetadataTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeMountTargetsResponseTypeDef",
     "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
     "FileSystemDescriptionResponseMetadataTypeDef",
     "FileSystemDescriptionTypeDef",
     "LifecycleConfigurationDescriptionTypeDef",
     "PutLifecycleConfigurationRequestRequestTypeDef",
@@ -118,25 +118,14 @@
     },
     total=False,
 )
 
 class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
     pass
 
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -270,20 +259,20 @@
 DescribeFileSystemPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CreationToken": str,
+        "FileSystemId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
@@ -305,14 +294,33 @@
 DescribeMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 
+DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+        "MountTargetId": str,
+        "AccessPointId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMountTargetsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "Marker": str,
         "FileSystemId": str,
         "MountTargetId": str,
@@ -354,14 +362,34 @@
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+    },
+)
+_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeTagsRequestDescribeTagsPaginateTypeDef(
+    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
+    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -393,14 +421,21 @@
     },
     total=False,
 )
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFileSystemSizeTypeDef = TypedDict(
     "_RequiredFileSystemSizeTypeDef",
     {
         "Value": int,
     },
 )
 _OptionalFileSystemSizeTypeDef = TypedDict(
@@ -412,14 +447,23 @@
     },
     total=False,
 )
 
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
+FileSystemPolicyDescriptionTypeDef = TypedDict(
+    "FileSystemPolicyDescriptionTypeDef",
+    {
+        "FileSystemId": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -462,14 +506,41 @@
 
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
+MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
+    "MountTargetDescriptionResponseMetadataTypeDef",
+    {
+        "OwnerId": str,
+        "MountTargetId": str,
+        "FileSystemId": str,
+        "SubnetId": str,
+        "LifeCycleState": LifeCycleStateType,
+        "IpAddress": str,
+        "NetworkInterfaceId": str,
+        "AvailabilityZoneId": str,
+        "AvailabilityZoneName": str,
+        "VpcId": str,
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
 PutAccountPreferencesRequestRequestTypeDef = TypedDict(
     "PutAccountPreferencesRequestRequestTypeDef",
     {
         "ResourceIdType": ResourceIdTypeType,
     },
 )
 
@@ -490,14 +561,25 @@
 
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
 ):
     pass
 
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
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -518,55 +600,14 @@
 )
 
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
-DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    {
-        "SecurityGroups": List[str],
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
-FileSystemPolicyDescriptionTypeDef = TypedDict(
-    "FileSystemPolicyDescriptionTypeDef",
-    {
-        "FileSystemId": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    {
-        "OwnerId": str,
-        "MountTargetId": str,
-        "FileSystemId": str,
-        "SubnetId": str,
-        "LifeCycleState": LifeCycleStateType,
-        "IpAddress": str,
-        "NetworkInterfaceId": str,
-        "AvailabilityZoneId": str,
-        "AvailabilityZoneName": str,
-        "VpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
     },
 )
 _OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
@@ -599,24 +640,24 @@
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "Marker": str,
         "Tags": List[TagTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
         "ResourceId": str,
@@ -624,15 +665,15 @@
     },
 )
 
 BackupPolicyDescriptionTypeDef = TypedDict(
     "BackupPolicyDescriptionTypeDef",
     {
         "BackupPolicy": BackupPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBackupPolicyRequestRequestTypeDef = TypedDict(
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -658,87 +699,46 @@
 )
 
 DescribeAccountPreferencesResponseTypeDef = TypedDict(
     "DescribeAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountPreferencesResponseTypeDef = TypedDict(
     "PutAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    {
-        "CreationToken": str,
-        "FileSystemId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-        "MountTargetId": str,
-        "AccessPointId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "FileSystemId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeTagsRequestDescribeTagsPaginateTypeDef(
-    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
-    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
-):
-    pass
 
 DescribeMountTargetsResponseTypeDef = TypedDict(
     "DescribeMountTargetsResponseTypeDef",
     {
         "Marker": str,
         "MountTargets": List[MountTargetDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationConfigurationDescriptionResponseMetadataTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
     {
         "SourceFileSystemId": str,
         "SourceFileSystemRegion": str,
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationConfigurationDescriptionTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionTypeDef",
     {
         "SourceFileSystemId": str,
@@ -766,15 +766,15 @@
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
         "OwnerId": str,
@@ -808,15 +808,15 @@
 ):
     pass
 
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
         "LifecyclePolicies": List[LifecyclePolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -833,15 +833,15 @@
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
         "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
@@ -881,29 +881,29 @@
     pass
 
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileSystemsResponseTypeDef = TypedDict(
     "DescribeFileSystemsResponseTypeDef",
     {
         "Marker": str,
         "FileSystems": List[FileSystemDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccessPointsResponseTypeDef = TypedDict(
     "DescribeAccessPointsResponseTypeDef",
     {
         "AccessPoints": List[AccessPointDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/PKG-INFO` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.26.72
-Summary: Type annotations for boto3.EFS 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EFS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-efs"></a>
 
 # mypy-boto3-efs
 
 [![PyPI - mypy-boto3-efs](https://img.shields.io/pypi/v/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-efs?color=blue)](https://pypistats.org/packages/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,15 +339,14 @@
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
@@ -356,49 +355,50 @@
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
+    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
+    MountTargetDescriptionResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
     ReplicationConfigurationDescriptionResponseMetadataTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
     FileSystemDescriptionResponseMetadataTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
@@ -418,42 +418,42 @@
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

### Comparing `mypy-boto3-efs-1.26.72/mypy_boto3_efs.egg-info/SOURCES.txt` & `mypy-boto3-efs-1.27.0/mypy_boto3_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.26.72/setup.py` & `mypy-boto3-efs-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-efs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-efs",
-    version="1.26.72",
+    version="1.27.0",
     packages=["mypy_boto3_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EFS 1.26.72 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.EFS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/",
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


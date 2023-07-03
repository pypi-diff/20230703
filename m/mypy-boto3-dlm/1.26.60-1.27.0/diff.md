# Comparing `tmp/mypy-boto3-dlm-1.26.60.tar.gz` & `tmp/mypy-boto3-dlm-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dlm-1.26.60.tar", last modified: Mon Jan 30 21:06:23 2023, max compression
+gzip compressed data, was "mypy-boto3-dlm-1.27.0.tar", last modified: Mon Jul  3 19:50:40 2023, max compression
```

## Comparing `mypy-boto3-dlm-1.26.60.tar` & `mypy-boto3-dlm-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.522471 mypy-boto3-dlm-1.26.60/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-01-30 21:06:23.522471 mypy-boto3-dlm-1.26.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.522471 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.522471 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-01-30 21:06:23.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-30 21:06:23.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 21:06:23.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-30 21:06:23.000000 mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:06:23.522471 mypy-boto3-dlm-1.26.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-30 21:05:19.000000 mypy-boto3-dlm-1.26.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.203137 mypy-boto3-dlm-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-03 19:50:40.199137 mypy-boto3-dlm-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.199137 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.199137 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:40.203137 mypy-boto3-dlm-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/setup.py
```

### Comparing `mypy-boto3-dlm-1.26.60/LICENSE` & `mypy-boto3-dlm-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-dlm-1.26.60/PKG-INFO` & `mypy-boto3-dlm-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.26.60
-Summary: Type annotations for boto3.DLM 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.DLM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dlm"></a>
 
 # mypy-boto3-dlm
 
 [![PyPI - mypy-boto3-dlm](https://img.shields.io/pypi/v/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dlm?color=blue)](https://pypistats.org/packages/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,35 +306,35 @@
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
     CreateRuleTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
     DeprecateRuleTypeDef,
     EventParametersTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     RetainRuleTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArchiveRetainRuleTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
     CrossRegionCopyRuleTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     ParametersTypeDef,
     ArchiveRuleTypeDef,
     ActionTypeDef,
@@ -354,42 +354,42 @@
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

### Comparing `mypy-boto3-dlm-1.26.60/README.md` & `mypy-boto3-dlm-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dlm"></a>
 
 # mypy-boto3-dlm
 
 [![PyPI - mypy-boto3-dlm](https://img.shields.io/pypi/v/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dlm?color=blue)](https://pypistats.org/packages/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,35 +274,35 @@
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
     CreateRuleTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
     DeprecateRuleTypeDef,
     EventParametersTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     RetainRuleTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArchiveRetainRuleTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
     CrossRegionCopyRuleTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     ParametersTypeDef,
     ArchiveRuleTypeDef,
     ActionTypeDef,
@@ -322,42 +322,42 @@
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

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/client.py` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/client.pyi` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/literals.py` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -98,21 +99,23 @@
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
@@ -191,14 +194,15 @@
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
@@ -209,14 +213,15 @@
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
@@ -252,14 +257,15 @@
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
@@ -278,16 +284,19 @@
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
@@ -367,18 +376,21 @@
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
@@ -409,16 +421,18 @@
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
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

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/literals.pyi` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -96,21 +97,23 @@
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
@@ -189,14 +192,15 @@
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
@@ -207,14 +211,15 @@
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
@@ -250,14 +255,15 @@
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
@@ -276,16 +282,19 @@
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
@@ -365,18 +374,21 @@
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
@@ -407,16 +419,18 @@
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
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

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/type_defs.py` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,35 +33,35 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "RetentionArchiveTierTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateLifecyclePolicyResponseTypeDef",
     "CreateRuleTypeDef",
     "CrossRegionCopyRetainRuleTypeDef",
     "EncryptionConfigurationTypeDef",
     "CrossRegionCopyDeprecateRuleTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
     "DeprecateRuleTypeDef",
     "EventParametersTypeDef",
     "FastRestoreRuleTypeDef",
     "GetLifecyclePoliciesRequestRequestTypeDef",
     "LifecyclePolicySummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "RetainRuleTypeDef",
     "ShareRuleTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArchiveRetainRuleTypeDef",
-    "CreateLifecyclePolicyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CrossRegionCopyActionTypeDef",
     "CrossRegionCopyRuleTypeDef",
     "EventSourceTypeDef",
     "GetLifecyclePoliciesResponseTypeDef",
     "ParametersTypeDef",
     "ArchiveRuleTypeDef",
     "ActionTypeDef",
@@ -79,22 +79,19 @@
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLifecyclePolicyResponseTypeDef = TypedDict(
+    "CreateLifecyclePolicyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PolicyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleTypeDef = TypedDict(
     "CreateRuleTypeDef",
     {
         "Location": LocationValuesType,
@@ -226,22 +223,41 @@
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 RetainRuleTypeDef = TypedDict(
     "RetainRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
@@ -287,30 +303,14 @@
 ArchiveRetainRuleTypeDef = TypedDict(
     "ArchiveRetainRuleTypeDef",
     {
         "RetentionArchiveTier": RetentionArchiveTierTypeDef,
     },
 )
 
-CreateLifecyclePolicyResponseTypeDef = TypedDict(
-    "CreateLifecyclePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
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
 _RequiredCrossRegionCopyActionTypeDef = TypedDict(
     "_RequiredCrossRegionCopyActionTypeDef",
     {
         "Target": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
@@ -374,15 +374,15 @@
     pass
 
 
 GetLifecyclePoliciesResponseTypeDef = TypedDict(
     "GetLifecyclePoliciesResponseTypeDef",
     {
         "Policies": List[LifecyclePolicySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ParametersTypeDef = TypedDict(
     "ParametersTypeDef",
     {
         "ExcludeBootVolume": bool,
@@ -507,10 +507,10 @@
     pass
 
 
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "Policy": LifecyclePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm/type_defs.pyi` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,35 +32,35 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "RetentionArchiveTierTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateLifecyclePolicyResponseTypeDef",
     "CreateRuleTypeDef",
     "CrossRegionCopyRetainRuleTypeDef",
     "EncryptionConfigurationTypeDef",
     "CrossRegionCopyDeprecateRuleTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
     "DeprecateRuleTypeDef",
     "EventParametersTypeDef",
     "FastRestoreRuleTypeDef",
     "GetLifecyclePoliciesRequestRequestTypeDef",
     "LifecyclePolicySummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "RetainRuleTypeDef",
     "ShareRuleTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArchiveRetainRuleTypeDef",
-    "CreateLifecyclePolicyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CrossRegionCopyActionTypeDef",
     "CrossRegionCopyRuleTypeDef",
     "EventSourceTypeDef",
     "GetLifecyclePoliciesResponseTypeDef",
     "ParametersTypeDef",
     "ArchiveRuleTypeDef",
     "ActionTypeDef",
@@ -78,22 +78,19 @@
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateLifecyclePolicyResponseTypeDef = TypedDict(
+    "CreateLifecyclePolicyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PolicyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleTypeDef = TypedDict(
     "CreateRuleTypeDef",
     {
         "Location": LocationValuesType,
@@ -221,22 +218,41 @@
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 RetainRuleTypeDef = TypedDict(
     "RetainRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
@@ -280,30 +296,14 @@
 ArchiveRetainRuleTypeDef = TypedDict(
     "ArchiveRetainRuleTypeDef",
     {
         "RetentionArchiveTier": RetentionArchiveTierTypeDef,
     },
 )
 
-CreateLifecyclePolicyResponseTypeDef = TypedDict(
-    "CreateLifecyclePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
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
 _RequiredCrossRegionCopyActionTypeDef = TypedDict(
     "_RequiredCrossRegionCopyActionTypeDef",
     {
         "Target": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
@@ -361,15 +361,15 @@
 class EventSourceTypeDef(_RequiredEventSourceTypeDef, _OptionalEventSourceTypeDef):
     pass
 
 GetLifecyclePoliciesResponseTypeDef = TypedDict(
     "GetLifecyclePoliciesResponseTypeDef",
     {
         "Policies": List[LifecyclePolicySummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ParametersTypeDef = TypedDict(
     "ParametersTypeDef",
     {
         "ExcludeBootVolume": bool,
@@ -490,10 +490,10 @@
 ):
     pass
 
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "Policy": LifecyclePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/PKG-INFO` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.26.60
-Summary: Type annotations for boto3.DLM 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.DLM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dlm"></a>
 
 # mypy-boto3-dlm
 
 [![PyPI - mypy-boto3-dlm](https://img.shields.io/pypi/v/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dlm?color=blue)](https://pypistats.org/packages/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,35 +306,35 @@
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
-    ResponseMetadataTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
     CreateRuleTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
     DeprecateRuleTypeDef,
     EventParametersTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     RetainRuleTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArchiveRetainRuleTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
     CrossRegionCopyRuleTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     ParametersTypeDef,
     ArchiveRuleTypeDef,
     ActionTypeDef,
@@ -354,42 +354,42 @@
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

### Comparing `mypy-boto3-dlm-1.26.60/mypy_boto3_dlm.egg-info/SOURCES.txt` & `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.26.60/setup.py` & `mypy-boto3-dlm-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-dlm.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dlm",
-    version="1.26.60",
+    version="1.27.0",
     packages=["mypy_boto3_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DLM 1.26.60 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.DLM 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/",
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


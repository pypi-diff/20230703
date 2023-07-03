# Comparing `tmp/mypy-boto3-translate-1.26.31.tar.gz` & `tmp/mypy-boto3-translate-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-translate-1.26.31.tar", last modified: Thu Dec 15 20:33:07 2022, max compression
+gzip compressed data, was "mypy-boto3-translate-1.27.0.tar", last modified: Mon Jul  3 19:51:34 2023, max compression
```

## Comparing `mypy-boto3-translate-1.26.31.tar` & `mypy-boto3-translate-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/mypy_boto3_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15931 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2022-12-15 20:32:56.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2022-12-15 20:32:56.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2022-12-15 20:32:57.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2022-12-15 20:32:56.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.652116 mypy-boto3-translate-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-03 19:51:34.652116 mypy-boto3-translate-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.652116 mypy-boto3-translate-1.27.0/mypy_boto3_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20137 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.652116 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-03 19:51:34.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:34.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:34.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:34.000000 mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:34.652116 mypy-boto3-translate-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:49:16.000000 mypy-boto3-translate-1.27.0/setup.py
```

### Comparing `mypy-boto3-translate-1.26.31/LICENSE` & `mypy-boto3-translate-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-translate-1.26.31/PKG-INFO` & `mypy-boto3-translate-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.26.31
-Summary: Type annotations for boto3.Translate 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.Translate 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,54 +334,58 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
+    DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
+    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
@@ -398,42 +402,42 @@
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

### Comparing `mypy-boto3-translate-1.26.31/README.md` & `mypy-boto3-translate-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,54 +302,58 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
+    DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
+    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
@@ -366,42 +370,42 @@
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

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.py` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.pyi` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/__main__.py` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Translate 1.26.31\nVersion:         1.26.31\nBuilder version:"
-        " 7.12.0\nDocs:           "
+        "Type annotations for boto3.Translate 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.31")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.py` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from .literals import DisplayLanguageCodeType, TerminologyDataFormatType
 from .paginator import ListTerminologiesPaginator
 from .type_defs import (
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataResponseTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
+    DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionKeyTypeDef,
     GetParallelDataResponseTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     InputDataConfigTypeDef,
     ListLanguagesResponseTypeDef,
@@ -38,14 +39,15 @@
     OutputDataConfigTypeDef,
     ParallelDataConfigTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     TagTypeDef,
     TerminologyDataTypeDef,
     TextTranslationJobFilterTypeDef,
+    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     TranslationSettingsTypeDef,
     UpdateParallelDataResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -302,14 +304,30 @@
         """
         Associates a specific tag with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#tag_resource)
         """
 
+    def translate_document(
+        self,
+        *,
+        Document: DocumentTypeDef,
+        SourceLanguageCode: str,
+        TargetLanguageCode: str,
+        TerminologyNames: Sequence[str] = ...,
+        Settings: TranslationSettingsTypeDef = ...
+    ) -> TranslateDocumentResponseTypeDef:
+        """
+        Translates the input document from the source language to the target language.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_document)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#translate_document)
+        """
+
     def translate_text(
         self,
         *,
         Text: str,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.pyi` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from .literals import DisplayLanguageCodeType, TerminologyDataFormatType
 from .paginator import ListTerminologiesPaginator
 from .type_defs import (
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataResponseTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
+    DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionKeyTypeDef,
     GetParallelDataResponseTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     InputDataConfigTypeDef,
     ListLanguagesResponseTypeDef,
@@ -38,14 +39,15 @@
     OutputDataConfigTypeDef,
     ParallelDataConfigTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     TagTypeDef,
     TerminologyDataTypeDef,
     TextTranslationJobFilterTypeDef,
+    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     TranslationSettingsTypeDef,
     UpdateParallelDataResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -279,14 +281,29 @@
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Associates a specific tag with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#tag_resource)
         """
+    def translate_document(
+        self,
+        *,
+        Document: DocumentTypeDef,
+        SourceLanguageCode: str,
+        TargetLanguageCode: str,
+        TerminologyNames: Sequence[str] = ...,
+        Settings: TranslationSettingsTypeDef = ...
+    ) -> TranslateDocumentResponseTypeDef:
+        """
+        Translates the input document from the source language to the target language.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_document)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#translate_document)
+        """
     def translate_text(
         self,
         *,
         Text: str,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.py` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -98,31 +99,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -201,14 +205,15 @@
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
@@ -219,34 +224,38 @@
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
@@ -259,14 +268,15 @@
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
@@ -285,16 +295,19 @@
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
@@ -374,18 +387,21 @@
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

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.pyi` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -96,31 +97,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -199,14 +203,15 @@
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
@@ -217,34 +222,38 @@
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
@@ -257,14 +266,15 @@
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
@@ -283,16 +293,19 @@
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
@@ -372,18 +385,21 @@
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

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.py` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListTerminologiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.pyi` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListTerminologiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTerminologiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/paginators/#listterminologiespaginator)
         """
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.py` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,54 +38,58 @@
 
 
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
+    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
+    "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
+    "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
     "TerminologyPropertiesTypeDef",
     "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateParallelDataResponseTypeDef",
-    "DeleteParallelDataResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
-    "UpdateParallelDataResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
+    "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
+    "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
     "ImportTerminologyResponseTypeDef",
     "ListTerminologiesResponseTypeDef",
     "GetParallelDataResponseTypeDef",
@@ -123,46 +127,68 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeTextTranslationJobRequestRequestTypeDef = TypedDict(
     "DescribeTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DocumentTypeDef = TypedDict(
+    "DocumentTypeDef",
+    {
+        "Content": Union[str, bytes, IO[Any], StreamingBody],
+        "ContentType": str,
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
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -271,20 +297,18 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTerminologiesRequestRequestTypeDef = TypedDict(
     "ListTerminologiesRequestRequestTypeDef",
     {
@@ -301,38 +325,95 @@
         "JobStatus": JobStatusType,
         "SubmittedBeforeTime": Union[datetime, str],
         "SubmittedAfterTime": Union[datetime, str],
     },
     total=False,
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
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TranslatedDocumentTypeDef = TypedDict(
+    "TranslatedDocumentTypeDef",
+    {
+        "Content": bytes,
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
 
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
     total=False,
@@ -448,81 +529,27 @@
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
@@ -549,36 +576,52 @@
 
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredTranslateDocumentRequestRequestTypeDef",
+    {
+        "Document": DocumentTypeDef,
+        "SourceLanguageCode": str,
+        "TargetLanguageCode": str,
+    },
+)
+_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalTranslateDocumentRequestRequestTypeDef",
+    {
+        "TerminologyNames": Sequence[str],
+        "Settings": TranslationSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class TranslateDocumentRequestRequestTypeDef(
+    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -595,23 +638,35 @@
 
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
 
+TranslateDocumentResponseTypeDef = TypedDict(
+    "TranslateDocumentResponseTypeDef",
+    {
+        "TranslatedDocument": TranslatedDocumentTypeDef,
+        "SourceLanguageCode": str,
+        "TargetLanguageCode": str,
+        "AppliedTerminologies": List[AppliedTerminologyTypeDef],
+        "AppliedSettings": TranslationSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
@@ -665,65 +720,65 @@
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.pyi` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -37,54 +37,58 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
+    "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
+    "DocumentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
+    "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
+    "StopTextTranslationJobResponseTypeDef",
+    "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
     "TerminologyPropertiesTypeDef",
     "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateParallelDataResponseTypeDef",
-    "DeleteParallelDataResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartTextTranslationJobResponseTypeDef",
-    "StopTextTranslationJobResponseTypeDef",
-    "UpdateParallelDataResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
+    "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
+    "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
     "ImportTerminologyResponseTypeDef",
     "ListTerminologiesResponseTypeDef",
     "GetParallelDataResponseTypeDef",
@@ -122,46 +126,68 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateParallelDataResponseTypeDef = TypedDict(
+    "CreateParallelDataResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteParallelDataRequestRequestTypeDef = TypedDict(
     "DeleteParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteParallelDataResponseTypeDef = TypedDict(
+    "DeleteParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTerminologyRequestRequestTypeDef = TypedDict(
     "DeleteTerminologyRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeTextTranslationJobRequestRequestTypeDef = TypedDict(
     "DescribeTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DocumentTypeDef = TypedDict(
+    "DocumentTypeDef",
+    {
+        "Content": Union[str, bytes, IO[Any], StreamingBody],
+        "ContentType": str,
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
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -266,20 +292,18 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
+    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListTerminologiesRequestRequestTypeDef = TypedDict(
     "ListTerminologiesRequestRequestTypeDef",
     {
@@ -296,38 +320,95 @@
         "JobStatus": JobStatusType,
         "SubmittedBeforeTime": Union[datetime, str],
         "SubmittedAfterTime": Union[datetime, str],
     },
     total=False,
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
 TranslationSettingsTypeDef = TypedDict(
     "TranslationSettingsTypeDef",
     {
         "Formality": FormalityType,
         "Profanity": Literal["MASK"],
     },
     total=False,
 )
 
+StartTextTranslationJobResponseTypeDef = TypedDict(
+    "StartTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopTextTranslationJobResponseTypeDef = TypedDict(
+    "StopTextTranslationJobResponseTypeDef",
+    {
+        "JobId": str,
+        "JobStatus": JobStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TranslatedDocumentTypeDef = TypedDict(
+    "TranslatedDocumentTypeDef",
+    {
+        "Content": bytes,
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
 
+UpdateParallelDataResponseTypeDef = TypedDict(
+    "UpdateParallelDataResponseTypeDef",
+    {
+        "Name": str,
+        "Status": ParallelDataStatusType,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
     total=False,
@@ -437,81 +518,27 @@
 
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateParallelDataResponseTypeDef = TypedDict(
-    "CreateParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteParallelDataResponseTypeDef = TypedDict(
-    "DeleteParallelDataResponseTypeDef",
-    {
-        "Name": str,
-        "Status": ParallelDataStatusType,
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTextTranslationJobResponseTypeDef = TypedDict(
-    "StartTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StopTextTranslationJobResponseTypeDef = TypedDict(
-    "StopTextTranslationJobResponseTypeDef",
-    {
-        "JobId": str,
-        "JobStatus": JobStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateParallelDataResponseTypeDef = TypedDict(
-    "UpdateParallelDataResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Name": str,
-        "Status": ParallelDataStatusType,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
@@ -536,36 +563,50 @@
 
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
-    "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_RequiredTranslateDocumentRequestRequestTypeDef",
+    {
+        "Document": DocumentTypeDef,
+        "SourceLanguageCode": str,
+        "TargetLanguageCode": str,
+    },
+)
+_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
+    "_OptionalTranslateDocumentRequestRequestTypeDef",
+    {
+        "TerminologyNames": Sequence[str],
+        "Settings": TranslationSettingsTypeDef,
+    },
+    total=False,
+)
+
+class TranslateDocumentRequestRequestTypeDef(
+    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
+):
+    pass
+
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -580,23 +621,35 @@
 )
 
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
+TranslateDocumentResponseTypeDef = TypedDict(
+    "TranslateDocumentResponseTypeDef",
+    {
+        "TranslatedDocument": TranslatedDocumentTypeDef,
+        "SourceLanguageCode": str,
+        "TargetLanguageCode": str,
+        "AppliedTerminologies": List[AppliedTerminologyTypeDef],
+        "AppliedSettings": TranslationSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
         "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
@@ -648,65 +701,65 @@
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTerminologyResponseTypeDef = TypedDict(
     "ImportTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "AuxiliaryDataLocation": TerminologyDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTerminologiesResponseTypeDef = TypedDict(
     "ListTerminologiesResponseTypeDef",
     {
         "TerminologyPropertiesList": List[TerminologyPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetParallelDataResponseTypeDef = TypedDict(
     "GetParallelDataResponseTypeDef",
     {
         "ParallelDataProperties": ParallelDataPropertiesTypeDef,
         "DataLocation": ParallelDataDataLocationTypeDef,
         "AuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
         "LatestUpdateAttemptAuxiliaryDataLocation": ParallelDataDataLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListParallelDataResponseTypeDef = TypedDict(
     "ListParallelDataResponseTypeDef",
     {
         "ParallelDataPropertiesList": List[ParallelDataPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTextTranslationJobResponseTypeDef = TypedDict(
     "DescribeTextTranslationJobResponseTypeDef",
     {
         "TextTranslationJobProperties": TextTranslationJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTextTranslationJobsResponseTypeDef = TypedDict(
     "ListTextTranslationJobsResponseTypeDef",
     {
         "TextTranslationJobPropertiesList": List[TextTranslationJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/PKG-INFO` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.26.31
-Summary: Type annotations for boto3.Translate 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.Translate 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,54 +334,58 @@
 
 ```python
 from mypy_boto3_translate.type_defs import (
     TermTypeDef,
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
+    DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
+    DocumentTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
+    StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
+    StopTextTranslationJobResponseTypeDef,
+    TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateParallelDataResponseTypeDef,
-    DeleteParallelDataResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartTextTranslationJobResponseTypeDef,
-    StopTextTranslationJobResponseTypeDef,
-    UpdateParallelDataResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
-    ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
+    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
@@ -398,42 +402,42 @@
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

### Comparing `mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/SOURCES.txt` & `mypy-boto3-translate-1.27.0/mypy_boto3_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.31/setup.py` & `mypy-boto3-translate-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-translate.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-translate",
-    version="1.26.31",
+    version="1.27.0",
     packages=["mypy_boto3_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Translate 1.26.31 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.Translate 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/",
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


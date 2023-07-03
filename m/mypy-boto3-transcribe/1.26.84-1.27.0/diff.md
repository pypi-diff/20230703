# Comparing `tmp/mypy-boto3-transcribe-1.26.84.tar.gz` & `tmp/mypy-boto3-transcribe-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transcribe-1.26.84.tar", last modified: Fri Mar  3 20:27:52 2023, max compression
+gzip compressed data, was "mypy-boto3-transcribe-1.27.0.tar", last modified: Mon Jul  3 19:51:34 2023, max compression
```

## Comparing `mypy-boto3-transcribe-1.26.84.tar` & `mypy-boto3-transcribe-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.686264 mypy-boto3-transcribe-1.26.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-03-03 20:27:52.686264 mypy-boto3-transcribe-1.26.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.674264 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29715 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29669 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-03-03 20:27:43.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39133 2023-03-03 20:27:43.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39102 2023-03-03 20:27:43.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-03 20:27:42.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.678264 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-03-03 20:27:52.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-03 20:27:52.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-03 20:27:52.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-03 20:27:52.000000 mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 20:27:52.686264 mypy-boto3-transcribe-1.26.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-03 20:27:41.000000 mypy-boto3-transcribe-1.26.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.308111 mypy-boto3-transcribe-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-03 19:51:34.308111 mypy-boto3-transcribe-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15165 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.300110 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29715 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29669 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39193 2023-07-03 19:49:12.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39162 2023-07-03 19:49:12.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:09.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.308111 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-03 19:51:34.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 19:51:34.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:34.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:34.000000 mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:34.308111 mypy-boto3-transcribe-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 19:49:08.000000 mypy-boto3-transcribe-1.27.0/setup.py
```

### Comparing `mypy-boto3-transcribe-1.26.84/LICENSE` & `mypy-boto3-transcribe-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-transcribe-1.26.84/PKG-INFO` & `mypy-boto3-transcribe-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.26.84
-Summary: Type annotations for boto3.TranscribeService 1.26.84 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.TranscribeService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,33 +324,39 @@
     AbsoluteTimeRangeTypeDef,
     ContentRedactionTypeDef,
     LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
     ChannelDefinitionTypeDef,
     MediaTypeDef,
     TranscriptTypeDef,
-    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
+    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    GetVocabularyResponseTypeDef,
     RelativeTimeRangeTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
@@ -361,33 +367,27 @@
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
     MedicalTranscriptTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
+    ResponseMetadataTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     SubtitlesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CallAnalyticsJobSettingsTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
-    GetVocabularyFilterResponseTypeDef,
-    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
-    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -434,42 +434,42 @@
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

### Comparing `mypy-boto3-transcribe-1.26.84/README.md` & `mypy-boto3-transcribe-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,33 +292,39 @@
     AbsoluteTimeRangeTypeDef,
     ContentRedactionTypeDef,
     LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
     ChannelDefinitionTypeDef,
     MediaTypeDef,
     TranscriptTypeDef,
-    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
+    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    GetVocabularyResponseTypeDef,
     RelativeTimeRangeTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
@@ -329,33 +335,27 @@
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
     MedicalTranscriptTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
+    ResponseMetadataTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     SubtitlesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CallAnalyticsJobSettingsTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
-    GetVocabularyFilterResponseTypeDef,
-    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
-    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -402,42 +402,42 @@
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

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/__main__.py` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TranscribeService 1.26.84\nVersion:         1.26.84\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.TranscribeService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.84")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/client.py` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/client.pyi` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/literals.py` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
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
@@ -181,14 +182,15 @@
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
@@ -286,14 +288,15 @@
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
@@ -329,14 +332,15 @@
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
@@ -355,16 +359,19 @@
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
@@ -448,15 +455,17 @@
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

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/literals.pyi` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
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
@@ -179,14 +180,15 @@
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
@@ -284,14 +286,15 @@
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
@@ -327,14 +330,15 @@
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
@@ -353,16 +357,19 @@
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
@@ -446,15 +453,17 @@
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

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/type_defs.py` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,33 +49,39 @@
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionTypeDef",
     "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
-    "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
+    "CreateMedicalVocabularyResponseTypeDef",
+    "CreateVocabularyFilterResponseTypeDef",
+    "CreateVocabularyResponseTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
     "DescribeLanguageModelRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
+    "GetMedicalVocabularyResponseTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
+    "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyRequestRequestTypeDef",
+    "GetVocabularyResponseTypeDef",
     "RelativeTimeRangeTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
@@ -86,33 +92,27 @@
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
+    "ResponseMetadataTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
     "SubtitlesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
+    "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
+    "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
+    "UpdateVocabularyResponseTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
-    "CreateMedicalVocabularyResponseTypeDef",
-    "CreateVocabularyFilterResponseTypeDef",
-    "CreateVocabularyResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetMedicalVocabularyResponseTypeDef",
-    "GetVocabularyFilterResponseTypeDef",
-    "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
-    "UpdateMedicalVocabularyResponseTypeDef",
-    "UpdateVocabularyFilterResponseTypeDef",
-    "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelResponseTypeDef",
     "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -229,25 +229,14 @@
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
     total=False,
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
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -268,14 +257,48 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateMedicalVocabularyResponseTypeDef = TypedDict(
+    "CreateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateVocabularyFilterResponseTypeDef = TypedDict(
+    "CreateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -331,14 +354,21 @@
 DescribeLanguageModelRequestRequestTypeDef = TypedDict(
     "DescribeLanguageModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -359,35 +389,72 @@
 GetMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "GetMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+GetMedicalVocabularyResponseTypeDef = TypedDict(
+    "GetMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTranscriptionJobRequestRequestTypeDef = TypedDict(
     "GetTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
     },
 )
 
 GetVocabularyFilterRequestRequestTypeDef = TypedDict(
     "GetVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 
+GetVocabularyFilterResponseTypeDef = TypedDict(
+    "GetVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "DownloadUri": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+GetVocabularyResponseTypeDef = TypedDict(
+    "GetVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
@@ -569,14 +636,25 @@
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
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
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -620,14 +698,25 @@
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
 )
 
+UpdateMedicalVocabularyResponseTypeDef = TypedDict(
+    "UpdateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 _OptionalUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
@@ -644,14 +733,24 @@
 class UpdateVocabularyFilterRequestRequestTypeDef(
     _RequiredUpdateVocabularyFilterRequestRequestTypeDef,
     _OptionalUpdateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateVocabularyFilterResponseTypeDef = TypedDict(
+    "UpdateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -668,157 +767,58 @@
 
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-CallAnalyticsJobSettingsTypeDef = TypedDict(
-    "CallAnalyticsJobSettingsTypeDef",
-    {
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "LanguageModelName": str,
-        "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
-    },
-    total=False,
-)
-
-CreateMedicalVocabularyResponseTypeDef = TypedDict(
-    "CreateMedicalVocabularyResponseTypeDef",
+UpdateVocabularyResponseTypeDef = TypedDict(
+    "UpdateVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVocabularyFilterResponseTypeDef = TypedDict(
-    "CreateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
         "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMedicalVocabularyResponseTypeDef = TypedDict(
-    "GetMedicalVocabularyResponseTypeDef",
+CallAnalyticsJobSettingsTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetVocabularyFilterResponseTypeDef = TypedDict(
-    "GetVocabularyFilterResponseTypeDef",
-    {
         "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "DownloadUri": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetVocabularyResponseTypeDef = TypedDict(
-    "GetVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "ContentRedaction": ContentRedactionTypeDef,
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
+    total=False,
 )
 
 ListCallAnalyticsJobsResponseTypeDef = TypedDict(
     "ListCallAnalyticsJobsResponseTypeDef",
     {
         "Status": CallAnalyticsJobStatusType,
         "NextToken": str,
         "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMedicalVocabularyResponseTypeDef = TypedDict(
-    "UpdateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateVocabularyFilterResponseTypeDef = TypedDict(
-    "UpdateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateVocabularyResponseTypeDef = TypedDict(
-    "UpdateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLanguageModelResponseTypeDef = TypedDict(
     "CreateLanguageModelResponseTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "ModelStatus": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LanguageModelTypeDef = TypedDict(
     "LanguageModelTypeDef",
     {
         "ModelName": str,
@@ -935,15 +935,15 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1021,44 +1021,44 @@
 
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MedicalTranscriptionJobTypeDef = TypedDict(
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
@@ -1254,24 +1254,24 @@
     pass
 
 
 DescribeLanguageModelResponseTypeDef = TypedDict(
     "DescribeLanguageModelResponseTypeDef",
     {
         "LanguageModel": LanguageModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
@@ -1282,65 +1282,65 @@
     total=False,
 )
 
 GetMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "GetMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "StartMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartCallAnalyticsJobResponseTypeDef = TypedDict(
     "StartCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
@@ -1398,35 +1398,35 @@
     pass
 
 
 CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "CreateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "GetCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesResponseTypeDef",
     {
         "NextToken": str,
         "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "UpdateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe/type_defs.pyi` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,33 +48,39 @@
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionTypeDef",
     "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
-    "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
+    "CreateMedicalVocabularyResponseTypeDef",
+    "CreateVocabularyFilterResponseTypeDef",
+    "CreateVocabularyResponseTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
     "DescribeLanguageModelRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
+    "GetMedicalVocabularyResponseTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
+    "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyRequestRequestTypeDef",
+    "GetVocabularyResponseTypeDef",
     "RelativeTimeRangeTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
@@ -85,33 +91,27 @@
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
+    "ResponseMetadataTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
     "SubtitlesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
+    "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
+    "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
+    "UpdateVocabularyResponseTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
-    "CreateMedicalVocabularyResponseTypeDef",
-    "CreateVocabularyFilterResponseTypeDef",
-    "CreateVocabularyResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetMedicalVocabularyResponseTypeDef",
-    "GetVocabularyFilterResponseTypeDef",
-    "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
-    "UpdateMedicalVocabularyResponseTypeDef",
-    "UpdateVocabularyFilterResponseTypeDef",
-    "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelResponseTypeDef",
     "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -226,25 +226,14 @@
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
     total=False,
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
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -263,14 +252,48 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateMedicalVocabularyResponseTypeDef = TypedDict(
+    "CreateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateVocabularyFilterResponseTypeDef = TypedDict(
+    "CreateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -326,14 +349,21 @@
 DescribeLanguageModelRequestRequestTypeDef = TypedDict(
     "DescribeLanguageModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -354,35 +384,72 @@
 GetMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "GetMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+GetMedicalVocabularyResponseTypeDef = TypedDict(
+    "GetMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTranscriptionJobRequestRequestTypeDef = TypedDict(
     "GetTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
     },
 )
 
 GetVocabularyFilterRequestRequestTypeDef = TypedDict(
     "GetVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 
+GetVocabularyFilterResponseTypeDef = TypedDict(
+    "GetVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "DownloadUri": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+GetVocabularyResponseTypeDef = TypedDict(
+    "GetVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
@@ -564,14 +631,25 @@
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
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
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -615,14 +693,25 @@
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
 )
 
+UpdateMedicalVocabularyResponseTypeDef = TypedDict(
+    "UpdateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 _OptionalUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
@@ -637,14 +726,24 @@
 
 class UpdateVocabularyFilterRequestRequestTypeDef(
     _RequiredUpdateVocabularyFilterRequestRequestTypeDef,
     _OptionalUpdateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
+UpdateVocabularyFilterResponseTypeDef = TypedDict(
+    "UpdateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -659,157 +758,58 @@
 )
 
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
-CallAnalyticsJobSettingsTypeDef = TypedDict(
-    "CallAnalyticsJobSettingsTypeDef",
-    {
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "LanguageModelName": str,
-        "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
-    },
-    total=False,
-)
-
-CreateMedicalVocabularyResponseTypeDef = TypedDict(
-    "CreateMedicalVocabularyResponseTypeDef",
+UpdateVocabularyResponseTypeDef = TypedDict(
+    "UpdateVocabularyResponseTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
         "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVocabularyFilterResponseTypeDef = TypedDict(
-    "CreateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
         "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMedicalVocabularyResponseTypeDef = TypedDict(
-    "GetMedicalVocabularyResponseTypeDef",
+CallAnalyticsJobSettingsTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetVocabularyFilterResponseTypeDef = TypedDict(
-    "GetVocabularyFilterResponseTypeDef",
-    {
         "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "DownloadUri": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetVocabularyResponseTypeDef = TypedDict(
-    "GetVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "ContentRedaction": ContentRedactionTypeDef,
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
+    total=False,
 )
 
 ListCallAnalyticsJobsResponseTypeDef = TypedDict(
     "ListCallAnalyticsJobsResponseTypeDef",
     {
         "Status": CallAnalyticsJobStatusType,
         "NextToken": str,
         "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMedicalVocabularyResponseTypeDef = TypedDict(
-    "UpdateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateVocabularyFilterResponseTypeDef = TypedDict(
-    "UpdateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateVocabularyResponseTypeDef = TypedDict(
-    "UpdateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLanguageModelResponseTypeDef = TypedDict(
     "CreateLanguageModelResponseTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "ModelStatus": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LanguageModelTypeDef = TypedDict(
     "LanguageModelTypeDef",
     {
         "ModelName": str,
@@ -918,15 +918,15 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1000,44 +1000,44 @@
 
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MedicalTranscriptionJobTypeDef = TypedDict(
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
@@ -1227,24 +1227,24 @@
 ):
     pass
 
 DescribeLanguageModelResponseTypeDef = TypedDict(
     "DescribeLanguageModelResponseTypeDef",
     {
         "LanguageModel": LanguageModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
@@ -1255,65 +1255,65 @@
     total=False,
 )
 
 GetMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "GetMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "StartMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartCallAnalyticsJobResponseTypeDef = TypedDict(
     "StartCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
@@ -1367,35 +1367,35 @@
 ):
     pass
 
 CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "CreateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "GetCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesResponseTypeDef",
     {
         "NextToken": str,
         "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "UpdateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/PKG-INFO` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.26.84
-Summary: Type annotations for boto3.TranscribeService 1.26.84 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.TranscribeService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,33 +324,39 @@
     AbsoluteTimeRangeTypeDef,
     ContentRedactionTypeDef,
     LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
     ChannelDefinitionTypeDef,
     MediaTypeDef,
     TranscriptTypeDef,
-    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
+    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    GetVocabularyResponseTypeDef,
     RelativeTimeRangeTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
@@ -361,33 +367,27 @@
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
     MedicalTranscriptTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
+    ResponseMetadataTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     SubtitlesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CallAnalyticsJobSettingsTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
-    GetVocabularyFilterResponseTypeDef,
-    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
-    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -434,42 +434,42 @@
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

### Comparing `mypy-boto3-transcribe-1.26.84/mypy_boto3_transcribe.egg-info/SOURCES.txt` & `mypy-boto3-transcribe-1.27.0/mypy_boto3_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.26.84/setup.py` & `mypy-boto3-transcribe-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-transcribe.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transcribe",
-    version="1.26.84",
+    version="1.27.0",
     packages=["mypy_boto3_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TranscribeService 1.26.84 service generated with"
-        " mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.TranscribeService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/",
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


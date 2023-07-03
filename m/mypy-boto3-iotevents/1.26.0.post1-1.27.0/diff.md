# Comparing `tmp/mypy-boto3-iotevents-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iotevents-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:34 2022, max compression
+gzip compressed data, was "mypy-boto3-iotevents-1.27.0.tar", last modified: Mon Jul  3 19:50:54 2023, max compression
```

## Comparing `mypy-boto3-iotevents-1.26.0.post1.tar` & `mypy-boto3-iotevents-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.500829 mypy-boto3-iotevents-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15903 2022-11-01 21:43:34.500829 mypy-boto3-iotevents-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14454 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.500829 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18784 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    18752 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8042 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    37352 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    37287 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.500829 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15903 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:34.500829 mypy-boto3-iotevents-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-01 21:36:10.000000 mypy-boto3-iotevents-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.771436 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37394 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/setup.py
```

### Comparing `mypy-boto3-iotevents-1.26.0.post1/LICENSE` & `mypy-boto3-iotevents-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iotevents-1.26.0.post1/PKG-INFO` & `mypy-boto3-iotevents-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTEvents 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTEvents 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
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
 
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,56 +318,56 @@
     AlarmModelVersionSummaryTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAlarmModelResponseTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
     PayloadTypeDef,
     EmailContentTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     SSOIdentityTypeDef,
+    ResponseMetadataTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     AlarmCapabilitiesTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
     AssetPropertyValueTypeDef,
     InputDefinitionTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAlarmModelResponseTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
-    ListAlarmModelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
-    UpdateAlarmModelResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
@@ -426,42 +427,42 @@
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

### Comparing `mypy-boto3-iotevents-1.26.0.post1/README.md` & `mypy-boto3-iotevents-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,56 +286,56 @@
     AlarmModelVersionSummaryTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAlarmModelResponseTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
     PayloadTypeDef,
     EmailContentTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     SSOIdentityTypeDef,
+    ResponseMetadataTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     AlarmCapabilitiesTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
     AssetPropertyValueTypeDef,
     InputDefinitionTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAlarmModelResponseTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
-    ListAlarmModelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
-    UpdateAlarmModelResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
@@ -395,42 +395,42 @@
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

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/client.py` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/client.pyi` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/literals.py` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,25 @@
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
@@ -87,30 +89,35 @@
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
@@ -136,14 +143,15 @@
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
@@ -188,51 +196,57 @@
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
@@ -245,14 +259,15 @@
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
@@ -264,28 +279,35 @@
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
@@ -294,14 +316,15 @@
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
@@ -312,55 +335,64 @@
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
```

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/literals.pyi` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -59,23 +59,25 @@
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
@@ -85,30 +87,35 @@
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
@@ -134,14 +141,15 @@
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
@@ -186,51 +194,57 @@
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
@@ -243,14 +257,15 @@
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
@@ -262,28 +277,35 @@
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
@@ -292,14 +314,15 @@
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
@@ -310,55 +333,64 @@
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
```

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/type_defs.py` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,56 +44,56 @@
     "AlarmModelVersionSummaryTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAlarmModelResponseTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
+    "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
     "PayloadTypeDef",
     "EmailContentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "SSOIdentityTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAlarmModelResponseTypeDef",
     "AlarmCapabilitiesTypeDef",
+    "ListAlarmModelsResponseTypeDef",
+    "ListAlarmModelVersionsResponseTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
     "AssetPropertyValueTypeDef",
     "InputDefinitionTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateAlarmModelResponseTypeDef",
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAlarmModelVersionsResponseTypeDef",
-    "ListAlarmModelsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartDetectorModelAnalysisResponseTypeDef",
-    "UpdateAlarmModelResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
@@ -286,22 +286,23 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAlarmModelResponseTypeDef = TypedDict(
+    "CreateAlarmModelResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectorModelConfigurationTypeDef = TypedDict(
     "DetectorModelConfigurationTypeDef",
     {
         "detectorModelName": str,
@@ -389,14 +390,22 @@
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
+DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    {
+        "status": AnalysisStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDescribeDetectorModelRequestRequestTypeDef = TypedDict(
@@ -481,14 +490,21 @@
     {
         "subject": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
@@ -640,31 +656,80 @@
 )
 
 
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
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
+StartDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "StartDetectorModelAnalysisResponseTypeDef",
+    {
+        "analysisId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateAlarmModelResponseTypeDef = TypedDict(
+    "UpdateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
 )
 
+ListAlarmModelsResponseTypeDef = TypedDict(
+    "ListAlarmModelsResponseTypeDef",
+    {
+        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAlarmModelVersionsResponseTypeDef = TypedDict(
+    "ListAlarmModelVersionsResponseTypeDef",
+    {
+        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -693,124 +758,59 @@
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateAlarmModelResponseTypeDef = TypedDict(
-    "CreateAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    {
-        "status": AnalysisStatusType,
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
-ListAlarmModelVersionsResponseTypeDef = TypedDict(
-    "ListAlarmModelVersionsResponseTypeDef",
-    {
-        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlarmModelsResponseTypeDef = TypedDict(
-    "ListAlarmModelsResponseTypeDef",
-    {
-        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "StartDetectorModelAnalysisResponseTypeDef",
-    {
-        "analysisId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAlarmModelResponseTypeDef = TypedDict(
-    "UpdateAlarmModelResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 CreateDetectorModelResponseTypeDef = TypedDict(
     "CreateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDetectorModelResponseTypeDef = TypedDict(
     "UpdateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
@@ -832,24 +832,24 @@
 
 
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDetectorModelVersionsResponseTypeDef = TypedDict(
     "ListDetectorModelVersionsResponseTypeDef",
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
@@ -1016,15 +1016,15 @@
 
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IotSiteWiseInputIdentifierTypeDef = TypedDict(
     "IotSiteWiseInputIdentifierTypeDef",
     {
         "iotSiteWiseAssetModelPropertyIdentifier": IotSiteWiseAssetModelPropertyIdentifierTypeDef,
@@ -1033,15 +1033,15 @@
 )
 
 ListInputRoutingsResponseTypeDef = TypedDict(
     "ListInputRoutingsResponseTypeDef",
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
@@ -1050,15 +1050,15 @@
 )
 
 GetDetectorModelAnalysisResultsResponseTypeDef = TypedDict(
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
@@ -1124,15 +1124,15 @@
     pass
 
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
@@ -1220,15 +1220,15 @@
     total=False,
 )
 
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInputRoutingsRequestRequestTypeDef = TypedDict(
     "_RequiredListInputRoutingsRequestRequestTypeDef",
     {
         "inputIdentifier": InputIdentifierTypeDef,
@@ -1440,15 +1440,15 @@
         "roleArn": str,
         "key": str,
         "severity": int,
         "alarmRule": AlarmRuleTypeDef,
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
@@ -1551,10 +1551,10 @@
     pass
 
 
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents/type_defs.pyi` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -43,56 +43,56 @@
     "AlarmModelVersionSummaryTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAlarmModelResponseTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
+    "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
     "PayloadTypeDef",
     "EmailContentTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "SSOIdentityTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAlarmModelResponseTypeDef",
     "AlarmCapabilitiesTypeDef",
+    "ListAlarmModelsResponseTypeDef",
+    "ListAlarmModelVersionsResponseTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
     "AssetPropertyValueTypeDef",
     "InputDefinitionTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateAlarmModelResponseTypeDef",
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAlarmModelVersionsResponseTypeDef",
-    "ListAlarmModelsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "StartDetectorModelAnalysisResponseTypeDef",
-    "UpdateAlarmModelResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
@@ -281,22 +281,23 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAlarmModelResponseTypeDef = TypedDict(
+    "CreateAlarmModelResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectorModelConfigurationTypeDef = TypedDict(
     "DetectorModelConfigurationTypeDef",
     {
         "detectorModelName": str,
@@ -380,14 +381,22 @@
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
+DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    {
+        "status": AnalysisStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDescribeDetectorModelRequestRequestTypeDef = TypedDict(
@@ -468,14 +477,21 @@
     {
         "subject": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
@@ -619,31 +635,80 @@
     },
     total=False,
 )
 
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
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
+StartDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "StartDetectorModelAnalysisResponseTypeDef",
+    {
+        "analysisId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateAlarmModelResponseTypeDef = TypedDict(
+    "UpdateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
 )
 
+ListAlarmModelsResponseTypeDef = TypedDict(
+    "ListAlarmModelsResponseTypeDef",
+    {
+        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAlarmModelVersionsResponseTypeDef = TypedDict(
+    "ListAlarmModelVersionsResponseTypeDef",
+    {
+        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -672,124 +737,59 @@
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateAlarmModelResponseTypeDef = TypedDict(
-    "CreateAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    {
-        "status": AnalysisStatusType,
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
-ListAlarmModelVersionsResponseTypeDef = TypedDict(
-    "ListAlarmModelVersionsResponseTypeDef",
-    {
-        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlarmModelsResponseTypeDef = TypedDict(
-    "ListAlarmModelsResponseTypeDef",
-    {
-        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "StartDetectorModelAnalysisResponseTypeDef",
-    {
-        "analysisId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAlarmModelResponseTypeDef = TypedDict(
-    "UpdateAlarmModelResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 CreateDetectorModelResponseTypeDef = TypedDict(
     "CreateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDetectorModelResponseTypeDef = TypedDict(
     "UpdateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
@@ -809,24 +809,24 @@
     pass
 
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDetectorModelVersionsResponseTypeDef = TypedDict(
     "ListDetectorModelVersionsResponseTypeDef",
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
@@ -977,15 +977,15 @@
     pass
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IotSiteWiseInputIdentifierTypeDef = TypedDict(
     "IotSiteWiseInputIdentifierTypeDef",
     {
         "iotSiteWiseAssetModelPropertyIdentifier": IotSiteWiseAssetModelPropertyIdentifierTypeDef,
@@ -994,15 +994,15 @@
 )
 
 ListInputRoutingsResponseTypeDef = TypedDict(
     "ListInputRoutingsResponseTypeDef",
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
@@ -1011,15 +1011,15 @@
 )
 
 GetDetectorModelAnalysisResultsResponseTypeDef = TypedDict(
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
@@ -1081,15 +1081,15 @@
 ):
     pass
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
@@ -1175,15 +1175,15 @@
     total=False,
 )
 
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListInputRoutingsRequestRequestTypeDef = TypedDict(
     "_RequiredListInputRoutingsRequestRequestTypeDef",
     {
         "inputIdentifier": InputIdentifierTypeDef,
@@ -1381,15 +1381,15 @@
         "roleArn": str,
         "key": str,
         "severity": int,
         "alarmRule": AlarmRuleTypeDef,
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
@@ -1486,10 +1486,10 @@
 ):
     pass
 
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/PKG-INFO` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTEvents 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTEvents 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
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
 
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,56 +318,56 @@
     AlarmModelVersionSummaryTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAlarmModelResponseTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
     PayloadTypeDef,
     EmailContentTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     SSOIdentityTypeDef,
+    ResponseMetadataTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     AlarmCapabilitiesTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
     AssetPropertyValueTypeDef,
     InputDefinitionTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateAlarmModelResponseTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
-    ListAlarmModelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
-    UpdateAlarmModelResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
@@ -426,42 +427,42 @@
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

### Comparing `mypy-boto3-iotevents-1.26.0.post1/mypy_boto3_iotevents.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.26.0.post1/setup.py` & `mypy-boto3-iotevents-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iotevents.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEvents 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.IoTEvents 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iotevents": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iotevents": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/",
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


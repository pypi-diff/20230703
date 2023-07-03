# Comparing `tmp/mypy-boto3-iotevents-data-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iotevents-data-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-data-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:34 2022, max compression
+gzip compressed data, was "mypy-boto3-iotevents-data-1.27.0.tar", last modified: Mon Jul  3 19:50:54 2023, max compression
```

## Comparing `mypy-boto3-iotevents-data-1.26.0.post1.tar` & `mypy-boto3-iotevents-data-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.184829 mypy-boto3-iotevents-data-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14353 2022-11-01 21:43:34.180829 mypy-boto3-iotevents-data-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12885 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.180829 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10483 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10465 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7593 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7591 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    18822 2022-11-01 21:36:12.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18797 2022-11-01 21:36:12.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.180829 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14353 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-01 21:43:34.000000 mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:34.184829 mypy-boto3-iotevents-data-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-01 21:36:11.000000 mypy-boto3-iotevents-data-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.791437 mypy-boto3-iotevents-data-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-03 19:50:54.791437 mypy-boto3-iotevents-data-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.791437 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.791437 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:54.791437 mypy-boto3-iotevents-data-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:39:40.000000 mypy-boto3-iotevents-data-1.27.0/setup.py
```

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/LICENSE` & `mypy-boto3-iotevents-data-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/PKG-INFO` & `mypy-boto3-iotevents-data-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents-data
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTEventsData 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTEventsData 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/
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
 
 <a id="mypy-boto3-iotevents-data"></a>
 
 # mypy-boto3-iotevents-data
 
 [![PyPI - mypy-boto3-iotevents-data](https://img.shields.io/pypi/v/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents-data?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEventsData 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
+[boto3.IoTEventsData 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
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
 [mypy-boto3-iotevents-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,15 +306,14 @@
 
 ```python
 from mypy_boto3_iotevents_data.type_defs import (
     AcknowledgeActionConfigurationTypeDef,
     AcknowledgeAlarmActionRequestTypeDef,
     AlarmSummaryTypeDef,
     BatchAlarmActionErrorEntryTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteDetectorErrorEntryTypeDef,
     DeleteDetectorRequestTypeDef,
     DisableAlarmActionRequestTypeDef,
     EnableAlarmActionRequestTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     ResetAlarmActionRequestTypeDef,
     SnoozeAlarmActionRequestTypeDef,
@@ -328,23 +328,24 @@
     VariableDefinitionTypeDef,
     DetectorStateSummaryTypeDef,
     TimerTypeDef,
     VariableTypeDef,
     ListAlarmsRequestRequestTypeDef,
     ListDetectorsRequestRequestTypeDef,
     TimestampValueTypeDef,
+    ResponseMetadataTypeDef,
     SimpleRuleEvaluationTypeDef,
     StateChangeConfigurationTypeDef,
     BatchAcknowledgeAlarmRequestRequestTypeDef,
+    ListAlarmsResponseTypeDef,
     BatchAcknowledgeAlarmResponseTypeDef,
     BatchDisableAlarmResponseTypeDef,
     BatchEnableAlarmResponseTypeDef,
     BatchResetAlarmResponseTypeDef,
     BatchSnoozeAlarmResponseTypeDef,
-    ListAlarmsResponseTypeDef,
     BatchDeleteDetectorResponseTypeDef,
     BatchDeleteDetectorRequestRequestTypeDef,
     BatchDisableAlarmRequestRequestTypeDef,
     BatchEnableAlarmRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchResetAlarmRequestRequestTypeDef,
     BatchSnoozeAlarmRequestRequestTypeDef,
@@ -375,42 +376,42 @@
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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/README.md` & `mypy-boto3-iotevents-data-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotevents-data"></a>
 
 # mypy-boto3-iotevents-data
 
 [![PyPI - mypy-boto3-iotevents-data](https://img.shields.io/pypi/v/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents-data?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEventsData 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
+[boto3.IoTEventsData 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
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
 [mypy-boto3-iotevents-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,15 +274,14 @@
 
 ```python
 from mypy_boto3_iotevents_data.type_defs import (
     AcknowledgeActionConfigurationTypeDef,
     AcknowledgeAlarmActionRequestTypeDef,
     AlarmSummaryTypeDef,
     BatchAlarmActionErrorEntryTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteDetectorErrorEntryTypeDef,
     DeleteDetectorRequestTypeDef,
     DisableAlarmActionRequestTypeDef,
     EnableAlarmActionRequestTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     ResetAlarmActionRequestTypeDef,
     SnoozeAlarmActionRequestTypeDef,
@@ -297,23 +296,24 @@
     VariableDefinitionTypeDef,
     DetectorStateSummaryTypeDef,
     TimerTypeDef,
     VariableTypeDef,
     ListAlarmsRequestRequestTypeDef,
     ListDetectorsRequestRequestTypeDef,
     TimestampValueTypeDef,
+    ResponseMetadataTypeDef,
     SimpleRuleEvaluationTypeDef,
     StateChangeConfigurationTypeDef,
     BatchAcknowledgeAlarmRequestRequestTypeDef,
+    ListAlarmsResponseTypeDef,
     BatchAcknowledgeAlarmResponseTypeDef,
     BatchDisableAlarmResponseTypeDef,
     BatchEnableAlarmResponseTypeDef,
     BatchResetAlarmResponseTypeDef,
     BatchSnoozeAlarmResponseTypeDef,
-    ListAlarmsResponseTypeDef,
     BatchDeleteDetectorResponseTypeDef,
     BatchDeleteDetectorRequestRequestTypeDef,
     BatchDisableAlarmRequestRequestTypeDef,
     BatchEnableAlarmRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchResetAlarmRequestRequestTypeDef,
     BatchSnoozeAlarmRequestRequestTypeDef,
@@ -344,42 +344,42 @@
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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/__main__.py` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEventsData 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.IoTEventsData 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData\nOther"
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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/client.py` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/client.pyi` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/literals.py` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,25 @@
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
@@ -86,30 +88,35 @@
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
@@ -135,14 +142,15 @@
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
@@ -187,51 +195,57 @@
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
@@ -244,14 +258,15 @@
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
@@ -263,28 +278,35 @@
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
@@ -293,14 +315,15 @@
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
@@ -311,55 +334,64 @@
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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/literals.pyi` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,25 @@
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
@@ -84,30 +86,35 @@
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
@@ -133,14 +140,15 @@
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
@@ -185,51 +193,57 @@
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
@@ -242,14 +256,15 @@
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
@@ -261,28 +276,35 @@
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
@@ -291,14 +313,15 @@
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
@@ -309,55 +332,64 @@
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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/type_defs.py` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 
 __all__ = (
     "AcknowledgeActionConfigurationTypeDef",
     "AcknowledgeAlarmActionRequestTypeDef",
     "AlarmSummaryTypeDef",
     "BatchAlarmActionErrorEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteDetectorErrorEntryTypeDef",
     "DeleteDetectorRequestTypeDef",
     "DisableAlarmActionRequestTypeDef",
     "EnableAlarmActionRequestTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResetAlarmActionRequestTypeDef",
     "SnoozeAlarmActionRequestTypeDef",
@@ -58,23 +57,24 @@
     "VariableDefinitionTypeDef",
     "DetectorStateSummaryTypeDef",
     "TimerTypeDef",
     "VariableTypeDef",
     "ListAlarmsRequestRequestTypeDef",
     "ListDetectorsRequestRequestTypeDef",
     "TimestampValueTypeDef",
+    "ResponseMetadataTypeDef",
     "SimpleRuleEvaluationTypeDef",
     "StateChangeConfigurationTypeDef",
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
+    "ListAlarmsResponseTypeDef",
     "BatchAcknowledgeAlarmResponseTypeDef",
     "BatchDisableAlarmResponseTypeDef",
     "BatchEnableAlarmResponseTypeDef",
     "BatchResetAlarmResponseTypeDef",
     "BatchSnoozeAlarmResponseTypeDef",
-    "ListAlarmsResponseTypeDef",
     "BatchDeleteDetectorResponseTypeDef",
     "BatchDeleteDetectorRequestRequestTypeDef",
     "BatchDisableAlarmRequestRequestTypeDef",
     "BatchEnableAlarmRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "BatchResetAlarmRequestRequestTypeDef",
     "BatchSnoozeAlarmRequestRequestTypeDef",
@@ -147,25 +147,14 @@
         "requestId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
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
 BatchDeleteDetectorErrorEntryTypeDef = TypedDict(
     "BatchDeleteDetectorErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
@@ -471,14 +460,25 @@
     "TimestampValueTypeDef",
     {
         "timeInMillis": int,
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
 SimpleRuleEvaluationTypeDef = TypedDict(
     "SimpleRuleEvaluationTypeDef",
     {
         "inputPropertyValue": str,
         "operator": ComparisonOperatorType,
         "thresholdValue": str,
     },
@@ -496,68 +496,68 @@
 BatchAcknowledgeAlarmRequestRequestTypeDef = TypedDict(
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
     {
         "acknowledgeActionRequests": Sequence[AcknowledgeAlarmActionRequestTypeDef],
     },
 )
 
+ListAlarmsResponseTypeDef = TypedDict(
+    "ListAlarmsResponseTypeDef",
+    {
+        "alarmSummaries": List[AlarmSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchAcknowledgeAlarmResponseTypeDef = TypedDict(
     "BatchAcknowledgeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisableAlarmResponseTypeDef = TypedDict(
     "BatchDisableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEnableAlarmResponseTypeDef = TypedDict(
     "BatchEnableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchResetAlarmResponseTypeDef = TypedDict(
     "BatchResetAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchSnoozeAlarmResponseTypeDef = TypedDict(
     "BatchSnoozeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlarmsResponseTypeDef = TypedDict(
-    "ListAlarmsResponseTypeDef",
-    {
-        "alarmSummaries": List[AlarmSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteDetectorResponseTypeDef = TypedDict(
     "BatchDeleteDetectorResponseTypeDef",
     {
         "batchDeleteDetectorErrorEntries": List[BatchDeleteDetectorErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteDetectorRequestRequestTypeDef = TypedDict(
     "BatchDeleteDetectorRequestRequestTypeDef",
     {
         "detectors": Sequence[DeleteDetectorRequestTypeDef],
@@ -578,15 +578,15 @@
     },
 )
 
 BatchPutMessageResponseTypeDef = TypedDict(
     "BatchPutMessageResponseTypeDef",
     {
         "BatchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchResetAlarmRequestRequestTypeDef = TypedDict(
     "BatchResetAlarmRequestRequestTypeDef",
     {
         "resetActionRequests": Sequence[ResetAlarmActionRequestTypeDef],
@@ -600,15 +600,15 @@
     },
 )
 
 BatchUpdateDetectorResponseTypeDef = TypedDict(
     "BatchUpdateDetectorResponseTypeDef",
     {
         "batchUpdateDetectorErrorEntries": List[BatchUpdateDetectorErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomerActionTypeDef = TypedDict(
     "CustomerActionTypeDef",
     {
         "actionName": CustomerActionNameType,
@@ -714,15 +714,15 @@
 
 
 ListDetectorsResponseTypeDef = TypedDict(
     "ListDetectorsResponseTypeDef",
     {
         "detectorSummaries": List[DetectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectorTypeDef = TypedDict(
     "DetectorTypeDef",
     {
         "detectorModelName": str,
@@ -760,15 +760,15 @@
     },
 )
 
 DescribeDetectorResponseTypeDef = TypedDict(
     "DescribeDetectorResponseTypeDef",
     {
         "detector": DetectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "alarmModelName": str,
@@ -782,10 +782,10 @@
     total=False,
 )
 
 DescribeAlarmResponseTypeDef = TypedDict(
     "DescribeAlarmResponseTypeDef",
     {
         "alarm": AlarmTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data/type_defs.pyi` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcknowledgeActionConfigurationTypeDef",
     "AcknowledgeAlarmActionRequestTypeDef",
     "AlarmSummaryTypeDef",
     "BatchAlarmActionErrorEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteDetectorErrorEntryTypeDef",
     "DeleteDetectorRequestTypeDef",
     "DisableAlarmActionRequestTypeDef",
     "EnableAlarmActionRequestTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResetAlarmActionRequestTypeDef",
     "SnoozeAlarmActionRequestTypeDef",
@@ -57,23 +56,24 @@
     "VariableDefinitionTypeDef",
     "DetectorStateSummaryTypeDef",
     "TimerTypeDef",
     "VariableTypeDef",
     "ListAlarmsRequestRequestTypeDef",
     "ListDetectorsRequestRequestTypeDef",
     "TimestampValueTypeDef",
+    "ResponseMetadataTypeDef",
     "SimpleRuleEvaluationTypeDef",
     "StateChangeConfigurationTypeDef",
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
+    "ListAlarmsResponseTypeDef",
     "BatchAcknowledgeAlarmResponseTypeDef",
     "BatchDisableAlarmResponseTypeDef",
     "BatchEnableAlarmResponseTypeDef",
     "BatchResetAlarmResponseTypeDef",
     "BatchSnoozeAlarmResponseTypeDef",
-    "ListAlarmsResponseTypeDef",
     "BatchDeleteDetectorResponseTypeDef",
     "BatchDeleteDetectorRequestRequestTypeDef",
     "BatchDisableAlarmRequestRequestTypeDef",
     "BatchEnableAlarmRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "BatchResetAlarmRequestRequestTypeDef",
     "BatchSnoozeAlarmRequestRequestTypeDef",
@@ -144,25 +144,14 @@
         "requestId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
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
 BatchDeleteDetectorErrorEntryTypeDef = TypedDict(
     "BatchDeleteDetectorErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
@@ -450,14 +439,25 @@
     "TimestampValueTypeDef",
     {
         "timeInMillis": int,
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
 SimpleRuleEvaluationTypeDef = TypedDict(
     "SimpleRuleEvaluationTypeDef",
     {
         "inputPropertyValue": str,
         "operator": ComparisonOperatorType,
         "thresholdValue": str,
     },
@@ -475,68 +475,68 @@
 BatchAcknowledgeAlarmRequestRequestTypeDef = TypedDict(
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
     {
         "acknowledgeActionRequests": Sequence[AcknowledgeAlarmActionRequestTypeDef],
     },
 )
 
+ListAlarmsResponseTypeDef = TypedDict(
+    "ListAlarmsResponseTypeDef",
+    {
+        "alarmSummaries": List[AlarmSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchAcknowledgeAlarmResponseTypeDef = TypedDict(
     "BatchAcknowledgeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisableAlarmResponseTypeDef = TypedDict(
     "BatchDisableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEnableAlarmResponseTypeDef = TypedDict(
     "BatchEnableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchResetAlarmResponseTypeDef = TypedDict(
     "BatchResetAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchSnoozeAlarmResponseTypeDef = TypedDict(
     "BatchSnoozeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAlarmsResponseTypeDef = TypedDict(
-    "ListAlarmsResponseTypeDef",
-    {
-        "alarmSummaries": List[AlarmSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteDetectorResponseTypeDef = TypedDict(
     "BatchDeleteDetectorResponseTypeDef",
     {
         "batchDeleteDetectorErrorEntries": List[BatchDeleteDetectorErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteDetectorRequestRequestTypeDef = TypedDict(
     "BatchDeleteDetectorRequestRequestTypeDef",
     {
         "detectors": Sequence[DeleteDetectorRequestTypeDef],
@@ -557,15 +557,15 @@
     },
 )
 
 BatchPutMessageResponseTypeDef = TypedDict(
     "BatchPutMessageResponseTypeDef",
     {
         "BatchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchResetAlarmRequestRequestTypeDef = TypedDict(
     "BatchResetAlarmRequestRequestTypeDef",
     {
         "resetActionRequests": Sequence[ResetAlarmActionRequestTypeDef],
@@ -579,15 +579,15 @@
     },
 )
 
 BatchUpdateDetectorResponseTypeDef = TypedDict(
     "BatchUpdateDetectorResponseTypeDef",
     {
         "batchUpdateDetectorErrorEntries": List[BatchUpdateDetectorErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomerActionTypeDef = TypedDict(
     "CustomerActionTypeDef",
     {
         "actionName": CustomerActionNameType,
@@ -689,15 +689,15 @@
     pass
 
 ListDetectorsResponseTypeDef = TypedDict(
     "ListDetectorsResponseTypeDef",
     {
         "detectorSummaries": List[DetectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectorTypeDef = TypedDict(
     "DetectorTypeDef",
     {
         "detectorModelName": str,
@@ -735,15 +735,15 @@
     },
 )
 
 DescribeDetectorResponseTypeDef = TypedDict(
     "DescribeDetectorResponseTypeDef",
     {
         "detector": DetectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "alarmModelName": str,
@@ -757,10 +757,10 @@
     total=False,
 )
 
 DescribeAlarmResponseTypeDef = TypedDict(
     "DescribeAlarmResponseTypeDef",
     {
         "alarm": AlarmTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/PKG-INFO` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents-data
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTEventsData 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTEventsData 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/
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
 
 <a id="mypy-boto3-iotevents-data"></a>
 
 # mypy-boto3-iotevents-data
 
 [![PyPI - mypy-boto3-iotevents-data](https://img.shields.io/pypi/v/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents-data?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEventsData 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
+[boto3.IoTEventsData 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
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
 [mypy-boto3-iotevents-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,15 +306,14 @@
 
 ```python
 from mypy_boto3_iotevents_data.type_defs import (
     AcknowledgeActionConfigurationTypeDef,
     AcknowledgeAlarmActionRequestTypeDef,
     AlarmSummaryTypeDef,
     BatchAlarmActionErrorEntryTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteDetectorErrorEntryTypeDef,
     DeleteDetectorRequestTypeDef,
     DisableAlarmActionRequestTypeDef,
     EnableAlarmActionRequestTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     ResetAlarmActionRequestTypeDef,
     SnoozeAlarmActionRequestTypeDef,
@@ -328,23 +328,24 @@
     VariableDefinitionTypeDef,
     DetectorStateSummaryTypeDef,
     TimerTypeDef,
     VariableTypeDef,
     ListAlarmsRequestRequestTypeDef,
     ListDetectorsRequestRequestTypeDef,
     TimestampValueTypeDef,
+    ResponseMetadataTypeDef,
     SimpleRuleEvaluationTypeDef,
     StateChangeConfigurationTypeDef,
     BatchAcknowledgeAlarmRequestRequestTypeDef,
+    ListAlarmsResponseTypeDef,
     BatchAcknowledgeAlarmResponseTypeDef,
     BatchDisableAlarmResponseTypeDef,
     BatchEnableAlarmResponseTypeDef,
     BatchResetAlarmResponseTypeDef,
     BatchSnoozeAlarmResponseTypeDef,
-    ListAlarmsResponseTypeDef,
     BatchDeleteDetectorResponseTypeDef,
     BatchDeleteDetectorRequestRequestTypeDef,
     BatchDisableAlarmRequestRequestTypeDef,
     BatchEnableAlarmRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchResetAlarmRequestRequestTypeDef,
     BatchSnoozeAlarmRequestRequestTypeDef,
@@ -375,42 +376,42 @@
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

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/mypy_boto3_iotevents_data.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-data-1.27.0/mypy_boto3_iotevents_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.26.0.post1/setup.py` & `mypy-boto3-iotevents-data-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iotevents-data.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents-data",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iotevents_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEventsData 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.IoTEventsData 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 iotevents-data type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iotevents_data": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iotevents_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/",
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


# Comparing `tmp/mypy-boto3-chime-sdk-meetings-1.26.68.tar.gz` & `tmp/mypy-boto3-chime-sdk-meetings-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-meetings-1.26.68.tar` & `mypy-boto3-chime-sdk-meetings-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-02-09 20:26:11.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-09 20:26:49.000000 mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.970837 mypy-boto3-chime-sdk-meetings-1.26.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-09 20:26:10.000000 mypy-boto3-chime-sdk-meetings-1.26.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.326907 mypy-boto3-chime-sdk-meetings-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-03 19:50:27.322907 mypy-boto3-chime-sdk-meetings-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.318907 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.322907 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.326907 mypy-boto3-chime-sdk-meetings-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-03 19:33:26.000000 mypy-boto3-chime-sdk-meetings-1.27.0/setup.py
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/LICENSE` & `mypy-boto3-chime-sdk-meetings-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.26.68
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,35 +314,35 @@
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
-    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MediaPlacementTypeDef,
+    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
     MeetingFeaturesConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
@@ -365,42 +365,42 @@
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

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/README.md` & `mypy-boto3-chime-sdk-meetings-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,35 +282,35 @@
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
-    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MediaPlacementTypeDef,
+    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
     MeetingFeaturesConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
@@ -333,42 +333,42 @@
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

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/__main__.py` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMeetings 1.26.68\nVersion:         1.26.68\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMeetings 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.68")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.py` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,12 +279,12 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#untag_resource)
         """
 
     def update_attendee_capabilities(
         self, *, MeetingId: str, AttendeeId: str, Capabilities: AttendeeCapabilitiesTypeDef
     ) -> UpdateAttendeeCapabilitiesResponseTypeDef:
         """
-        The capabilties that you want to update.
+        The capabilities that you want to update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.update_attendee_capabilities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#update_attendee_capabilities)
         """
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/client.pyi` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -257,12 +257,12 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#untag_resource)
         """
     def update_attendee_capabilities(
         self, *, MeetingId: str, AttendeeId: str, Capabilities: AttendeeCapabilitiesTypeDef
     ) -> UpdateAttendeeCapabilitiesResponseTypeDef:
         """
-        The capabilties that you want to update.
+        The capabilities that you want to update.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings.Client.update_attendee_capabilities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/client/#update_attendee_capabilities)
         """
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.py` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/literals.pyi`

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
     "MediaCapabilitiesType",
     "MeetingFeatureStatusType",
     "TranscribeContentIdentificationTypeType",
     "TranscribeContentRedactionTypeType",
     "TranscribeLanguageCodeType",
     "TranscribeMedicalContentIdentificationTypeType",
@@ -35,31 +34,32 @@
     "TranscribeVocabularyFilterMethodType",
     "ChimeSDKMeetingsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 MediaCapabilitiesType = Literal["None", "Receive", "Send", "SendReceive"]
 MeetingFeatureStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 TranscribeContentIdentificationTypeType = Literal["PII"]
 TranscribeContentRedactionTypeType = Literal["PII"]
 TranscribeLanguageCodeType = Literal[
     "de-DE",
     "en-AU",
     "en-GB",
     "en-US",
     "es-US",
     "fr-CA",
     "fr-FR",
+    "hi-IN",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "pt-BR",
+    "th-TH",
     "zh-CN",
 ]
 TranscribeMedicalContentIdentificationTypeType = Literal["PHI"]
 TranscribeMedicalLanguageCodeType = Literal["en-US"]
 TranscribeMedicalRegionType = Literal[
     "ap-southeast-2", "auto", "ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"
 ]
@@ -96,14 +96,15 @@
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
@@ -143,14 +144,15 @@
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
@@ -229,14 +231,15 @@
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
@@ -247,14 +250,15 @@
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
@@ -290,14 +294,15 @@
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
@@ -316,16 +321,19 @@
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
@@ -405,18 +413,21 @@
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

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/literals.pyi` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/literals.py`

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
     "MediaCapabilitiesType",
     "MeetingFeatureStatusType",
     "TranscribeContentIdentificationTypeType",
     "TranscribeContentRedactionTypeType",
     "TranscribeLanguageCodeType",
     "TranscribeMedicalContentIdentificationTypeType",
@@ -34,30 +35,33 @@
     "TranscribeVocabularyFilterMethodType",
     "ChimeSDKMeetingsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 MediaCapabilitiesType = Literal["None", "Receive", "Send", "SendReceive"]
 MeetingFeatureStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 TranscribeContentIdentificationTypeType = Literal["PII"]
 TranscribeContentRedactionTypeType = Literal["PII"]
 TranscribeLanguageCodeType = Literal[
     "de-DE",
     "en-AU",
     "en-GB",
     "en-US",
     "es-US",
     "fr-CA",
     "fr-FR",
+    "hi-IN",
     "it-IT",
     "ja-JP",
     "ko-KR",
     "pt-BR",
+    "th-TH",
     "zh-CN",
 ]
 TranscribeMedicalContentIdentificationTypeType = Literal["PHI"]
 TranscribeMedicalLanguageCodeType = Literal["en-US"]
 TranscribeMedicalRegionType = Literal[
     "ap-southeast-2", "auto", "ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"
 ]
@@ -94,14 +98,15 @@
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
@@ -141,14 +146,15 @@
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
@@ -227,14 +233,15 @@
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
@@ -245,14 +252,15 @@
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
@@ -288,14 +296,15 @@
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
@@ -314,16 +323,19 @@
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
@@ -403,18 +415,21 @@
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

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.py` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,35 +37,35 @@
 
 
 __all__ = (
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MediaPlacementTypeDef",
+    "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
@@ -110,25 +110,14 @@
         "ExternalUserId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 NotificationsConfigurationTypeDef = TypedDict(
     "NotificationsConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
@@ -154,14 +143,21 @@
 DeleteMeetingRequestRequestTypeDef = TypedDict(
     "DeleteMeetingRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -196,14 +192,16 @@
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "IdentifyLanguage": bool,
         "LanguageOptions": str,
         "PreferredLanguage": TranscribeLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
 GetAttendeeRequestRequestTypeDef = TypedDict(
     "GetAttendeeRequestRequestTypeDef",
     {
@@ -259,14 +257,25 @@
         "ScreenViewingUrl": str,
         "ScreenSharingUrl": str,
         "EventIngestionUrl": str,
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -354,26 +363,19 @@
     "MeetingFeaturesConfigurationTypeDef",
     {
         "Audio": AudioFeaturesTypeDef,
     },
     total=False,
 )
 
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -391,48 +393,48 @@
 )
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAttendeeCapabilitiesResponseTypeDef = TypedDict(
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -522,28 +524,28 @@
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings/type_defs.pyi` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,35 +36,35 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MediaPlacementTypeDef",
+    "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
@@ -109,25 +109,14 @@
         "ExternalUserId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 NotificationsConfigurationTypeDef = TypedDict(
     "NotificationsConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
@@ -153,14 +142,21 @@
 DeleteMeetingRequestRequestTypeDef = TypedDict(
     "DeleteMeetingRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -193,14 +189,16 @@
         "ContentIdentificationType": Literal["PII"],
         "ContentRedactionType": Literal["PII"],
         "PiiEntityTypes": str,
         "LanguageModelName": str,
         "IdentifyLanguage": bool,
         "LanguageOptions": str,
         "PreferredLanguage": TranscribeLanguageCodeType,
+        "VocabularyNames": str,
+        "VocabularyFilterNames": str,
     },
     total=False,
 )
 
 GetAttendeeRequestRequestTypeDef = TypedDict(
     "GetAttendeeRequestRequestTypeDef",
     {
@@ -254,14 +252,25 @@
         "ScreenViewingUrl": str,
         "ScreenSharingUrl": str,
         "EventIngestionUrl": str,
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -345,26 +354,19 @@
     "MeetingFeaturesConfigurationTypeDef",
     {
         "Audio": AudioFeaturesTypeDef,
     },
     total=False,
 )
 
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -382,48 +384,48 @@
 )
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAttendeeCapabilitiesResponseTypeDef = TypedDict(
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -509,28 +511,28 @@
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.26.68
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,35 +314,35 @@
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
-    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MediaPlacementTypeDef,
+    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
     MeetingFeaturesConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
@@ -365,42 +365,42 @@
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

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-meetings-1.27.0/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.26.68/setup.py` & `mypy-boto3-chime-sdk-meetings-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-chime-sdk-meetings.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-meetings",
-    version="1.26.68",
+    version="1.27.0",
     packages=["mypy_boto3_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMeetings 1.26.68 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ChimeSDKMeetings 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -47,11 +47,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/"
         ),
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


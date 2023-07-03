# Comparing `tmp/mypy-boto3-ivs-realtime-1.26.98.tar.gz` & `tmp/mypy-boto3-ivs-realtime-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-realtime-1.26.98.tar", last modified: Thu Mar 23 19:33:06 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-realtime-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
```

## Comparing `mypy-boto3-ivs-realtime-1.26.98.tar` & `mypy-boto3-ivs-realtime-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.899668 mypy-boto3-ivs-realtime-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-03-23 19:33:06.895668 mypy-boto3-ivs-realtime-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.895668 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.895668 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-03-23 19:33:06.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-23 19:33:06.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:06.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-23 19:33:06.000000 mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:06.899668 mypy-boto3-ivs-realtime-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-23 19:32:13.000000 mypy-boto3-ivs-realtime-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.035477 mypy-boto3-ivs-realtime-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-03 19:50:57.035477 mypy-boto3-ivs-realtime-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.027477 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-03 19:40:03.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-03 19:40:04.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-03 19:40:04.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-07-03 19:40:04.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-03 19:40:04.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.035477 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-03 19:50:56.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:50:56.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:56.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:56.000000 mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:57.035477 mypy-boto3-ivs-realtime-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:40:02.000000 mypy-boto3-ivs-realtime-1.27.0/setup.py
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/LICENSE` & `mypy-boto3-ivs-realtime-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.26.98/PKG-INFO` & `mypy-boto3-ivs-realtime-1.27.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs-realtime
-Version: 1.26.98
-Summary: Type annotations for boto3.ivsrealtime 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ivsrealtime 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ivs-realtime"></a>
 
 # mypy-boto3-ivs-realtime
 
 [![PyPI - mypy-boto3-ivs-realtime](https://img.shields.io/pypi/v/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs-realtime?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.ivsrealtime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -276,54 +276,73 @@
 ### Literals
 
 `mypy_boto3_ivs_realtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.literals import (
+    EventErrorCodeType,
+    EventNameType,
+    ParticipantStateType,
     ParticipantTokenCapabilityType,
     ivsrealtimeServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
-def check_value(value: ParticipantTokenCapabilityType) -> bool:
+def check_value(value: EventErrorCodeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import (
     CreateParticipantTokenRequestRequestTypeDef,
     ParticipantTokenTypeDef,
-    ResponseMetadataTypeDef,
     ParticipantTokenConfigurationTypeDef,
     StageTypeDef,
     DeleteStageRequestRequestTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
+    EventTypeDef,
+    GetParticipantRequestRequestTypeDef,
+    ParticipantTypeDef,
     GetStageRequestRequestTypeDef,
+    GetStageSessionRequestRequestTypeDef,
+    StageSessionTypeDef,
+    ListParticipantEventsRequestRequestTypeDef,
+    ListParticipantsRequestRequestTypeDef,
+    ParticipantSummaryTypeDef,
+    ListStageSessionsRequestRequestTypeDef,
+    StageSessionSummaryTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     CreateParticipantTokenResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     UpdateStageResponseTypeDef,
+    ListParticipantEventsResponseTypeDef,
+    GetParticipantResponseTypeDef,
+    GetStageSessionResponseTypeDef,
+    ListParticipantsResponseTypeDef,
+    ListStageSessionsResponseTypeDef,
     ListStagesResponseTypeDef,
 )
 
 
 def get_structure() -> CreateParticipantTokenRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/README.md` & `mypy-boto3-ivs-realtime-1.27.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivs-realtime"></a>
 
 # mypy-boto3-ivs-realtime
 
 [![PyPI - mypy-boto3-ivs-realtime](https://img.shields.io/pypi/v/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs-realtime?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.ivsrealtime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -244,54 +244,73 @@
 ### Literals
 
 `mypy_boto3_ivs_realtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.literals import (
+    EventErrorCodeType,
+    EventNameType,
+    ParticipantStateType,
     ParticipantTokenCapabilityType,
     ivsrealtimeServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
-def check_value(value: ParticipantTokenCapabilityType) -> bool:
+def check_value(value: EventErrorCodeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import (
     CreateParticipantTokenRequestRequestTypeDef,
     ParticipantTokenTypeDef,
-    ResponseMetadataTypeDef,
     ParticipantTokenConfigurationTypeDef,
     StageTypeDef,
     DeleteStageRequestRequestTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
+    EventTypeDef,
+    GetParticipantRequestRequestTypeDef,
+    ParticipantTypeDef,
     GetStageRequestRequestTypeDef,
+    GetStageSessionRequestRequestTypeDef,
+    StageSessionTypeDef,
+    ListParticipantEventsRequestRequestTypeDef,
+    ListParticipantsRequestRequestTypeDef,
+    ParticipantSummaryTypeDef,
+    ListStageSessionsRequestRequestTypeDef,
+    StageSessionSummaryTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     CreateParticipantTokenResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     UpdateStageResponseTypeDef,
+    ListParticipantEventsResponseTypeDef,
+    GetParticipantResponseTypeDef,
+    GetStageSessionResponseTypeDef,
+    ListParticipantsResponseTypeDef,
+    ListStageSessionsResponseTypeDef,
     ListStagesResponseTypeDef,
 )
 
 
 def get_structure() -> CreateParticipantTokenRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/__main__.py` & `mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivsrealtime 1.26.98\nVersion:         1.26.98\nBuilder version:"
-        " 7.14.2\nDocs:           "
+        "Type annotations for boto3.ivsrealtime 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.98")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/client.py` & `mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,24 @@
     client: ivsrealtimeClient = session.client("ivs-realtime")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ParticipantTokenCapabilityType
+from .literals import ParticipantStateType, ParticipantTokenCapabilityType
 from .type_defs import (
     CreateParticipantTokenResponseTypeDef,
     CreateStageResponseTypeDef,
+    GetParticipantResponseTypeDef,
     GetStageResponseTypeDef,
+    GetStageSessionResponseTypeDef,
+    ListParticipantEventsResponseTypeDef,
+    ListParticipantsResponseTypeDef,
+    ListStageSessionsResponseTypeDef,
     ListStagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ParticipantTokenConfigurationTypeDef,
     UpdateStageResponseTypeDef,
 )
 
 __all__ = ("ivsrealtimeClient",)
@@ -142,22 +147,85 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#generate_presigned_url)
         """
 
+    def get_participant(
+        self, *, participantId: str, sessionId: str, stageArn: str
+    ) -> GetParticipantResponseTypeDef:
+        """
+        Gets information about the specified participant token.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_participant)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_participant)
+        """
+
     def get_stage(self, *, arn: str) -> GetStageResponseTypeDef:
         """
         Gets information for the specified stage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage)
         """
 
+    def get_stage_session(self, *, sessionId: str, stageArn: str) -> GetStageSessionResponseTypeDef:
+        """
+        Gets information for the specified stage session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage_session)
+        """
+
+    def list_participant_events(
+        self,
+        *,
+        participantId: str,
+        sessionId: str,
+        stageArn: str,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListParticipantEventsResponseTypeDef:
+        """
+        Lists events for a specified participant that occurred during a specified stage
+        session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participant_events)
+        """
+
+    def list_participants(
+        self,
+        *,
+        sessionId: str,
+        stageArn: str,
+        filterByPublished: bool = ...,
+        filterByState: ParticipantStateType = ...,
+        filterByUserId: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListParticipantsResponseTypeDef:
+        """
+        Lists all participants in a specified stage session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participants)
+        """
+
+    def list_stage_sessions(
+        self, *, stageArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListStageSessionsResponseTypeDef:
+        """
+        Gets all sessions for a specified stage.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stage_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_stage_sessions)
+        """
+
     def list_stages(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStagesResponseTypeDef:
         """
         Gets summary information about all stages in your account, in the AWS region
         where the API request is processed.
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/client.pyi` & `mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,24 @@
     client: ivsrealtimeClient = session.client("ivs-realtime")
     ```
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ParticipantTokenCapabilityType
+from .literals import ParticipantStateType, ParticipantTokenCapabilityType
 from .type_defs import (
     CreateParticipantTokenResponseTypeDef,
     CreateStageResponseTypeDef,
+    GetParticipantResponseTypeDef,
     GetStageResponseTypeDef,
+    GetStageSessionResponseTypeDef,
+    ListParticipantEventsResponseTypeDef,
+    ListParticipantsResponseTypeDef,
+    ListStageSessionsResponseTypeDef,
     ListStagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ParticipantTokenConfigurationTypeDef,
     UpdateStageResponseTypeDef,
 )
 
 __all__ = ("ivsrealtimeClient",)
@@ -131,21 +136,79 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#generate_presigned_url)
         """
+    def get_participant(
+        self, *, participantId: str, sessionId: str, stageArn: str
+    ) -> GetParticipantResponseTypeDef:
+        """
+        Gets information about the specified participant token.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_participant)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_participant)
+        """
     def get_stage(self, *, arn: str) -> GetStageResponseTypeDef:
         """
         Gets information for the specified stage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage)
         """
+    def get_stage_session(self, *, sessionId: str, stageArn: str) -> GetStageSessionResponseTypeDef:
+        """
+        Gets information for the specified stage session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#get_stage_session)
+        """
+    def list_participant_events(
+        self,
+        *,
+        participantId: str,
+        sessionId: str,
+        stageArn: str,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListParticipantEventsResponseTypeDef:
+        """
+        Lists events for a specified participant that occurred during a specified stage
+        session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participant_events)
+        """
+    def list_participants(
+        self,
+        *,
+        sessionId: str,
+        stageArn: str,
+        filterByPublished: bool = ...,
+        filterByState: ParticipantStateType = ...,
+        filterByUserId: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListParticipantsResponseTypeDef:
+        """
+        Lists all participants in a specified stage session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_participants)
+        """
+    def list_stage_sessions(
+        self, *, stageArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListStageSessionsResponseTypeDef:
+        """
+        Gets all sessions for a specified stage.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stage_sessions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/client/#list_stage_sessions)
+        """
     def list_stages(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStagesResponseTypeDef:
         """
         Gets summary information about all stages in your account, in the AWS region
         where the API request is processed.
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime/type_defs.py` & `mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime/type_defs.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,43 +11,62 @@
     data: CreateParticipantTokenRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
-from .literals import ParticipantTokenCapabilityType
+from .literals import EventNameType, ParticipantStateType, ParticipantTokenCapabilityType
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateParticipantTokenRequestRequestTypeDef",
     "ParticipantTokenTypeDef",
-    "ResponseMetadataTypeDef",
     "ParticipantTokenConfigurationTypeDef",
     "StageTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
+    "EventTypeDef",
+    "GetParticipantRequestRequestTypeDef",
+    "ParticipantTypeDef",
     "GetStageRequestRequestTypeDef",
+    "GetStageSessionRequestRequestTypeDef",
+    "StageSessionTypeDef",
+    "ListParticipantEventsRequestRequestTypeDef",
+    "ListParticipantsRequestRequestTypeDef",
+    "ParticipantSummaryTypeDef",
+    "ListStageSessionsRequestRequestTypeDef",
+    "StageSessionSummaryTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "CreateParticipantTokenResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "UpdateStageResponseTypeDef",
+    "ListParticipantEventsResponseTypeDef",
+    "GetParticipantResponseTypeDef",
+    "GetStageSessionResponseTypeDef",
+    "ListParticipantsResponseTypeDef",
+    "ListStageSessionsResponseTypeDef",
     "ListStagesResponseTypeDef",
 )
 
 _RequiredCreateParticipantTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParticipantTokenRequestRequestTypeDef",
     {
         "stageArn": str,
@@ -82,25 +101,14 @@
         "participantId": str,
         "token": str,
         "userId": str,
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
 ParticipantTokenConfigurationTypeDef = TypedDict(
     "ParticipantTokenConfigurationTypeDef",
     {
         "attributes": Mapping[str, str],
         "capabilities": Sequence[ParticipantTokenCapabilityType],
         "duration": int,
         "userId": str,
@@ -155,21 +163,168 @@
 class DisconnectParticipantRequestRequestTypeDef(
     _RequiredDisconnectParticipantRequestRequestTypeDef,
     _OptionalDisconnectParticipantRequestRequestTypeDef,
 ):
     pass
 
 
+EventTypeDef = TypedDict(
+    "EventTypeDef",
+    {
+        "errorCode": Literal["INSUFFICIENT_CAPABILITIES"],
+        "eventTime": datetime,
+        "name": EventNameType,
+        "participantId": str,
+        "remoteParticipantId": str,
+    },
+    total=False,
+)
+
+GetParticipantRequestRequestTypeDef = TypedDict(
+    "GetParticipantRequestRequestTypeDef",
+    {
+        "participantId": str,
+        "sessionId": str,
+        "stageArn": str,
+    },
+)
+
+ParticipantTypeDef = TypedDict(
+    "ParticipantTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "firstJoinTime": datetime,
+        "participantId": str,
+        "published": bool,
+        "state": ParticipantStateType,
+        "userId": str,
+    },
+    total=False,
+)
+
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+GetStageSessionRequestRequestTypeDef = TypedDict(
+    "GetStageSessionRequestRequestTypeDef",
+    {
+        "sessionId": str,
+        "stageArn": str,
+    },
+)
+
+StageSessionTypeDef = TypedDict(
+    "StageSessionTypeDef",
+    {
+        "endTime": datetime,
+        "sessionId": str,
+        "startTime": datetime,
+    },
+    total=False,
+)
+
+_RequiredListParticipantEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListParticipantEventsRequestRequestTypeDef",
+    {
+        "participantId": str,
+        "sessionId": str,
+        "stageArn": str,
+    },
+)
+_OptionalListParticipantEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListParticipantEventsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListParticipantEventsRequestRequestTypeDef(
+    _RequiredListParticipantEventsRequestRequestTypeDef,
+    _OptionalListParticipantEventsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListParticipantsRequestRequestTypeDef = TypedDict(
+    "_RequiredListParticipantsRequestRequestTypeDef",
+    {
+        "sessionId": str,
+        "stageArn": str,
+    },
+)
+_OptionalListParticipantsRequestRequestTypeDef = TypedDict(
+    "_OptionalListParticipantsRequestRequestTypeDef",
+    {
+        "filterByPublished": bool,
+        "filterByState": ParticipantStateType,
+        "filterByUserId": str,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListParticipantsRequestRequestTypeDef(
+    _RequiredListParticipantsRequestRequestTypeDef, _OptionalListParticipantsRequestRequestTypeDef
+):
+    pass
+
+
+ParticipantSummaryTypeDef = TypedDict(
+    "ParticipantSummaryTypeDef",
+    {
+        "firstJoinTime": datetime,
+        "participantId": str,
+        "published": bool,
+        "state": ParticipantStateType,
+        "userId": str,
+    },
+    total=False,
+)
+
+_RequiredListStageSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListStageSessionsRequestRequestTypeDef",
+    {
+        "stageArn": str,
+    },
+)
+_OptionalListStageSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListStageSessionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListStageSessionsRequestRequestTypeDef(
+    _RequiredListStageSessionsRequestRequestTypeDef, _OptionalListStageSessionsRequestRequestTypeDef
+):
+    pass
+
+
+StageSessionSummaryTypeDef = TypedDict(
+    "StageSessionSummaryTypeDef",
+    {
+        "endTime": datetime,
+        "sessionId": str,
+        "startTime": datetime,
+    },
+    total=False,
+)
+
 ListStagesRequestRequestTypeDef = TypedDict(
     "ListStagesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -199,14 +354,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -240,23 +414,15 @@
     pass
 
 
 CreateParticipantTokenResponseTypeDef = TypedDict(
     "CreateParticipantTokenResponseTypeDef",
     {
         "participantToken": ParticipantTokenTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStageRequestRequestTypeDef = TypedDict(
     "CreateStageRequestRequestTypeDef",
     {
         "name": str,
@@ -267,35 +433,78 @@
 )
 
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
         "participantTokens": List[ParticipantTokenTypeDef],
         "stage": StageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
         "stage": StageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
         "stage": StageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListParticipantEventsResponseTypeDef = TypedDict(
+    "ListParticipantEventsResponseTypeDef",
+    {
+        "events": List[EventTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetParticipantResponseTypeDef = TypedDict(
+    "GetParticipantResponseTypeDef",
+    {
+        "participant": ParticipantTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetStageSessionResponseTypeDef = TypedDict(
+    "GetStageSessionResponseTypeDef",
+    {
+        "stageSession": StageSessionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListParticipantsResponseTypeDef = TypedDict(
+    "ListParticipantsResponseTypeDef",
+    {
+        "nextToken": str,
+        "participants": List[ParticipantSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStageSessionsResponseTypeDef = TypedDict(
+    "ListStageSessionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "stageSessions": List[StageSessionSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStagesResponseTypeDef = TypedDict(
     "ListStagesResponseTypeDef",
     {
         "nextToken": str,
         "stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/PKG-INFO` & `mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs-realtime
-Version: 1.26.98
-Summary: Type annotations for boto3.ivsrealtime 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ivsrealtime 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ivs-realtime"></a>
 
 # mypy-boto3-ivs-realtime
 
 [![PyPI - mypy-boto3-ivs-realtime](https://img.shields.io/pypi/v/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs-realtime?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.ivsrealtime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -276,54 +276,73 @@
 ### Literals
 
 `mypy_boto3_ivs_realtime.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.literals import (
+    EventErrorCodeType,
+    EventNameType,
+    ParticipantStateType,
     ParticipantTokenCapabilityType,
     ivsrealtimeServiceName,
     ServiceName,
     ResourceServiceName,
+    RegionName,
 )
 
 
-def check_value(value: ParticipantTokenCapabilityType) -> bool:
+def check_value(value: EventErrorCodeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import (
     CreateParticipantTokenRequestRequestTypeDef,
     ParticipantTokenTypeDef,
-    ResponseMetadataTypeDef,
     ParticipantTokenConfigurationTypeDef,
     StageTypeDef,
     DeleteStageRequestRequestTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
+    EventTypeDef,
+    GetParticipantRequestRequestTypeDef,
+    ParticipantTypeDef,
     GetStageRequestRequestTypeDef,
+    GetStageSessionRequestRequestTypeDef,
+    StageSessionTypeDef,
+    ListParticipantEventsRequestRequestTypeDef,
+    ListParticipantsRequestRequestTypeDef,
+    ParticipantSummaryTypeDef,
+    ListStageSessionsRequestRequestTypeDef,
+    StageSessionSummaryTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     CreateParticipantTokenResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     UpdateStageResponseTypeDef,
+    ListParticipantEventsResponseTypeDef,
+    GetParticipantResponseTypeDef,
+    GetStageSessionResponseTypeDef,
+    ListParticipantsResponseTypeDef,
+    ListStageSessionsResponseTypeDef,
     ListStagesResponseTypeDef,
 )
 
 
 def get_structure() -> CreateParticipantTokenRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-ivs-realtime-1.26.98/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt` & `mypy-boto3-ivs-realtime-1.27.0/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.26.98/setup.py` & `mypy-boto3-ivs-realtime-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs-realtime",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_ivs_realtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ivsrealtime 1.26.98 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.ivsrealtime 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


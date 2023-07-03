# Comparing `tmp/mypy-boto3-mediapackagev2-1.26.137.tar.gz` & `tmp/mypy-boto3-mediapackagev2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackagev2-1.26.137.tar", last modified: Fri May 19 19:32:21 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackagev2-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
```

## Comparing `mypy-boto3-mediapackagev2-1.26.137.tar` & `mypy-boto3-mediapackagev2-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:21.624119 mypy-boto3-mediapackagev2-1.26.137/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-05-19 19:32:21.624119 mypy-boto3-mediapackagev2-1.26.137/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:21.624119 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-19 19:32:04.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-05-19 19:32:04.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:32:21.624119 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-05-19 19:32:21.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-19 19:32:21.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:32:21.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:32:21.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 19:32:21.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 19:32:21.000000 mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:32:21.624119 mypy-boto3-mediapackagev2-1.26.137/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-19 19:32:03.000000 mypy-boto3-mediapackagev2-1.26.137/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.495649 mypy-boto3-mediapackagev2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-03 19:51:06.487649 mypy-boto3-mediapackagev2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.483648 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-03 19:42:07.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-03 19:42:08.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-03 19:42:08.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-03 19:42:07.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-03 19:42:07.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26978 2023-07-03 19:42:09.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-07-03 19:42:09.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.487649 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-03 19:51:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:51:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:06.000000 mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.495649 mypy-boto3-mediapackagev2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:42:06.000000 mypy-boto3-mediapackagev2-1.27.0/setup.py
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/LICENSE` & `mypy-boto3-mediapackagev2-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.26.137/PKG-INFO` & `mypy-boto3-mediapackagev2-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.26.137
-Summary: Type annotations for boto3.mediapackagev2 1.26.137 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.mediapackagev2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackagev2?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.26.137](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -323,14 +323,15 @@
     PresetSpeke20VideoType,
     ScteFilterType,
     TsEncryptionMethodType,
     mediapackagev2ServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
@@ -342,64 +343,64 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateChannelGroupResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     IngestEndpointTypeDef,
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
+    GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
+    GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
+    GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHlsManifestConfigurationTypeDef,
     ListLowLatencyHlsManifestConfigurationTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
+    UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelGroupResponseTypeDef,
-    GetChannelPolicyResponseTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
     SpekeKeyProviderTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     OriginEndpointListConfigurationTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/README.md` & `mypy-boto3-mediapackagev2-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackagev2?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.26.137](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -291,14 +291,15 @@
     PresetSpeke20VideoType,
     ScteFilterType,
     TsEncryptionMethodType,
     mediapackagev2ServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
@@ -310,64 +311,64 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateChannelGroupResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     IngestEndpointTypeDef,
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
+    GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
+    GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
+    GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHlsManifestConfigurationTypeDef,
     ListLowLatencyHlsManifestConfigurationTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
+    UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelGroupResponseTypeDef,
-    GetChannelPolicyResponseTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
     SpekeKeyProviderTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     OriginEndpointListConfigurationTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/__init__.py` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/__init__.pyi` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/__main__.py` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mediapackagev2 1.26.137\nVersion:         1.26.137\nBuilder"
+        "Type annotations for boto3.mediapackagev2 1.27.0\nVersion:         1.27.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.137")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/client.py` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/client.pyi` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/literals.py` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "PresetSpeke20VideoType",
     "ScteFilterType",
     "TsEncryptionMethodType",
     "mediapackagev2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 
 AdMarkerHlsType = Literal["DATERANGE"]
 CmafEncryptionMethodType = Literal["CBCS", "CENC"]
 ContainerTypeType = Literal["CMAF", "TS"]
 DrmSystemType = Literal["CLEAR_KEY_AES_128", "FAIRPLAY", "PLAYREADY", "WIDEVINE"]
@@ -84,14 +85,15 @@
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
@@ -131,14 +133,15 @@
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
@@ -310,14 +313,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
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
@@ -401,14 +406,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
@@ -429,7 +435,24 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_channel_groups", "list_channels", "list_origin_endpoints"]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/literals.pyi` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/literals.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "PresetSpeke20VideoType",
     "ScteFilterType",
     "TsEncryptionMethodType",
     "mediapackagev2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 AdMarkerHlsType = Literal["DATERANGE"]
 CmafEncryptionMethodType = Literal["CBCS", "CENC"]
 ContainerTypeType = Literal["CMAF", "TS"]
 DrmSystemType = Literal["CLEAR_KEY_AES_128", "FAIRPLAY", "PLAYREADY", "WIDEVINE"]
 ListChannelGroupsPaginatorName = Literal["list_channel_groups"]
@@ -82,14 +83,15 @@
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
@@ -129,14 +131,15 @@
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
@@ -308,14 +311,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
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
@@ -399,14 +404,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
@@ -427,7 +433,24 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_channel_groups", "list_channels", "list_origin_endpoints"]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/paginator.py` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,30 +50,30 @@
 class ListChannelGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, ChannelGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
         """
 
 
@@ -84,13 +84,13 @@
     """
 
     def paginate(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/paginator.pyi` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,29 @@
 class ListChannelGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannelGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelgroupspaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, ChannelGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listchannelspaginator)
         """
 
 class ListOriginEndpointsPaginator(Paginator):
@@ -79,13 +79,13 @@
     """
 
     def paginate(
         self,
         *,
         ChannelGroupName: str,
         ChannelName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOriginEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2.Paginator.ListOriginEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/paginators/#listoriginendpointspaginator)
         """
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/type_defs.py` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,64 +35,64 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateChannelGroupResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "EncryptionMethodTypeDef",
     "GetChannelGroupRequestRequestTypeDef",
+    "GetChannelGroupResponseTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
+    "GetChannelPolicyResponseTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
+    "GetOriginEndpointPolicyResponseTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
+    "UpdateChannelGroupResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "CreateChannelGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetChannelGroupResponseTypeDef",
-    "GetChannelPolicyResponseTypeDef",
-    "GetOriginEndpointPolicyResponseTypeDef",
     "ListChannelGroupsResponseTypeDef",
     "ListChannelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateChannelGroupResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
     "SpekeKeyProviderTypeDef",
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
@@ -169,22 +169,25 @@
 class CreateChannelGroupRequestRequestTypeDef(
     _RequiredCreateChannelGroupRequestRequestTypeDef,
     _OptionalCreateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateChannelGroupResponseTypeDef = TypedDict(
+    "CreateChannelGroupResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -262,14 +265,21 @@
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
@@ -286,22 +296,46 @@
 GetChannelGroupRequestRequestTypeDef = TypedDict(
     "GetChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 
+GetChannelGroupResponseTypeDef = TypedDict(
+    "GetChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -311,42 +345,73 @@
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
+GetOriginEndpointPolicyResponseTypeDef = TypedDict(
+    "GetOriginEndpointPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "OriginEndpointName": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetOriginEndpointRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelGroupsRequestRequestTypeDef = TypedDict(
     "ListChannelGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+    },
+)
+_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListChannelsRequestListChannelsPaginateTypeDef(
+    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
+    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalListChannelsRequestRequestTypeDef = TypedDict(
@@ -406,14 +471,37 @@
 class ListLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredListLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalListLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
 
+_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+    },
+)
+_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
+    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -437,14 +525,32 @@
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
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "Policy": str,
     },
@@ -456,14 +562,25 @@
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "Policy": str,
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
 ScteTypeDef = TypedDict(
     "ScteTypeDef",
     {
         "ScteFilter": Sequence[ScteFilterType],
     },
     total=False,
 )
@@ -502,14 +619,28 @@
 class UpdateChannelGroupRequestRequestTypeDef(
     _RequiredUpdateChannelGroupRequestRequestTypeDef,
     _OptionalUpdateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateChannelGroupResponseTypeDef = TypedDict(
+    "UpdateChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -524,152 +655,74 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-CreateChannelGroupResponseTypeDef = TypedDict(
-    "CreateChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
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
-GetChannelGroupResponseTypeDef = TypedDict(
-    "GetChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOriginEndpointPolicyResponseTypeDef = TypedDict(
-    "GetOriginEndpointPolicyResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "OriginEndpointName": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListChannelGroupsResponseTypeDef = TypedDict(
     "ListChannelGroupsResponseTypeDef",
     {
         "Items": List[ChannelGroupListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Items": List[ChannelListConfigurationTypeDef],
         "NextToken": str,
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
-UpdateChannelGroupResponseTypeDef = TypedDict(
-    "UpdateChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
@@ -776,67 +829,14 @@
         "ResourceId": str,
         "DrmSystems": Sequence[DrmSystemType],
         "RoleArn": str,
         "Url": str,
     },
 )
 
-ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-    },
-)
-_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListChannelsRequestListChannelsPaginateTypeDef(
-    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
-    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-    },
-)
-_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
-    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -884,15 +884,15 @@
 
 
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentDurationSeconds": int,
@@ -949,15 +949,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOriginEndpointResponseTypeDef = TypedDict(
     "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -969,15 +969,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -1018,10 +1018,10 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2/type_defs.pyi` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,64 +34,64 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChannelGroupListConfigurationTypeDef",
     "ChannelListConfigurationTypeDef",
     "CreateChannelGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateChannelGroupResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "IngestEndpointTypeDef",
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "EncryptionMethodTypeDef",
     "GetChannelGroupRequestRequestTypeDef",
+    "GetChannelGroupResponseTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
+    "GetChannelPolicyResponseTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
+    "GetOriginEndpointPolicyResponseTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListHlsManifestConfigurationTypeDef",
     "ListLowLatencyHlsManifestConfigurationTypeDef",
+    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
+    "UpdateChannelGroupResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "CreateChannelGroupResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetChannelGroupResponseTypeDef",
-    "GetChannelPolicyResponseTypeDef",
-    "GetOriginEndpointPolicyResponseTypeDef",
     "ListChannelGroupsResponseTypeDef",
     "ListChannelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateChannelGroupResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
     "SpekeKeyProviderTypeDef",
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
     "OriginEndpointListConfigurationTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
     "SegmentTypeDef",
     "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
@@ -162,22 +162,25 @@
 
 class CreateChannelGroupRequestRequestTypeDef(
     _RequiredCreateChannelGroupRequestRequestTypeDef,
     _OptionalCreateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateChannelGroupResponseTypeDef = TypedDict(
+    "CreateChannelGroupResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -253,14 +256,21 @@
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
@@ -277,22 +287,46 @@
 GetChannelGroupRequestRequestTypeDef = TypedDict(
     "GetChannelGroupRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 
+GetChannelGroupResponseTypeDef = TypedDict(
+    "GetChannelGroupResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "Arn": str,
+        "EgressDomain": str,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelPolicyRequestRequestTypeDef = TypedDict(
     "GetChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
+GetChannelPolicyResponseTypeDef = TypedDict(
+    "GetChannelPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -302,42 +336,71 @@
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
+GetOriginEndpointPolicyResponseTypeDef = TypedDict(
+    "GetOriginEndpointPolicyResponseTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+        "OriginEndpointName": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetOriginEndpointRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
+    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListChannelGroupsRequestRequestTypeDef = TypedDict(
     "ListChannelGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+    },
+)
+_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListChannelsRequestListChannelsPaginateTypeDef(
+    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
+    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
+):
+    pass
+
 _RequiredListChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
     },
 )
 _OptionalListChannelsRequestRequestTypeDef = TypedDict(
@@ -391,14 +454,35 @@
 
 class ListLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredListLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalListLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "ChannelGroupName": str,
+        "ChannelName": str,
+    },
+)
+_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
+    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
+):
+    pass
+
 _RequiredListOriginEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListOriginEndpointsRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
@@ -420,14 +504,32 @@
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
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "Policy": str,
     },
@@ -439,14 +541,25 @@
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "Policy": str,
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
 ScteTypeDef = TypedDict(
     "ScteTypeDef",
     {
         "ScteFilter": Sequence[ScteFilterType],
     },
     total=False,
 )
@@ -483,172 +596,108 @@
 
 class UpdateChannelGroupRequestRequestTypeDef(
     _RequiredUpdateChannelGroupRequestRequestTypeDef,
     _OptionalUpdateChannelGroupRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelRequestRequestTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-    },
-)
-_OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateChannelRequestRequestTypeDef(
-    _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
-):
-    pass
-
-CreateChannelGroupResponseTypeDef = TypedDict(
-    "CreateChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
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
-GetChannelGroupResponseTypeDef = TypedDict(
-    "GetChannelGroupResponseTypeDef",
+UpdateChannelGroupResponseTypeDef = TypedDict(
+    "UpdateChannelGroupResponseTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
         "EgressDomain": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetChannelPolicyResponseTypeDef = TypedDict(
-    "GetChannelPolicyResponseTypeDef",
+_RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-GetOriginEndpointPolicyResponseTypeDef = TypedDict(
-    "GetOriginEndpointPolicyResponseTypeDef",
+_OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateChannelRequestRequestTypeDef",
     {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-        "OriginEndpointName": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Description": str,
     },
+    total=False,
 )
 
+class UpdateChannelRequestRequestTypeDef(
+    _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
+):
+    pass
+
 ListChannelGroupsResponseTypeDef = TypedDict(
     "ListChannelGroupsResponseTypeDef",
     {
         "Items": List[ChannelGroupListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Items": List[ChannelListConfigurationTypeDef],
         "NextToken": str,
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
-UpdateChannelGroupResponseTypeDef = TypedDict(
-    "UpdateChannelGroupResponseTypeDef",
-    {
-        "ChannelGroupName": str,
-        "Arn": str,
-        "EgressDomain": str,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelGroupName": str,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "IngestEndpoints": List[IngestEndpointTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredCreateHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
@@ -747,63 +796,14 @@
         "ResourceId": str,
         "DrmSystems": Sequence[DrmSystemType],
         "RoleArn": str,
         "Url": str,
     },
 )
 
-ListChannelGroupsRequestListChannelGroupsPaginateTypeDef = TypedDict(
-    "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-    },
-)
-_OptionalListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListChannelsRequestListChannelsPaginateTypeDef(
-    _RequiredListChannelsRequestListChannelsPaginateTypeDef,
-    _OptionalListChannelsRequestListChannelsPaginateTypeDef,
-):
-    pass
-
-_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "ChannelGroupName": str,
-        "ChannelName": str,
-    },
-)
-_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(
-    _RequiredListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-    _OptionalListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
-):
-    pass
-
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -847,15 +847,15 @@
     pass
 
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentDurationSeconds": int,
@@ -910,15 +910,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOriginEndpointResponseTypeDef = TypedDict(
     "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
@@ -930,15 +930,15 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
@@ -977,10 +977,10 @@
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/PKG-INFO` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.26.137
-Summary: Type annotations for boto3.mediapackagev2 1.26.137 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.mediapackagev2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackagev2?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.26.137](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -323,14 +323,15 @@
     PresetSpeke20VideoType,
     ScteFilterType,
     TsEncryptionMethodType,
     mediapackagev2ServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AdMarkerHlsType) -> bool:
     ...
 ```
 
@@ -342,64 +343,64 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackagev2.type_defs import (
     ChannelGroupListConfigurationTypeDef,
     ChannelListConfigurationTypeDef,
     CreateChannelGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateChannelGroupResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     IngestEndpointTypeDef,
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionContractConfigurationTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
+    GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
+    GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
+    GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHlsManifestConfigurationTypeDef,
     ListLowLatencyHlsManifestConfigurationTypeDef,
+    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
+    UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    CreateChannelGroupResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChannelGroupResponseTypeDef,
-    GetChannelPolicyResponseTypeDef,
-    GetOriginEndpointPolicyResponseTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateChannelGroupResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
     SpekeKeyProviderTypeDef,
-    ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
     OriginEndpointListConfigurationTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
     SegmentTypeDef,
     CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-mediapackagev2-1.26.137/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt` & `mypy-boto3-mediapackagev2-1.27.0/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.26.137/setup.py` & `mypy-boto3-mediapackagev2-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackagev2",
-    version="1.26.137",
+    version="1.27.0",
     packages=["mypy_boto3_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mediapackagev2 1.26.137 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.mediapackagev2 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


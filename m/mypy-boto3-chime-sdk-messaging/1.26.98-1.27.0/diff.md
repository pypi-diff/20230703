# Comparing `tmp/mypy-boto3-chime-sdk-messaging-1.26.98.tar.gz` & `tmp/mypy-boto3-chime-sdk-messaging-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-messaging-1.26.98.tar` & `mypy-boto3-chime-sdk-messaging-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-03-23 19:32:02.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48068 2023-03-23 19:32:03.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48007 2023-03-23 19:32:03.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.718914 mypy-boto3-chime-sdk-messaging-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-03 19:50:27.714913 mypy-boto3-chime-sdk-messaging-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16808 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.710914 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47641 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47584 2023-07-03 19:33:29.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.714913 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.718914 mypy-boto3-chime-sdk-messaging-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-03 19:33:28.000000 mypy-boto3-chime-sdk-messaging-1.27.0/setup.py
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/LICENSE` & `mypy-boto3-chime-sdk-messaging-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-messaging"></a>
 
 # mypy-boto3-chime-sdk-messaging
 
 [![PyPI - mypy-boto3-chime-sdk-messaging](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,27 +318,30 @@
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
+    TargetTypeDef,
     ElasticChannelConfigurationTypeDef,
     ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -346,14 +349,15 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
@@ -366,50 +370,47 @@
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    UpdateChannelFlowResponseTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
-    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
-    ChannelMessageSummaryTypeDef,
-    ChannelMessageTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    ChannelMessageSummaryTypeDef,
+    ChannelMessageTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/README.md` & `mypy-boto3-chime-sdk-messaging-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-messaging"></a>
 
 # mypy-boto3-chime-sdk-messaging
 
 [![PyPI - mypy-boto3-chime-sdk-messaging](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,27 +286,30 @@
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
+    TargetTypeDef,
     ElasticChannelConfigurationTypeDef,
     ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -314,14 +317,15 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
@@ -334,50 +338,47 @@
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    UpdateChannelFlowResponseTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
-    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
-    ChannelMessageSummaryTypeDef,
-    ChannelMessageTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    ChannelMessageSummaryTypeDef,
+    ChannelMessageTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__main__.py` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMessaging 1.26.98\nVersion:         1.26.98\nBuilder"
-        " version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMessaging 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.py` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,44 +70,42 @@
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
+    TargetTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 __all__ = ("ChimeSDKMessagingClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottledClientException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
 
-
 class ChimeSDKMessagingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/)
     """
 
     meta: ClientMeta
@@ -116,25 +114,23 @@
     def exceptions(self) -> Exceptions:
         """
         ChimeSDKMessagingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#exceptions)
         """
-
     def associate_channel_flow(
         self, *, ChannelArn: str, ChannelFlowArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates a channel flow with a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.associate_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#associate_channel_flow)
         """
-
     def batch_create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArns: Sequence[str],
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
@@ -142,46 +138,42 @@
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
         Adds a specified number of users and bots to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.batch_create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#batch_create_channel_membership)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#can_paginate)
         """
-
     def channel_flow_callback(
         self,
         *,
         CallbackId: str,
         ChannelArn: str,
         ChannelMessage: ChannelMessageCallbackTypeDef,
         DeleteResource: bool = ...
     ) -> ChannelFlowCallbackResponseTypeDef:
         """
-        Calls back Chime SDK Messaging with a processing response message.
+        Calls back Amazon Chime SDK messaging with a processing response message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.channel_flow_callback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#channel_flow_callback)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#close)
         """
-
     def create_channel(
         self,
         *,
         AppInstanceArn: str,
         Name: str,
         ClientRequestToken: str,
         ChimeBearer: str,
@@ -197,25 +189,23 @@
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel)
         """
-
     def create_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> CreateChannelBanResponseTypeDef:
         """
         Permanently bans a member from a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_ban)
         """
-
     def create_channel_flow(
         self,
         *,
         AppInstanceArn: str,
         Processors: Sequence[ProcessorTypeDef],
         Name: str,
         ClientRequestToken: str,
@@ -223,15 +213,14 @@
     ) -> CreateChannelFlowResponseTypeDef:
         """
         Creates a channel flow, a container for processors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_flow)
         """
-
     def create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
         ChimeBearer: str,
@@ -239,257 +228,230 @@
     ) -> CreateChannelMembershipResponseTypeDef:
         """
         Adds a member to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_membership)
         """
-
     def create_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> CreateChannelModeratorResponseTypeDef:
         """
         Creates a new `ChannelModerator`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_moderator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_moderator)
         """
-
-    def delete_channel(
-        self, *, ChannelArn: str, ChimeBearer: str, SubChannelId: str = ...
-    ) -> EmptyResponseMetadataTypeDef:
+    def delete_channel(self, *, ChannelArn: str, ChimeBearer: str) -> EmptyResponseMetadataTypeDef:
         """
         Immediately makes a channel and its memberships inaccessible and marks them for
         deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel)
         """
-
     def delete_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a member from a channel's ban list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_ban)
         """
-
     def delete_channel_flow(self, *, ChannelFlowArn: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel flow, an irreversible process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_flow)
         """
-
     def delete_channel_membership(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a member from a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_membership)
         """
-
     def delete_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_message)
         """
-
     def delete_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel moderator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_moderator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_moderator)
         """
-
     def delete_messaging_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the streaming configurations for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_messaging_streaming_configurations)
         """
-
     def describe_channel(
         self, *, ChannelArn: str, ChimeBearer: str
     ) -> DescribeChannelResponseTypeDef:
         """
         Returns the full details of a channel in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel)
         """
-
     def describe_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> DescribeChannelBanResponseTypeDef:
         """
         Returns the full details of a channel ban.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_ban)
         """
-
     def describe_channel_flow(self, *, ChannelFlowArn: str) -> DescribeChannelFlowResponseTypeDef:
         """
         Returns the full details of a channel flow in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_flow)
         """
-
     def describe_channel_membership(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> DescribeChannelMembershipResponseTypeDef:
         """
         Returns the full details of a user's channel membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership)
         """
-
     def describe_channel_membership_for_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
         """
         Returns the details of a channel based on the membership of the specified
         `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_membership_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership_for_app_instance_user)
         """
-
     def describe_channel_moderated_by_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
         """
         Returns the full details of a channel moderated by the specified
         `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_moderated_by_app_instance_user)
         """
-
     def describe_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratorResponseTypeDef:
         """
         Returns the full details of a single ChannelModerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_moderator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_moderator)
         """
-
     def disassociate_channel_flow(
         self, *, ChannelArn: str, ChannelFlowArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disassociates a channel flow from all its channels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.disassociate_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#disassociate_channel_flow)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#generate_presigned_url)
         """
-
     def get_channel_membership_preferences(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> GetChannelMembershipPreferencesResponseTypeDef:
         """
         Gets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
         the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_membership_preferences)
         """
-
     def get_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> GetChannelMessageResponseTypeDef:
         """
         Gets the full details of a channel message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_message)
         """
-
     def get_channel_message_status(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> GetChannelMessageStatusResponseTypeDef:
         """
         Gets message status for a specified `messageId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_message_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_message_status)
         """
-
     def get_messaging_session_endpoint(self) -> GetMessagingSessionEndpointResponseTypeDef:
         """
         The details of the endpoint for the messaging session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_messaging_session_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_messaging_session_endpoint)
         """
-
     def get_messaging_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> GetMessagingStreamingConfigurationsResponseTypeDef:
         """
         Retrieves the data streaming configuration for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_messaging_streaming_configurations)
         """
-
     def list_channel_bans(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelBansResponseTypeDef:
         """
         Lists all the users and bots banned from a particular channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_bans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_bans)
         """
-
     def list_channel_flows(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelFlowsResponseTypeDef:
         """
         Returns a paginated lists of all the channel flows created under a single Chime.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_flows)
         """
-
     def list_channel_memberships(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
         MaxResults: int = ...,
@@ -498,30 +460,28 @@
     ) -> ListChannelMembershipsResponseTypeDef:
         """
         Lists all channel memberships in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_memberships)
         """
-
     def list_channel_memberships_for_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
-        Lists all channels that anr `AppInstanceUser` or `AppInstanceBot` is a part of.
+        Lists all channels that an `AppInstanceUser` or `AppInstanceBot` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_memberships_for_app_instance_user)
         """
-
     def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
         NotBefore: Union[datetime, str] = ...,
@@ -532,25 +492,23 @@
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_messages)
         """
-
     def list_channel_moderators(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelModeratorsResponseTypeDef:
         """
         Lists all the moderators for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_moderators)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_moderators)
         """
-
     def list_channels(
         self,
         *,
         AppInstanceArn: str,
         ChimeBearer: str,
         Privacy: ChannelPrivacyType = ...,
         MaxResults: int = ...,
@@ -558,169 +516,157 @@
     ) -> ListChannelsResponseTypeDef:
         """
         Lists all Channels created under a single Chime App as a paginated list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels)
         """
-
     def list_channels_associated_with_channel_flow(
         self, *, ChannelFlowArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsAssociatedWithChannelFlowResponseTypeDef:
         """
         Lists all channels associated with a specified channel flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_associated_with_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels_associated_with_channel_flow)
         """
-
     def list_channels_moderated_by_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
         A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels_moderated_by_app_instance_user)
         """
-
     def list_sub_channels(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSubChannelsResponseTypeDef:
         """
         Lists all the SubChannels in an elastic channel when given a channel ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_sub_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_sub_channels)
         """
-
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags applied to an Amazon Chime SDK messaging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_tags_for_resource)
         """
-
     def put_channel_expiration_settings(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str = ...,
         ExpirationSettings: ExpirationSettingsTypeDef = ...
     ) -> PutChannelExpirationSettingsResponseTypeDef:
         """
         Sets the number of days before the channel is automatically deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_expiration_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_expiration_settings)
         """
-
     def put_channel_membership_preferences(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         ChimeBearer: str,
         Preferences: ChannelMembershipPreferencesTypeDef
     ) -> PutChannelMembershipPreferencesResponseTypeDef:
         """
-        Sets the membership preferences of an `AppInstanceUser` or `AppIntanceBot` for
+        Sets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
         the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_membership_preferences)
         """
-
     def put_messaging_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
         StreamingConfigurations: Sequence[StreamingConfigurationTypeDef]
     ) -> PutMessagingStreamingConfigurationsResponseTypeDef:
         """
         Sets the data streaming configuration for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_messaging_streaming_configurations)
         """
-
     def redact_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> RedactChannelMessageResponseTypeDef:
         """
         Redacts message content, but not metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.redact_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#redact_channel_message)
         """
-
     def search_channels(
         self,
         *,
         Fields: Sequence[SearchFieldTypeDef],
         ChimeBearer: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SearchChannelsResponseTypeDef:
         """
         Allows the `ChimeBearer` to search channels by channel members.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.search_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#search_channels)
         """
-
     def send_channel_message(
         self,
         *,
         ChannelArn: str,
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         SubChannelId: str = ...,
-        ContentType: str = ...
+        ContentType: str = ...,
+        Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.send_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#send_channel_message)
         """
-
     def tag_resource(
         self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Applies the specified tags to the specified Amazon Chime SDK messaging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#tag_resource)
         """
-
     def untag_resource(
         self, *, ResourceARN: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the specified tags from the specified Amazon Chime SDK messaging
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#untag_resource)
         """
-
     def update_channel(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Name: str = ...,
         Mode: ChannelModeType = ...,
@@ -728,25 +674,23 @@
     ) -> UpdateChannelResponseTypeDef:
         """
         Update a channel's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel)
         """
-
     def update_channel_flow(
         self, *, ChannelFlowArn: str, Processors: Sequence[ProcessorTypeDef], Name: str
     ) -> UpdateChannelFlowResponseTypeDef:
         """
         Updates channel flow attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_flow)
         """
-
     def update_channel_message(
         self,
         *,
         ChannelArn: str,
         MessageId: str,
         Content: str,
         ChimeBearer: str,
@@ -756,17 +700,16 @@
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_message)
         """
-
     def update_channel_read_marker(
-        self, *, ChannelArn: str, ChimeBearer: str, SubChannelId: str = ...
+        self, *, ChannelArn: str, ChimeBearer: str
     ) -> UpdateChannelReadMarkerResponseTypeDef:
         """
         The details of the time when a user last read messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_read_marker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_read_marker)
         """
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.pyi` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,41 +70,45 @@
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
+    TargetTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 __all__ = ("ChimeSDKMessagingClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ServiceFailureException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottledClientException: Type[BotocoreClientError]
     UnauthorizedClientException: Type[BotocoreClientError]
 
+
 class ChimeSDKMessagingClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/)
     """
 
     meta: ClientMeta
@@ -113,23 +117,25 @@
     def exceptions(self) -> Exceptions:
         """
         ChimeSDKMessagingClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#exceptions)
         """
+
     def associate_channel_flow(
         self, *, ChannelArn: str, ChannelFlowArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates a channel flow with a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.associate_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#associate_channel_flow)
         """
+
     def batch_create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArns: Sequence[str],
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
@@ -137,42 +143,46 @@
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
         Adds a specified number of users and bots to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.batch_create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#batch_create_channel_membership)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#can_paginate)
         """
+
     def channel_flow_callback(
         self,
         *,
         CallbackId: str,
         ChannelArn: str,
         ChannelMessage: ChannelMessageCallbackTypeDef,
         DeleteResource: bool = ...
     ) -> ChannelFlowCallbackResponseTypeDef:
         """
-        Calls back Chime SDK Messaging with a processing response message.
+        Calls back Amazon Chime SDK messaging with a processing response message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.channel_flow_callback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#channel_flow_callback)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#close)
         """
+
     def create_channel(
         self,
         *,
         AppInstanceArn: str,
         Name: str,
         ClientRequestToken: str,
         ChimeBearer: str,
@@ -188,23 +198,25 @@
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel)
         """
+
     def create_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> CreateChannelBanResponseTypeDef:
         """
         Permanently bans a member from a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_ban)
         """
+
     def create_channel_flow(
         self,
         *,
         AppInstanceArn: str,
         Processors: Sequence[ProcessorTypeDef],
         Name: str,
         ClientRequestToken: str,
@@ -212,14 +224,15 @@
     ) -> CreateChannelFlowResponseTypeDef:
         """
         Creates a channel flow, a container for processors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_flow)
         """
+
     def create_channel_membership(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
         ChimeBearer: str,
@@ -227,232 +240,255 @@
     ) -> CreateChannelMembershipResponseTypeDef:
         """
         Adds a member to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_membership)
         """
+
     def create_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> CreateChannelModeratorResponseTypeDef:
         """
         Creates a new `ChannelModerator`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_moderator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_moderator)
         """
-    def delete_channel(
-        self, *, ChannelArn: str, ChimeBearer: str, SubChannelId: str = ...
-    ) -> EmptyResponseMetadataTypeDef:
+
+    def delete_channel(self, *, ChannelArn: str, ChimeBearer: str) -> EmptyResponseMetadataTypeDef:
         """
         Immediately makes a channel and its memberships inaccessible and marks them for
         deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel)
         """
+
     def delete_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a member from a channel's ban list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_ban)
         """
+
     def delete_channel_flow(self, *, ChannelFlowArn: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel flow, an irreversible process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_flow)
         """
+
     def delete_channel_membership(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a member from a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_membership)
         """
+
     def delete_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_message)
         """
+
     def delete_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel moderator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_moderator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_moderator)
         """
+
     def delete_messaging_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the streaming configurations for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_messaging_streaming_configurations)
         """
+
     def describe_channel(
         self, *, ChannelArn: str, ChimeBearer: str
     ) -> DescribeChannelResponseTypeDef:
         """
         Returns the full details of a channel in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel)
         """
+
     def describe_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> DescribeChannelBanResponseTypeDef:
         """
         Returns the full details of a channel ban.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_ban)
         """
+
     def describe_channel_flow(self, *, ChannelFlowArn: str) -> DescribeChannelFlowResponseTypeDef:
         """
         Returns the full details of a channel flow in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_flow)
         """
+
     def describe_channel_membership(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> DescribeChannelMembershipResponseTypeDef:
         """
         Returns the full details of a user's channel membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership)
         """
+
     def describe_channel_membership_for_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
         """
         Returns the details of a channel based on the membership of the specified
         `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_membership_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership_for_app_instance_user)
         """
+
     def describe_channel_moderated_by_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
         """
         Returns the full details of a channel moderated by the specified
         `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_moderated_by_app_instance_user)
         """
+
     def describe_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratorResponseTypeDef:
         """
         Returns the full details of a single ChannelModerator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_moderator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_moderator)
         """
+
     def disassociate_channel_flow(
         self, *, ChannelArn: str, ChannelFlowArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disassociates a channel flow from all its channels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.disassociate_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#disassociate_channel_flow)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#generate_presigned_url)
         """
+
     def get_channel_membership_preferences(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> GetChannelMembershipPreferencesResponseTypeDef:
         """
         Gets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
         the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_membership_preferences)
         """
+
     def get_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> GetChannelMessageResponseTypeDef:
         """
         Gets the full details of a channel message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_message)
         """
+
     def get_channel_message_status(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> GetChannelMessageStatusResponseTypeDef:
         """
         Gets message status for a specified `messageId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_message_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_message_status)
         """
+
     def get_messaging_session_endpoint(self) -> GetMessagingSessionEndpointResponseTypeDef:
         """
         The details of the endpoint for the messaging session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_messaging_session_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_messaging_session_endpoint)
         """
+
     def get_messaging_streaming_configurations(
         self, *, AppInstanceArn: str
     ) -> GetMessagingStreamingConfigurationsResponseTypeDef:
         """
         Retrieves the data streaming configuration for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_messaging_streaming_configurations)
         """
+
     def list_channel_bans(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelBansResponseTypeDef:
         """
         Lists all the users and bots banned from a particular channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_bans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_bans)
         """
+
     def list_channel_flows(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelFlowsResponseTypeDef:
         """
         Returns a paginated lists of all the channel flows created under a single Chime.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_flows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_flows)
         """
+
     def list_channel_memberships(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
         MaxResults: int = ...,
@@ -461,28 +497,30 @@
     ) -> ListChannelMembershipsResponseTypeDef:
         """
         Lists all channel memberships in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_memberships)
         """
+
     def list_channel_memberships_for_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
-        Lists all channels that anr `AppInstanceUser` or `AppInstanceBot` is a part of.
+        Lists all channels that an `AppInstanceUser` or `AppInstanceBot` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_memberships_for_app_instance_user)
         """
+
     def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
         NotBefore: Union[datetime, str] = ...,
@@ -493,23 +531,25 @@
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_messages)
         """
+
     def list_channel_moderators(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelModeratorsResponseTypeDef:
         """
         Lists all the moderators for a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_moderators)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_moderators)
         """
+
     def list_channels(
         self,
         *,
         AppInstanceArn: str,
         ChimeBearer: str,
         Privacy: ChannelPrivacyType = ...,
         MaxResults: int = ...,
@@ -517,156 +557,170 @@
     ) -> ListChannelsResponseTypeDef:
         """
         Lists all Channels created under a single Chime App as a paginated list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels)
         """
+
     def list_channels_associated_with_channel_flow(
         self, *, ChannelFlowArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsAssociatedWithChannelFlowResponseTypeDef:
         """
         Lists all channels associated with a specified channel flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_associated_with_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels_associated_with_channel_flow)
         """
+
     def list_channels_moderated_by_app_instance_user(
         self,
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
         A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels_moderated_by_app_instance_user)
         """
+
     def list_sub_channels(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSubChannelsResponseTypeDef:
         """
         Lists all the SubChannels in an elastic channel when given a channel ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_sub_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_sub_channels)
         """
+
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags applied to an Amazon Chime SDK messaging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_tags_for_resource)
         """
+
     def put_channel_expiration_settings(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str = ...,
         ExpirationSettings: ExpirationSettingsTypeDef = ...
     ) -> PutChannelExpirationSettingsResponseTypeDef:
         """
         Sets the number of days before the channel is automatically deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_expiration_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_expiration_settings)
         """
+
     def put_channel_membership_preferences(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         ChimeBearer: str,
         Preferences: ChannelMembershipPreferencesTypeDef
     ) -> PutChannelMembershipPreferencesResponseTypeDef:
         """
-        Sets the membership preferences of an `AppInstanceUser` or `AppIntanceBot` for
+        Sets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
         the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_membership_preferences)
         """
+
     def put_messaging_streaming_configurations(
         self,
         *,
         AppInstanceArn: str,
         StreamingConfigurations: Sequence[StreamingConfigurationTypeDef]
     ) -> PutMessagingStreamingConfigurationsResponseTypeDef:
         """
         Sets the data streaming configuration for an `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_messaging_streaming_configurations)
         """
+
     def redact_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> RedactChannelMessageResponseTypeDef:
         """
         Redacts message content, but not metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.redact_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#redact_channel_message)
         """
+
     def search_channels(
         self,
         *,
         Fields: Sequence[SearchFieldTypeDef],
         ChimeBearer: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SearchChannelsResponseTypeDef:
         """
         Allows the `ChimeBearer` to search channels by channel members.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.search_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#search_channels)
         """
+
     def send_channel_message(
         self,
         *,
         ChannelArn: str,
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         SubChannelId: str = ...,
-        ContentType: str = ...
+        ContentType: str = ...,
+        Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.send_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#send_channel_message)
         """
+
     def tag_resource(
         self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Applies the specified tags to the specified Amazon Chime SDK messaging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#tag_resource)
         """
+
     def untag_resource(
         self, *, ResourceARN: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the specified tags from the specified Amazon Chime SDK messaging
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#untag_resource)
         """
+
     def update_channel(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         Name: str = ...,
         Mode: ChannelModeType = ...,
@@ -674,23 +728,25 @@
     ) -> UpdateChannelResponseTypeDef:
         """
         Update a channel's attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel)
         """
+
     def update_channel_flow(
         self, *, ChannelFlowArn: str, Processors: Sequence[ProcessorTypeDef], Name: str
     ) -> UpdateChannelFlowResponseTypeDef:
         """
         Updates channel flow attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_flow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_flow)
         """
+
     def update_channel_message(
         self,
         *,
         ChannelArn: str,
         MessageId: str,
         Content: str,
         ChimeBearer: str,
@@ -700,16 +756,17 @@
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_message)
         """
+
     def update_channel_read_marker(
-        self, *, ChannelArn: str, ChimeBearer: str, SubChannelId: str = ...
+        self, *, ChannelArn: str, ChimeBearer: str
     ) -> UpdateChannelReadMarkerResponseTypeDef:
         """
         The details of the time when a user last read messages in a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_read_marker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_read_marker)
         """
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.py` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AllowNotificationsType",
     "ChannelMembershipTypeType",
     "ChannelMessagePersistenceTypeType",
     "ChannelMessageStatusType",
     "ChannelMessageTypeType",
     "ChannelModeType",
@@ -38,15 +37,14 @@
     "SortOrderType",
     "ChimeSDKMessagingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AllowNotificationsType = Literal["ALL", "FILTERED", "NONE"]
 ChannelMembershipTypeType = Literal["DEFAULT", "HIDDEN"]
 ChannelMessagePersistenceTypeType = Literal["NON_PERSISTENT", "PERSISTENT"]
 ChannelMessageStatusType = Literal["DENIED", "FAILED", "PENDING", "SENT"]
 ChannelMessageTypeType = Literal["CONTROL", "STANDARD"]
 ChannelModeType = Literal["RESTRICTED", "UNRESTRICTED"]
 ChannelPrivacyType = Literal["PRIVATE", "PUBLIC"]
@@ -87,14 +85,15 @@
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
@@ -134,14 +133,15 @@
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
@@ -283,14 +283,15 @@
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
@@ -309,16 +310,19 @@
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
@@ -402,15 +406,17 @@
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.pyi` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AllowNotificationsType",
     "ChannelMembershipTypeType",
     "ChannelMessagePersistenceTypeType",
     "ChannelMessageStatusType",
     "ChannelMessageTypeType",
     "ChannelModeType",
@@ -37,14 +38,15 @@
     "SortOrderType",
     "ChimeSDKMessagingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AllowNotificationsType = Literal["ALL", "FILTERED", "NONE"]
 ChannelMembershipTypeType = Literal["DEFAULT", "HIDDEN"]
 ChannelMessagePersistenceTypeType = Literal["NON_PERSISTENT", "PERSISTENT"]
 ChannelMessageStatusType = Literal["DENIED", "FAILED", "PENDING", "SENT"]
 ChannelMessageTypeType = Literal["CONTROL", "STANDARD"]
 ChannelModeType = Literal["RESTRICTED", "UNRESTRICTED"]
 ChannelPrivacyType = Literal["PRIVATE", "PUBLIC"]
@@ -85,14 +87,15 @@
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
@@ -132,14 +135,15 @@
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
@@ -281,14 +285,15 @@
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
@@ -307,16 +312,19 @@
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
@@ -400,15 +408,17 @@
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

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.py` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,30 @@
 
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
+    "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
+    "TargetTypeDef",
     "ElasticChannelConfigurationTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
+    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
+    "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
@@ -72,14 +75,15 @@
     "DescribeChannelFlowRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelMembershipRequestRequestTypeDef",
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociateChannelFlowRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
@@ -92,50 +96,47 @@
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "UpdateChannelResponseTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
-    "ChannelFlowCallbackResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
-    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
-    "CreateChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "UpdateChannelFlowResponseTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
-    "ChannelMessageSummaryTypeDef",
-    "ChannelMessageTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
+    "ChannelMessageSummaryTypeDef",
+    "ChannelMessageTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -231,37 +232,35 @@
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
 ):
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
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
     },
     total=False,
 )
 
+ChannelFlowCallbackResponseTypeDef = TypedDict(
+    "ChannelFlowCallbackResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "CallbackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -315,14 +314,22 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
+    {
+        "MemberArn": str,
+    },
+    total=False,
+)
+
 ElasticChannelConfigurationTypeDef = TypedDict(
     "ElasticChannelConfigurationTypeDef",
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
@@ -349,14 +356,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateChannelFlowResponseTypeDef = TypedDict(
+    "CreateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateChannelMembershipRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelMembershipRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "Type": ChannelMembershipTypeType,
         "ChimeBearer": str,
@@ -383,14 +398,22 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteChannelBanRequestRequestTypeDef = TypedDict(
     "DeleteChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -456,35 +479,21 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
-_RequiredDeleteChannelRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteChannelRequestRequestTypeDef",
+DeleteChannelRequestRequestTypeDef = TypedDict(
+    "DeleteChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
-_OptionalDeleteChannelRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteChannelRequestRequestTypeDef",
-    {
-        "SubChannelId": str,
-    },
-    total=False,
-)
-
-
-class DeleteChannelRequestRequestTypeDef(
-    _RequiredDeleteChannelRequestRequestTypeDef, _OptionalDeleteChannelRequestRequestTypeDef
-):
-    pass
-
 
 DeleteMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
@@ -569,14 +578,21 @@
     {
         "ChannelArn": str,
         "ChannelFlowArn": str,
         "ChimeBearer": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -937,14 +953,35 @@
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "SubChannelId": str,
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
 SearchFieldTypeDef = TypedDict(
     "SearchFieldTypeDef",
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
@@ -954,14 +991,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateChannelFlowResponseTypeDef = TypedDict(
+    "UpdateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Content": str,
         "ChimeBearer": str,
@@ -981,37 +1026,30 @@
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
+UpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
+    "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
-_OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelReadMarkerRequestRequestTypeDef",
+
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
     {
-        "SubChannelId": str,
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class UpdateChannelReadMarkerRequestRequestTypeDef(
-    _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
-    _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -1028,14 +1066,22 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchChannelMembershipsTypeDef = TypedDict(
     "BatchChannelMembershipsTypeDef",
     {
         "InvitedBy": IdentityTypeDef,
         "Type": ChannelMembershipTypeType,
         "Members": List[IdentityTypeDef],
         "ChannelArn": str,
@@ -1100,115 +1146,48 @@
         "ChannelArn": str,
         "CreatedTimestamp": datetime,
         "CreatedBy": IdentityTypeDef,
     },
     total=False,
 )
 
-ChannelFlowCallbackResponseTypeDef = TypedDict(
-    "ChannelFlowCallbackResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "CallbackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateChannelFlowResponseTypeDef = TypedDict(
-    "CreateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelModeratorResponseTypeDef = TypedDict(
     "CreateChannelModeratorResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
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
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChannelFlowResponseTypeDef = TypedDict(
-    "UpdateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsAssociatedWithChannelFlowResponseTypeDef = TypedDict(
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     {
         "Channels": List[ChannelAssociatedWithFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -1226,24 +1205,24 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchChannelsResponseTypeDef = TypedDict(
     "SearchChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
@@ -1273,44 +1252,43 @@
 
 class ChannelMessageCallbackTypeDef(
     _RequiredChannelMessageCallbackTypeDef, _OptionalChannelMessageCallbackTypeDef
 ):
     pass
 
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
+GetChannelMessageStatusResponseTypeDef = TypedDict(
+    "GetChannelMessageStatusResponseTypeDef",
     {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
+        "Status": ChannelMessageStatusStructureTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
+
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
     {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "ChannelArn": str,
+        "MessageId": str,
+        "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "Status": ChannelMessageStatusStructureTypeDef,
+        "SubChannelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
@@ -1319,14 +1297,15 @@
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "ContentType": str,
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1341,48 +1320,51 @@
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
         "ContentType": str,
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
-GetChannelMessageStatusResponseTypeDef = TypedDict(
-    "GetChannelMessageStatusResponseTypeDef",
-    {
-        "Status": ChannelMessageStatusStructureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "MessageId": str,
-        "Status": ChannelMessageStatusStructureTypeDef,
-        "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
     },
 )
-
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "Status": ChannelMessageStatusStructureTypeDef,
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
     },
+    total=False,
 )
 
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1422,15 +1404,15 @@
 
 
 PutChannelExpirationSettingsResponseTypeDef = TypedDict(
     "PutChannelExpirationSettingsResponseTypeDef",
     {
         "ChannelArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1462,15 +1444,15 @@
     pass
 
 
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
@@ -1478,23 +1460,23 @@
     },
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1502,15 +1484,15 @@
     },
 )
 
 PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
@@ -1519,15 +1501,15 @@
 
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
@@ -1551,113 +1533,113 @@
 
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelBansResponseTypeDef = TypedDict(
     "ListChannelBansResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelBans": List[ChannelBanSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelBanResponseTypeDef = TypedDict(
     "DescribeChannelBanResponseTypeDef",
     {
         "ChannelBan": ChannelBanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelMembershipsResponseTypeDef = TypedDict(
     "ListChannelMembershipsResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelMemberships": List[ChannelMembershipSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelMembershipResponseTypeDef = TypedDict(
     "DescribeChannelMembershipResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelModeratorsResponseTypeDef = TypedDict(
     "ListChannelModeratorsResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelModerators": List[ChannelModeratorSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelModeratorResponseTypeDef = TypedDict(
     "DescribeChannelModeratorResponseTypeDef",
     {
         "ChannelModerator": ChannelModeratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelMembershipsForAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     {
         "ChannelMemberships": List[ChannelMembershipForAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channel": ChannelModeratedByAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channels": List[ChannelModeratedByAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
@@ -1669,15 +1651,15 @@
 
 PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1704,31 +1686,31 @@
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelMessageResponseTypeDef = TypedDict(
     "GetChannelMessageResponseTypeDef",
     {
         "ChannelMessage": ChannelMessageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
@@ -1794,18 +1776,18 @@
 )
 
 ListChannelFlowsResponseTypeDef = TypedDict(
     "ListChannelFlowsResponseTypeDef",
     {
         "ChannelFlows": List[ChannelFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelFlowResponseTypeDef = TypedDict(
     "DescribeChannelFlowResponseTypeDef",
     {
         "ChannelFlow": ChannelFlowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.pyi` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,30 @@
 
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
+    "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
+    "TargetTypeDef",
     "ElasticChannelConfigurationTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
+    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
+    "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
@@ -71,14 +74,15 @@
     "DescribeChannelFlowRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelMembershipRequestRequestTypeDef",
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociateChannelFlowRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
@@ -91,50 +95,47 @@
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "UpdateChannelResponseTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
-    "ChannelFlowCallbackResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
-    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
-    "CreateChannelResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "UpdateChannelFlowResponseTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
-    "ChannelMessageSummaryTypeDef",
-    "ChannelMessageTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
+    "ChannelMessageSummaryTypeDef",
+    "ChannelMessageTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -228,37 +229,35 @@
 
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
 ):
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
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
     },
     total=False,
 )
 
+ChannelFlowCallbackResponseTypeDef = TypedDict(
+    "ChannelFlowCallbackResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "CallbackId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -310,14 +309,22 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
+    {
+        "MemberArn": str,
+    },
+    total=False,
+)
+
 ElasticChannelConfigurationTypeDef = TypedDict(
     "ElasticChannelConfigurationTypeDef",
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
@@ -344,14 +351,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateChannelFlowResponseTypeDef = TypedDict(
+    "CreateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateChannelMembershipRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelMembershipRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "Type": ChannelMembershipTypeType,
         "ChimeBearer": str,
@@ -376,14 +391,22 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteChannelBanRequestRequestTypeDef = TypedDict(
     "DeleteChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -445,33 +468,21 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
-_RequiredDeleteChannelRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteChannelRequestRequestTypeDef",
+DeleteChannelRequestRequestTypeDef = TypedDict(
+    "DeleteChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
-_OptionalDeleteChannelRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteChannelRequestRequestTypeDef",
-    {
-        "SubChannelId": str,
-    },
-    total=False,
-)
-
-class DeleteChannelRequestRequestTypeDef(
-    _RequiredDeleteChannelRequestRequestTypeDef, _OptionalDeleteChannelRequestRequestTypeDef
-):
-    pass
 
 DeleteMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
@@ -554,14 +565,21 @@
     {
         "ChannelArn": str,
         "ChannelFlowArn": str,
         "ChimeBearer": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -896,14 +914,35 @@
 
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "SubChannelId": str,
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
 SearchFieldTypeDef = TypedDict(
     "SearchFieldTypeDef",
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
@@ -913,14 +952,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateChannelFlowResponseTypeDef = TypedDict(
+    "UpdateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Content": str,
         "ChimeBearer": str,
@@ -938,35 +985,30 @@
 
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
+UpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
+    "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
-_OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelReadMarkerRequestRequestTypeDef",
+
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
     {
-        "SubChannelId": str,
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class UpdateChannelReadMarkerRequestRequestTypeDef(
-    _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
-    _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -981,14 +1023,22 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchChannelMembershipsTypeDef = TypedDict(
     "BatchChannelMembershipsTypeDef",
     {
         "InvitedBy": IdentityTypeDef,
         "Type": ChannelMembershipTypeType,
         "Members": List[IdentityTypeDef],
         "ChannelArn": str,
@@ -1053,115 +1103,48 @@
         "ChannelArn": str,
         "CreatedTimestamp": datetime,
         "CreatedBy": IdentityTypeDef,
     },
     total=False,
 )
 
-ChannelFlowCallbackResponseTypeDef = TypedDict(
-    "ChannelFlowCallbackResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "CallbackId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateChannelFlowResponseTypeDef = TypedDict(
-    "CreateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelModeratorResponseTypeDef = TypedDict(
     "CreateChannelModeratorResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
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
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChannelFlowResponseTypeDef = TypedDict(
-    "UpdateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsAssociatedWithChannelFlowResponseTypeDef = TypedDict(
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     {
         "Channels": List[ChannelAssociatedWithFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -1179,24 +1162,24 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchChannelsResponseTypeDef = TypedDict(
     "SearchChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
@@ -1224,42 +1207,43 @@
 )
 
 class ChannelMessageCallbackTypeDef(
     _RequiredChannelMessageCallbackTypeDef, _OptionalChannelMessageCallbackTypeDef
 ):
     pass
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
+GetChannelMessageStatusResponseTypeDef = TypedDict(
+    "GetChannelMessageStatusResponseTypeDef",
     {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
+        "Status": ChannelMessageStatusStructureTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
+
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
     {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "ChannelArn": str,
+        "MessageId": str,
+        "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "Status": ChannelMessageStatusStructureTypeDef,
+        "SubChannelId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
@@ -1268,14 +1252,15 @@
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "ContentType": str,
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1290,48 +1275,49 @@
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
         "ContentType": str,
+        "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
-GetChannelMessageStatusResponseTypeDef = TypedDict(
-    "GetChannelMessageStatusResponseTypeDef",
-    {
-        "Status": ChannelMessageStatusStructureTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
-        "MessageId": str,
-        "Status": ChannelMessageStatusStructureTypeDef,
-        "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
     },
 )
-
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "Status": ChannelMessageStatusStructureTypeDef,
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
     },
+    total=False,
 )
 
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1369,15 +1355,15 @@
     pass
 
 PutChannelExpirationSettingsResponseTypeDef = TypedDict(
     "PutChannelExpirationSettingsResponseTypeDef",
     {
         "ChannelArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1407,15 +1393,15 @@
 ):
     pass
 
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
@@ -1423,23 +1409,23 @@
     },
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1447,15 +1433,15 @@
     },
 )
 
 PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
@@ -1464,15 +1450,15 @@
 
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
@@ -1494,113 +1480,113 @@
     pass
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelBansResponseTypeDef = TypedDict(
     "ListChannelBansResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelBans": List[ChannelBanSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelBanResponseTypeDef = TypedDict(
     "DescribeChannelBanResponseTypeDef",
     {
         "ChannelBan": ChannelBanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelMembershipsResponseTypeDef = TypedDict(
     "ListChannelMembershipsResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelMemberships": List[ChannelMembershipSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelMembershipResponseTypeDef = TypedDict(
     "DescribeChannelMembershipResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelModeratorsResponseTypeDef = TypedDict(
     "ListChannelModeratorsResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelModerators": List[ChannelModeratorSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelModeratorResponseTypeDef = TypedDict(
     "DescribeChannelModeratorResponseTypeDef",
     {
         "ChannelModerator": ChannelModeratorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelMembershipsForAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     {
         "ChannelMemberships": List[ChannelMembershipForAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channel": ChannelModeratedByAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListChannelsModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channels": List[ChannelModeratedByAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
@@ -1612,15 +1598,15 @@
 
 PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1645,31 +1631,31 @@
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelMessageResponseTypeDef = TypedDict(
     "GetChannelMessageResponseTypeDef",
     {
         "ChannelMessage": ChannelMessageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
@@ -1733,18 +1719,18 @@
 )
 
 ListChannelFlowsResponseTypeDef = TypedDict(
     "ListChannelFlowsResponseTypeDef",
     {
         "ChannelFlows": List[ChannelFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelFlowResponseTypeDef = TypedDict(
     "DescribeChannelFlowResponseTypeDef",
     {
         "ChannelFlow": ChannelFlowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-messaging"></a>
 
 # mypy-boto3-chime-sdk-messaging
 
 [![PyPI - mypy-boto3-chime-sdk-messaging](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,27 +318,30 @@
 ```python
 from mypy_boto3_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
+    TargetTypeDef,
     ElasticChannelConfigurationTypeDef,
     ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -346,14 +349,15 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
@@ -366,50 +370,47 @@
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    UpdateChannelFlowResponseTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
-    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
-    ChannelMessageSummaryTypeDef,
-    ChannelMessageTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    ChannelMessageSummaryTypeDef,
+    ChannelMessageTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-messaging-1.27.0/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.98/setup.py` & `mypy-boto3-chime-sdk-messaging-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-messaging",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMessaging 1.26.98 service generated with"
-        " mypy-boto3-builder 7.14.2"
+        "Type annotations for boto3.ChimeSDKMessaging 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


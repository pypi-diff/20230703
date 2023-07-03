# Comparing `tmp/mypy-boto3-chime-1.26.164.tar.gz` & `tmp/mypy-boto3-chime-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-1.26.164.tar", last modified: Thu Jun 29 20:25:42 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-chime-1.26.164.tar` & `mypy-boto3-chime-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.248377 mypy-boto3-chime-1.26.164/mypy_boto3_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-29 20:24:32.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144436 2023-06-29 20:24:36.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144277 2023-06-29 20:24:34.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-29 20:24:31.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 20:25:42.000000 mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:25:42.252378 mypy-boto3-chime-1.26.164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-29 20:24:30.000000 mypy-boto3-chime-1.26.164/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.158904 mypy-boto3-chime-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32557 2023-07-03 19:50:27.154904 mypy-boto3-chime-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31080 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.150904 mypy-boto3-chime-1.27.0/mypy_boto3_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121396 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121196 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-03 19:33:19.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-07-03 19:33:19.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-03 19:33:19.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144728 2023-07-03 19:33:23.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144569 2023-07-03 19:33:21.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.150904 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32557 2023-07-03 19:50:26.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:50:27.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:26.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:50:26.000000 mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.158904 mypy-boto3-chime-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:33:18.000000 mypy-boto3-chime-1.27.0/setup.py
```

### Comparing `mypy-boto3-chime-1.26.164/LICENSE` & `mypy-boto3-chime-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/PKG-INFO` & `mypy-boto3-chime-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.26.164
-Summary: Type annotations for boto3.Chime 1.26.164 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Chime 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -388,15 +388,14 @@
     AppInstanceUserTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
-    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
@@ -409,19 +408,23 @@
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -471,14 +474,15 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
@@ -488,14 +492,15 @@
     GetEventsConfigurationRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -512,15 +517,15 @@
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
@@ -540,59 +545,72 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
+    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
+    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
+    SendChannelMessageResponseTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
+    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
+    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    UpdateChannelResponseTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
     AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
@@ -603,49 +621,33 @@
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccountSettingsResponseTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SendChannelMessageResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
-    UpdateChannelMessageResponseTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
-    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -710,16 +712,14 @@
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
```

### Comparing `mypy-boto3-chime-1.26.164/README.md` & `mypy-boto3-chime-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -356,15 +356,14 @@
     AppInstanceUserTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
-    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
@@ -377,19 +376,23 @@
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -439,14 +442,15 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
@@ -456,14 +460,15 @@
     GetEventsConfigurationRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -480,15 +485,15 @@
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
@@ -508,59 +513,72 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
+    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
+    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
+    SendChannelMessageResponseTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
+    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
+    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    UpdateChannelResponseTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
     AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
@@ -571,49 +589,33 @@
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccountSettingsResponseTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SendChannelMessageResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
-    UpdateChannelMessageResponseTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
-    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -678,16 +680,14 @@
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.py` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/__init__.pyi` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/__main__.py` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Chime 1.26.164\nVersion:         1.26.164\nBuilder version:"
+        "Type annotations for boto3.Chime 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.164")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.py` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/client.pyi` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.py` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/literals.pyi` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.py` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listaccountspaginator)
         """
 
 
@@ -68,13 +68,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/paginator.pyi` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listaccountspaginator)
         """
 
 class ListUsersPaginator(Paginator):
@@ -64,13 +64,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.py` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     "AppInstanceUserTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
@@ -106,19 +105,23 @@
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
+    "CreateChannelResponseTypeDef",
     "CreateMeetingDialOutRequestRequestTypeDef",
+    "CreateMeetingDialOutResponseTypeDef",
     "MeetingNotificationConfigurationTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateRoomMembershipRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
@@ -168,14 +171,15 @@
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociatePhoneNumberFromUserRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
@@ -185,14 +189,15 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
@@ -209,15 +214,15 @@
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationTypeDef",
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
@@ -237,59 +242,72 @@
     "ListRoomMembershipsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
+    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
+    "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
+    "SendChannelMessageResponseTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
+    "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "UpdateChannelResponseTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
+    "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
     "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
@@ -300,49 +318,33 @@
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateChannelBanResponseTypeDef",
+    "CreateChannelMembershipResponseTypeDef",
+    "CreateChannelModeratorResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "DescribeAppInstanceUserResponseTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
-    "CreateChannelBanResponseTypeDef",
-    "CreateChannelMembershipResponseTypeDef",
-    "CreateChannelModeratorResponseTypeDef",
-    "CreateChannelResponseTypeDef",
-    "CreateMeetingDialOutResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "DescribeAppInstanceUserResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAccountSettingsResponseTypeDef",
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    "SendChannelMessageResponseTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
-    "UpdateChannelMessageResponseTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -407,16 +409,14 @@
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
@@ -716,25 +716,14 @@
         "PhoneNumberId": str,
         "ErrorCode": ErrorCodeType,
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
 _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -960,14 +949,30 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "DisplayName": str,
     },
 )
@@ -1051,24 +1056,40 @@
 class CreateChannelModeratorRequestRequestTypeDef(
     _RequiredCreateChannelModeratorRequestRequestTypeDef,
     _OptionalCreateChannelModeratorRequestRequestTypeDef,
 ):
     pass
 
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateMeetingDialOutRequestRequestTypeDef = TypedDict(
     "CreateMeetingDialOutRequestRequestTypeDef",
     {
         "MeetingId": str,
         "FromPhoneNumber": str,
         "ToPhoneNumber": str,
         "JoinToken": str,
     },
 )
 
+CreateMeetingDialOutResponseTypeDef = TypedDict(
+    "CreateMeetingDialOutResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MeetingNotificationConfigurationTypeDef = TypedDict(
     "MeetingNotificationConfigurationTypeDef",
     {
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
     total=False,
@@ -1767,14 +1788,21 @@
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     {
         "AccountId": str,
         "GroupNames": Sequence[str],
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
@@ -1943,14 +1971,23 @@
 GetPhoneNumberRequestRequestTypeDef = TypedDict(
     "GetPhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
+GetPhoneNumberSettingsResponseTypeDef = TypedDict(
+    "GetPhoneNumberSettingsResponseTypeDef",
+    {
+        "CallingName": str,
+        "CallingNameUpdatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetProxySessionRequestRequestTypeDef = TypedDict(
     "GetProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "ProxySessionId": str,
     },
 )
@@ -2148,20 +2185,20 @@
 
 class InviteUsersRequestRequestTypeDef(
     _RequiredInviteUsersRequestRequestTypeDef, _OptionalInviteUsersRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "UserEmail": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccountsRequestRequestTypeDef = TypedDict(
     "ListAccountsRequestRequestTypeDef",
     {
@@ -2580,14 +2617,38 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserEmail": str,
+        "UserType": UserTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -2620,14 +2681,22 @@
 ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    {
+        "Usernames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVoiceConnectorsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -2685,14 +2754,24 @@
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
         "Weight": int,
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
 ParticipantTypeDef = TypedDict(
     "ParticipantTypeDef",
     {
         "PhoneNumber": str,
         "ProxyPhoneNumber": str,
     },
     total=False,
@@ -2789,14 +2868,23 @@
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RedactConversationMessageRequestRequestTypeDef = TypedDict(
     "RedactConversationMessageRequestRequestTypeDef",
     {
         "AccountId": str,
         "ConversationId": str,
         "MessageId": str,
     },
@@ -2823,14 +2911,25 @@
     "ResetPersonalPINRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -2853,14 +2952,23 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    {
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -2889,14 +2997,23 @@
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -2981,14 +3098,22 @@
 
 class UpdateAppInstanceRequestRequestTypeDef(
     _RequiredUpdateAppInstanceRequestRequestTypeDef, _OptionalUpdateAppInstanceRequestRequestTypeDef
 ):
     pass
 
 
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
     },
 )
@@ -3004,14 +3129,22 @@
 class UpdateAppInstanceUserRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
@@ -3051,14 +3184,23 @@
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
@@ -3073,14 +3215,22 @@
 class UpdateChannelReadMarkerRequestRequestTypeDef(
     _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
     _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Mode": ChannelModeType,
     },
@@ -3097,14 +3247,22 @@
 
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
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -3227,14 +3385,22 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
+GetAccountSettingsResponseTypeDef = TypedDict(
+    "GetAccountSettingsResponseTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "AccountSettings": AccountSettingsTypeDef,
     },
 )
@@ -3484,337 +3650,205 @@
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-AppInstanceRetentionSettingsTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsTypeDef",
-    {
-        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
-    },
-    total=False,
-)
-
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
-    },
-)
-
-ArtifactsConfigurationTypeDef = TypedDict(
-    "ArtifactsConfigurationTypeDef",
-    {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
-    },
-)
-
-AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchDeletePhoneNumberResponseTypeDef = TypedDict(
-    "BatchDeletePhoneNumberResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
-    "BatchUpdatePhoneNumberResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
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
-CreateMeetingDialOutResponseTypeDef = TypedDict(
-    "CreateMeetingDialOutResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
-    {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppInstanceUserResponseTypeDef = TypedDict(
-    "DescribeAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
-GetAccountSettingsResponseTypeDef = TypedDict(
-    "GetAccountSettingsResponseTypeDef",
+AppInstanceRetentionSettingsTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsTypeDef",
     {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
+    total=False,
 )
 
 GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     {
         "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
     },
 )
 
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppInstancesResponseTypeDef = TypedDict(
     "ListAppInstancesResponseTypeDef",
     {
         "AppInstances": List[AppInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
     {
-        "Usernames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
+DescribeAppInstanceUserResponseTypeDef = TypedDict(
+    "DescribeAppInstanceUserResponseTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceUser": AppInstanceUserTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+ArtifactsConfigurationTypeDef = TypedDict(
+    "ArtifactsConfigurationTypeDef",
     {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
     },
 )
 
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
+AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
+AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
+BatchDeletePhoneNumberResponseTypeDef = TypedDict(
+    "BatchDeletePhoneNumberResponseTypeDef",
     {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
+BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
+    "BatchUpdatePhoneNumberResponseTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
-        "ChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
-        "ChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateRoomMembershipRequestRequestTypeDef = TypedDict(
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -3823,98 +3857,98 @@
     },
 )
 
 BatchCreateRoomMembershipResponseTypeDef = TypedDict(
     "BatchCreateRoomMembershipResponseTypeDef",
     {
         "Errors": List[MemberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchSuspendUserResponseTypeDef = TypedDict(
     "BatchSuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUnsuspendUserResponseTypeDef = TypedDict(
     "BatchUnsuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateUserResponseTypeDef = TypedDict(
     "BatchUpdateUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "Bots": List[BotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegenerateSecurityTokenResponseTypeDef = TypedDict(
     "RegenerateSecurityTokenResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -3932,15 +3966,15 @@
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
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -4059,31 +4093,31 @@
     pass
 
 
 ListAttendeeTagsResponseTypeDef = TypedDict(
     "ListAttendeeTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMeetingTagsResponseTypeDef = TypedDict(
     "ListMeetingTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -4161,56 +4195,56 @@
     pass
 
 
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "Rooms": List[RoomTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "CreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
@@ -4361,40 +4395,40 @@
     total=False,
 )
 
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorResponseTypeDef = TypedDict(
     "GetVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4433,32 +4467,32 @@
     total=False,
 )
 
 GetEventsConfigurationResponseTypeDef = TypedDict(
     "GetEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEventsConfigurationResponseTypeDef = TypedDict(
     "PutEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsRequestRequestTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
@@ -4467,23 +4501,23 @@
     total=False,
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
@@ -4505,23 +4539,23 @@
     pass
 
 
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4529,47 +4563,47 @@
     },
 )
 
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorProxyResponseTypeDef = TypedDict(
     "PutVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorTerminationHealthResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     {
         "TerminationHealth": TerminationHealthTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4577,65 +4611,31 @@
     },
 )
 
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "ListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "Name": str,
-        "UserEmail": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserEmail": str,
-        "UserType": UserTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
@@ -4766,40 +4766,40 @@
     },
 )
 
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "Accounts": List[AccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountResponseTypeDef = TypedDict(
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateUserRequestRequestTypeDef = TypedDict(
     "BatchUpdateUserRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -4807,164 +4807,164 @@
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetPersonalPINResponseTypeDef = TypedDict(
     "ResetPersonalPINResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
 
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
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
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -4973,49 +4973,49 @@
 )
 
 PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
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
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5050,114 +5050,114 @@
     pass
 
 
 CreateSipMediaApplicationResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipMediaApplicationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSipMediaApplicationsResponseTypeDef = TypedDict(
     "ListSipMediaApplicationsResponseTypeDef",
     {
         "SipMediaApplications": List[SipMediaApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSipMediaApplicationResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSipRuleResponseTypeDef = TypedDict(
     "CreateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipRuleResponseTypeDef = TypedDict(
     "GetSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSipRulesResponseTypeDef = TypedDict(
     "ListSipRulesResponseTypeDef",
     {
         "SipRules": List[SipRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSipRuleResponseTypeDef = TypedDict(
     "UpdateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "CreateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorGroupResponseTypeDef = TypedDict(
     "GetVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
     "ListVoiceConnectorGroupsResponseTypeDef",
     {
         "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -5165,15 +5165,15 @@
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5181,100 +5181,100 @@
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
 
 ListMeetingsResponseTypeDef = TypedDict(
     "ListMeetingsResponseTypeDef",
     {
         "Meetings": List[MeetingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRoomMembershipResponseTypeDef = TypedDict(
     "CreateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoomMembershipsResponseTypeDef = TypedDict(
     "ListRoomMembershipsResponseTypeDef",
     {
         "RoomMemberships": List[RoomMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRoomMembershipResponseTypeDef = TypedDict(
     "UpdateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPhoneNumberOrderResponseTypeDef = TypedDict(
     "GetPhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -5282,90 +5282,90 @@
     },
 )
 
 PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "PutVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProxySessionResponseTypeDef = TypedDict(
     "GetProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPhoneNumberResponseTypeDef = TypedDict(
     "GetPhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePhoneNumberResponseTypeDef = TypedDict(
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutRetentionSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -5374,15 +5374,15 @@
 )
 
 PutRetentionSettingsResponseTypeDef = TypedDict(
     "PutRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
@@ -5391,15 +5391,15 @@
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -5407,23 +5407,23 @@
     },
 )
 
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -5474,27 +5474,27 @@
     total=False,
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime/type_defs.pyi` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     "AppInstanceUserTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
@@ -105,19 +104,23 @@
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
+    "CreateChannelResponseTypeDef",
     "CreateMeetingDialOutRequestRequestTypeDef",
+    "CreateMeetingDialOutResponseTypeDef",
     "MeetingNotificationConfigurationTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateRoomMembershipRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
@@ -167,14 +170,15 @@
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociatePhoneNumberFromUserRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
@@ -184,14 +188,15 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
@@ -208,15 +213,15 @@
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationTypeDef",
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
@@ -236,59 +241,72 @@
     "ListRoomMembershipsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
+    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
+    "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
+    "SendChannelMessageResponseTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
+    "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "UpdateChannelResponseTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
+    "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
     "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
@@ -299,49 +317,33 @@
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateChannelBanResponseTypeDef",
+    "CreateChannelMembershipResponseTypeDef",
+    "CreateChannelModeratorResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "DescribeAppInstanceUserResponseTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
-    "CreateChannelBanResponseTypeDef",
-    "CreateChannelMembershipResponseTypeDef",
-    "CreateChannelModeratorResponseTypeDef",
-    "CreateChannelResponseTypeDef",
-    "CreateMeetingDialOutResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "DescribeAppInstanceUserResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAccountSettingsResponseTypeDef",
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    "SendChannelMessageResponseTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
-    "UpdateChannelMessageResponseTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -406,16 +408,14 @@
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
@@ -709,25 +709,14 @@
         "PhoneNumberId": str,
         "ErrorCode": ErrorCodeType,
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
 _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -947,14 +936,30 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "DisplayName": str,
     },
 )
@@ -1030,24 +1035,40 @@
 
 class CreateChannelModeratorRequestRequestTypeDef(
     _RequiredCreateChannelModeratorRequestRequestTypeDef,
     _OptionalCreateChannelModeratorRequestRequestTypeDef,
 ):
     pass
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateMeetingDialOutRequestRequestTypeDef = TypedDict(
     "CreateMeetingDialOutRequestRequestTypeDef",
     {
         "MeetingId": str,
         "FromPhoneNumber": str,
         "ToPhoneNumber": str,
         "JoinToken": str,
     },
 )
 
+CreateMeetingDialOutResponseTypeDef = TypedDict(
+    "CreateMeetingDialOutResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MeetingNotificationConfigurationTypeDef = TypedDict(
     "MeetingNotificationConfigurationTypeDef",
     {
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
     total=False,
@@ -1712,14 +1733,21 @@
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     {
         "AccountId": str,
         "GroupNames": Sequence[str],
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
@@ -1884,14 +1912,23 @@
 GetPhoneNumberRequestRequestTypeDef = TypedDict(
     "GetPhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
+GetPhoneNumberSettingsResponseTypeDef = TypedDict(
+    "GetPhoneNumberSettingsResponseTypeDef",
+    {
+        "CallingName": str,
+        "CallingNameUpdatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetProxySessionRequestRequestTypeDef = TypedDict(
     "GetProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "ProxySessionId": str,
     },
 )
@@ -2087,20 +2124,20 @@
 )
 
 class InviteUsersRequestRequestTypeDef(
     _RequiredInviteUsersRequestRequestTypeDef, _OptionalInviteUsersRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "UserEmail": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccountsRequestRequestTypeDef = TypedDict(
     "ListAccountsRequestRequestTypeDef",
     {
@@ -2495,14 +2532,36 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserEmail": str,
+        "UserType": UserTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -2533,14 +2592,22 @@
 ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    {
+        "Usernames": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVoiceConnectorsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -2598,14 +2665,24 @@
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
         "Weight": int,
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
 ParticipantTypeDef = TypedDict(
     "ParticipantTypeDef",
     {
         "PhoneNumber": str,
         "ProxyPhoneNumber": str,
     },
     total=False,
@@ -2696,14 +2773,23 @@
 
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RedactConversationMessageRequestRequestTypeDef = TypedDict(
     "RedactConversationMessageRequestRequestTypeDef",
     {
         "AccountId": str,
         "ConversationId": str,
         "MessageId": str,
     },
@@ -2730,14 +2816,25 @@
     "ResetPersonalPINRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -2760,14 +2857,23 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    {
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -2794,14 +2900,23 @@
 
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
 ):
     pass
 
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -2882,14 +2997,22 @@
 )
 
 class UpdateAppInstanceRequestRequestTypeDef(
     _RequiredUpdateAppInstanceRequestRequestTypeDef, _OptionalUpdateAppInstanceRequestRequestTypeDef
 ):
     pass
 
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
     },
 )
@@ -2903,14 +3026,22 @@
 
 class UpdateAppInstanceUserRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
@@ -2946,14 +3077,23 @@
 
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
@@ -2966,14 +3106,22 @@
 
 class UpdateChannelReadMarkerRequestRequestTypeDef(
     _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
     _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
 ):
     pass
 
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Mode": ChannelModeType,
     },
@@ -2988,14 +3136,22 @@
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
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -3110,14 +3266,22 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
+GetAccountSettingsResponseTypeDef = TypedDict(
+    "GetAccountSettingsResponseTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "AccountSettings": AccountSettingsTypeDef,
     },
 )
@@ -3359,337 +3523,205 @@
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-AppInstanceRetentionSettingsTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsTypeDef",
-    {
-        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
-    },
-    total=False,
-)
-
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
-    },
-)
-
-ArtifactsConfigurationTypeDef = TypedDict(
-    "ArtifactsConfigurationTypeDef",
-    {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
-    },
-)
-
-AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchDeletePhoneNumberResponseTypeDef = TypedDict(
-    "BatchDeletePhoneNumberResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
-    "BatchUpdatePhoneNumberResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
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
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateMeetingDialOutResponseTypeDef = TypedDict(
-    "CreateMeetingDialOutResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
-    {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppInstanceUserResponseTypeDef = TypedDict(
-    "DescribeAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
-GetAccountSettingsResponseTypeDef = TypedDict(
-    "GetAccountSettingsResponseTypeDef",
+AppInstanceRetentionSettingsTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsTypeDef",
     {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
+    total=False,
 )
 
 GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     {
         "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
     {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
     },
 )
 
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppInstancesResponseTypeDef = TypedDict(
     "ListAppInstancesResponseTypeDef",
     {
         "AppInstances": List[AppInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
     {
-        "Usernames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
+DescribeAppInstanceUserResponseTypeDef = TypedDict(
+    "DescribeAppInstanceUserResponseTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AppInstanceUser": AppInstanceUserTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+ArtifactsConfigurationTypeDef = TypedDict(
+    "ArtifactsConfigurationTypeDef",
     {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
     },
 )
 
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
+AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
+AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
+BatchDeletePhoneNumberResponseTypeDef = TypedDict(
+    "BatchDeletePhoneNumberResponseTypeDef",
     {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
+BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
+    "BatchUpdatePhoneNumberResponseTypeDef",
     {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
-        "ChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
+DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
-        "ChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateRoomMembershipRequestRequestTypeDef = TypedDict(
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -3698,98 +3730,98 @@
     },
 )
 
 BatchCreateRoomMembershipResponseTypeDef = TypedDict(
     "BatchCreateRoomMembershipResponseTypeDef",
     {
         "Errors": List[MemberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchSuspendUserResponseTypeDef = TypedDict(
     "BatchSuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUnsuspendUserResponseTypeDef = TypedDict(
     "BatchUnsuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateUserResponseTypeDef = TypedDict(
     "BatchUpdateUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "Bots": List[BotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegenerateSecurityTokenResponseTypeDef = TypedDict(
     "RegenerateSecurityTokenResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -3807,15 +3839,15 @@
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
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -3924,31 +3956,31 @@
 ):
     pass
 
 ListAttendeeTagsResponseTypeDef = TypedDict(
     "ListAttendeeTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMeetingTagsResponseTypeDef = TypedDict(
     "ListMeetingTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -4022,56 +4054,56 @@
 ):
     pass
 
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "Rooms": List[RoomTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "CreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
@@ -4214,40 +4246,40 @@
     total=False,
 )
 
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorResponseTypeDef = TypedDict(
     "GetVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4284,32 +4316,32 @@
     total=False,
 )
 
 GetEventsConfigurationResponseTypeDef = TypedDict(
     "GetEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutEventsConfigurationResponseTypeDef = TypedDict(
     "PutEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsRequestRequestTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
@@ -4318,23 +4350,23 @@
     total=False,
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
@@ -4354,23 +4386,23 @@
 ):
     pass
 
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4378,47 +4410,47 @@
     },
 )
 
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorProxyResponseTypeDef = TypedDict(
     "PutVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorTerminationHealthResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     {
         "TerminationHealth": TerminationHealthTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4426,63 +4458,31 @@
     },
 )
 
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
         "Termination": TerminationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "ListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "Name": str,
-        "UserEmail": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserEmail": str,
-        "UserType": UserTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
@@ -4611,40 +4611,40 @@
     },
 )
 
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "Accounts": List[AccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountResponseTypeDef = TypedDict(
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateUserRequestRequestTypeDef = TypedDict(
     "BatchUpdateUserRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -4652,164 +4652,164 @@
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetPersonalPINResponseTypeDef = TypedDict(
     "ResetPersonalPINResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
 
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
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
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -4818,49 +4818,49 @@
 )
 
 PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
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
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -4893,114 +4893,114 @@
 ):
     pass
 
 CreateSipMediaApplicationResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipMediaApplicationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSipMediaApplicationsResponseTypeDef = TypedDict(
     "ListSipMediaApplicationsResponseTypeDef",
     {
         "SipMediaApplications": List[SipMediaApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSipMediaApplicationResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSipRuleResponseTypeDef = TypedDict(
     "CreateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSipRuleResponseTypeDef = TypedDict(
     "GetSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSipRulesResponseTypeDef = TypedDict(
     "ListSipRulesResponseTypeDef",
     {
         "SipRules": List[SipRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSipRuleResponseTypeDef = TypedDict(
     "UpdateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "CreateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorGroupResponseTypeDef = TypedDict(
     "GetVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
     "ListVoiceConnectorGroupsResponseTypeDef",
     {
         "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -5008,15 +5008,15 @@
     },
 )
 
 PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5024,100 +5024,100 @@
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
 
 ListMeetingsResponseTypeDef = TypedDict(
     "ListMeetingsResponseTypeDef",
     {
         "Meetings": List[MeetingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRoomMembershipResponseTypeDef = TypedDict(
     "CreateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoomMembershipsResponseTypeDef = TypedDict(
     "ListRoomMembershipsResponseTypeDef",
     {
         "RoomMemberships": List[RoomMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRoomMembershipResponseTypeDef = TypedDict(
     "UpdateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPhoneNumberOrderResponseTypeDef = TypedDict(
     "GetPhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -5125,90 +5125,90 @@
     },
 )
 
 PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "PutVoiceConnectorOriginationResponseTypeDef",
     {
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProxySessionResponseTypeDef = TypedDict(
     "GetProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPhoneNumberResponseTypeDef = TypedDict(
     "GetPhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePhoneNumberResponseTypeDef = TypedDict(
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutRetentionSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -5217,15 +5217,15 @@
 )
 
 PutRetentionSettingsResponseTypeDef = TypedDict(
     "PutRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
@@ -5234,15 +5234,15 @@
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -5250,23 +5250,23 @@
     },
 )
 
 PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -5315,27 +5315,27 @@
     total=False,
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/PKG-INFO` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime
-Version: 1.26.164
-Summary: Type annotations for boto3.Chime 1.26.164 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Chime 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime?color=blue)](https://pypistats.org/packages/mypy-boto3-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Chime 1.26.164](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
+[boto3.Chime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -388,15 +388,14 @@
     AppInstanceUserTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
-    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
@@ -409,19 +408,23 @@
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
+    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -471,14 +474,15 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
@@ -488,14 +492,15 @@
     GetEventsConfigurationRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -512,15 +517,15 @@
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
@@ -540,59 +545,72 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
+    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
+    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
+    SendChannelMessageResponseTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
+    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
+    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    UpdateChannelResponseTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
+    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
     AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
@@ -603,49 +621,33 @@
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
-    CreateChannelResponseTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccountSettingsResponseTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
-    SendChannelMessageResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
-    UpdateChannelMessageResponseTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
-    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -710,16 +712,14 @@
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
```

### Comparing `mypy-boto3-chime-1.26.164/mypy_boto3_chime.egg-info/SOURCES.txt` & `mypy-boto3-chime-1.27.0/mypy_boto3_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-1.26.164/setup.py` & `mypy-boto3-chime-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime",
-    version="1.26.164",
+    version="1.27.0",
     packages=["mypy_boto3_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Chime 1.26.164 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Chime 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


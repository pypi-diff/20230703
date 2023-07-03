# Comparing `tmp/mypy-boto3-chime-sdk-voice-1.26.98.tar.gz` & `tmp/mypy-boto3-chime-sdk-voice-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-voice-1.27.0.tar", last modified: Mon Jul  3 19:50:28 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-voice-1.26.98.tar` & `mypy-boto3-chime-sdk-voice-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-voice-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23460 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-voice-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71962 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71860 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69354 2023-03-23 19:32:06.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69305 2023-03-23 19:32:06.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.379626 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23460 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-voice-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-23 19:32:04.000000 mypy-boto3-chime-sdk-voice-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:28.194922 mypy-boto3-chime-sdk-voice-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-03 19:50:28.186922 mypy-boto3-chime-sdk-voice-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:28.186922 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66722 2023-07-03 19:33:31.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-03 19:33:31.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-03 19:33:31.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-07-03 19:33:31.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-03 19:33:31.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-03 19:33:31.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70049 2023-07-03 19:33:32.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69998 2023-07-03 19:33:32.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:28.186922 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-03 19:50:28.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:50:28.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:28.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:28.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:28.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:50:28.000000 mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:28.194922 mypy-boto3-chime-sdk-voice-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 19:33:30.000000 mypy-boto3-chime-sdk-voice-1.27.0/setup.py
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/LICENSE` & `mypy-boto3-chime-sdk-voice-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKVoice 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKVoice 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,14 +305,15 @@
 
 `mypy_boto3_chime_sdk_voice.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.literals import (
     AlexaSkillStatusType,
+    CallLegTypeType,
     CallingNameStatusType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
     LanguageCodeType,
     ListSipMediaApplicationsPaginatorName,
     ListSipRulesPaginatorName,
@@ -349,31 +350,29 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.type_defs import (
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
-    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
     SipMediaApplicationCallTypeDef,
     SipMediaApplicationEndpointTypeDef,
+    TagTypeDef,
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
-    CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    TagTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
@@ -386,17 +385,19 @@
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -413,39 +414,45 @@
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
+    ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
+    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
+    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -459,42 +466,38 @@
     ValidateE911AddressRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
-    ListAvailableVoiceConnectorRegionsResponseTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
-    CreateSipMediaApplicationRequestRequestTypeDef,
     SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
+    CreateSipMediaApplicationRequestRequestTypeDef,
+    CreateVoiceConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
     SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
-    VoiceProfileDomainTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
@@ -509,16 +512,14 @@
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
-    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
-    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/README.md` & `mypy-boto3-chime-sdk-voice-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,14 +273,15 @@
 
 `mypy_boto3_chime_sdk_voice.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.literals import (
     AlexaSkillStatusType,
+    CallLegTypeType,
     CallingNameStatusType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
     LanguageCodeType,
     ListSipMediaApplicationsPaginatorName,
     ListSipRulesPaginatorName,
@@ -317,31 +318,29 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.type_defs import (
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
-    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
     SipMediaApplicationCallTypeDef,
     SipMediaApplicationEndpointTypeDef,
+    TagTypeDef,
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
-    CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    TagTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
@@ -354,17 +353,19 @@
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -381,39 +382,45 @@
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
+    ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
+    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
+    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -427,42 +434,38 @@
     ValidateE911AddressRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
-    ListAvailableVoiceConnectorRegionsResponseTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
-    CreateSipMediaApplicationRequestRequestTypeDef,
     SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
+    CreateSipMediaApplicationRequestRequestTypeDef,
+    CreateVoiceConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
     SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
-    VoiceProfileDomainTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
@@ -477,16 +480,14 @@
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
-    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
-    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.py` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__init__.pyi` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/__main__.py` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKVoice 1.26.98\nVersion:         1.26.98\nBuilder"
-        " version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKVoice 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice\nOther"
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

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.py` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    CallLegTypeType,
     CapabilityType,
     GeoMatchLevelType,
     NumberSelectionBehaviorType,
     PhoneNumberAssociationNameType,
     PhoneNumberProductTypeType,
     PhoneNumberTypeType,
     ProxySessionStatusType,
@@ -172,53 +173,50 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#exceptions)
         """
 
     def associate_phone_numbers_with_voice_connector(
         self, *, VoiceConnectorId: str, E164PhoneNumbers: Sequence[str], ForceAssociate: bool = ...
     ) -> AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/AssociatePhoneNumbersWithVoiceConnector).
+        Associates phone numbers with the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#associate_phone_numbers_with_voice_connector)
         """
 
     def associate_phone_numbers_with_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         E164PhoneNumbers: Sequence[str],
         ForceAssociate: bool = ...
     ) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/AssociatePhoneNumbersWithVoiceConnectorGroup).
+        Associates phone numbers with the specified Amazon Chime SDK Voice Connector
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#associate_phone_numbers_with_voice_connector_group)
         """
 
     def batch_delete_phone_number(
         self, *, PhoneNumberIds: Sequence[str]
     ) -> BatchDeletePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/BatchDeletePhoneNumber).
+        Moves phone numbers into the **Deletion queue**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_delete_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_delete_phone_number)
         """
 
     def batch_update_phone_number(
         self, *, UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef]
     ) -> BatchUpdatePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/BatchUpdatePhoneNumber).
+        Updates one or more phone numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_update_phone_number)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -236,16 +234,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#close)
         """
 
     def create_phone_number_order(
         self, *, ProductType: PhoneNumberProductTypeType, E164PhoneNumbers: Sequence[str]
     ) -> CreatePhoneNumberOrderResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreatePhoneNumberOrder).
+        Creates an order for phone numbers to be provisioned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_phone_number_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_phone_number_order)
         """
 
     def create_proxy_session(
         self,
@@ -256,27 +253,31 @@
         Name: str = ...,
         ExpiryMinutes: int = ...,
         NumberSelectionBehavior: NumberSelectionBehaviorType = ...,
         GeoMatchLevel: GeoMatchLevelType = ...,
         GeoMatchParams: GeoMatchParamsTypeDef = ...
     ) -> CreateProxySessionResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateProxySession).
+        Creates a proxy session for the specified Amazon Chime SDK Voice Connector for
+        the specified participant phone numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_proxy_session)
         """
 
     def create_sip_media_application(
-        self, *, AwsRegion: str, Name: str, Endpoints: Sequence[SipMediaApplicationEndpointTypeDef]
+        self,
+        *,
+        AwsRegion: str,
+        Name: str,
+        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],
+        Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSipMediaApplicationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateSipMediaApplication).
+        Creates a SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_media_application)
         """
 
     def create_sip_media_application_call(
         self,
@@ -284,16 +285,17 @@
         FromPhoneNumber: str,
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
         SipHeaders: Mapping[str, str] = ...,
         ArgumentsMap: Mapping[str, str] = ...
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateSipMediaApplicationCall).
+        Creates an outbound call to a phone number from the phone number specified in
+        the request, and it invokes the endpoint of the specified
+        `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application_call)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_media_application_call)
         """
 
     def create_sip_rule(
         self,
@@ -301,49 +303,53 @@
         Name: str,
         TriggerType: SipRuleTriggerTypeType,
         TriggerValue: str,
         Disabled: bool = ...,
         TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
     ) -> CreateSipRuleResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateSipRule).
+        Creates a SIP rule, which can be used to run a SIP media application as a target
+        for a specific trigger type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_rule)
         """
 
     def create_voice_connector(
-        self, *, Name: str, RequireEncryption: bool, AwsRegion: VoiceConnectorAwsRegionType = ...
+        self,
+        *,
+        Name: str,
+        RequireEncryption: bool,
+        AwsRegion: VoiceConnectorAwsRegionType = ...,
+        Tags: Sequence[TagTypeDef] = ...
     ) -> CreateVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceConnector).
+        Creates an Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector)
         """
 
     def create_voice_connector_group(
         self, *, Name: str, VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef] = ...
     ) -> CreateVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceConnectorGroup).
+        Creates an Amazon Chime SDK Voice Connector group under the administrator's AWS
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector_group)
         """
 
     def create_voice_profile(
         self, *, SpeakerSearchTaskId: str
     ) -> CreateVoiceProfileResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceProfile).
+        Creates a voice profile, which consists of an enrolled user and their latest
+        voice print.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile)
         """
 
     def create_voice_profile_domain(
         self,
@@ -351,184 +357,176 @@
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         Description: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateVoiceProfileDomainResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceProfileDomain).
+        Creates a voice profile domain, a collection of voice profiles, their voice
+        prints, and encrypted enrollment audio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile_domain)
         """
 
     def delete_phone_number(self, *, PhoneNumberId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeletePhoneNumber).
+        Moves the specified phone number into the **Deletion queue**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_phone_number)
         """
 
     def delete_proxy_session(
         self, *, VoiceConnectorId: str, ProxySessionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteProxySession).
+        Deletes the specified proxy session from the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_proxy_session)
         """
 
     def delete_sip_media_application(
         self, *, SipMediaApplicationId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteSipMediaApplication).
+        Deletes a SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_sip_media_application)
         """
 
     def delete_sip_rule(self, *, SipRuleId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteSipRule).
+        Deletes a SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_sip_rule)
         """
 
     def delete_voice_connector(self, *, VoiceConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnector).
+        Deletes an Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector)
         """
 
     def delete_voice_connector_emergency_calling_configuration(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorEmergencyCallingConfiguration).
+        Deletes the emergency calling details from the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_emergency_calling_configuration)
         """
 
     def delete_voice_connector_group(
         self, *, VoiceConnectorGroupId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorGroup).
+        Deletes an Amazon Chime SDK Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_group)
         """
 
     def delete_voice_connector_origination(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorOrigination).
+        Deletes the origination settings for the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_origination)
         """
 
     def delete_voice_connector_proxy(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorProxy).
+        Deletes the proxy configuration from the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_proxy)
         """
 
     def delete_voice_connector_streaming_configuration(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorStreamingConfiguration).
+        Deletes a Voice Connector's streaming configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_streaming_configuration)
         """
 
     def delete_voice_connector_termination(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorTermination).
+        Deletes the termination settings for the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_termination)
         """
 
     def delete_voice_connector_termination_credentials(
         self, *, VoiceConnectorId: str, Usernames: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorTerminationCredentials).
+        Deletes the specified SIP credentials used by your equipment to authenticate
+        during call termination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_termination_credentials)
         """
 
     def delete_voice_profile(self, *, VoiceProfileId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceProfile).
+        Deletes a voice profile, including its voice print and enrollment data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile)
         """
 
     def delete_voice_profile_domain(
         self, *, VoiceProfileDomainId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceProfileDomain).
+        Deletes all voice profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile_domain)
         """
 
     def disassociate_phone_numbers_from_voice_connector(
         self, *, VoiceConnectorId: str, E164PhoneNumbers: Sequence[str]
     ) -> DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DisassociatePhoneNumbersFromVoiceConnector).
+        Disassociates the specified phone numbers from the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.disassociate_phone_numbers_from_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#disassociate_phone_numbers_from_voice_connector)
         """
 
     def disassociate_phone_numbers_from_voice_connector_group(
         self, *, VoiceConnectorGroupId: str, E164PhoneNumbers: Sequence[str]
     ) -> DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DisassociatePhoneNumbersFromVoiceConnectorGroup).
+        Disassociates the specified phone numbers from the specified Amazon Chime SDK
+        Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.disassociate_phone_numbers_from_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#disassociate_phone_numbers_from_voice_connector_group)
         """
 
     def generate_presigned_url(
         self,
@@ -542,259 +540,250 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#generate_presigned_url)
         """
 
     def get_global_settings(self) -> GetGlobalSettingsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetGlobalSettings).
+        Retrieves the global settings for the Amazon Chime SDK Voice Connectors in an
+        AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_global_settings)
         """
 
     def get_phone_number(self, *, PhoneNumberId: str) -> GetPhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetPhoneNumber).
+        Retrieves details for the specified phone number ID, such as associations,
+        capabilities, and product type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_phone_number)
         """
 
     def get_phone_number_order(
         self, *, PhoneNumberOrderId: str
     ) -> GetPhoneNumberOrderResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetPhoneNumberOrder).
+        Retrieves details for the specified phone number order, such as the order
+        creation timestamp, phone numbers in E.164 format, product type, and order
+        status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_phone_number_order)
         """
 
     def get_phone_number_settings(self) -> GetPhoneNumberSettingsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetPhoneNumberSettings).
+        Retrieves the phone number settings for the administrator's AWS account, such as
+        the default outbound calling name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_phone_number_settings)
         """
 
     def get_proxy_session(
         self, *, VoiceConnectorId: str, ProxySessionId: str
     ) -> GetProxySessionResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetProxySession).
+        Retrieves the specified proxy session details for the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_proxy_session)
         """
 
     def get_sip_media_application(
         self, *, SipMediaApplicationId: str
     ) -> GetSipMediaApplicationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipMediaApplication).
+        Retrieves the information for a SIP media application, including name, AWS
+        Region, and endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_media_application)
         """
 
     def get_sip_media_application_alexa_skill_configuration(
         self, *, SipMediaApplicationId: str
     ) -> GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipMediaApplicationAlexaSkillConfiguration).
+        Gets the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_media_application_alexa_skill_configuration)
         """
 
     def get_sip_media_application_logging_configuration(
         self, *, SipMediaApplicationId: str
     ) -> GetSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipMediaApplicationLoggingConfiguration).
+        Retrieves the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_media_application_logging_configuration)
         """
 
     def get_sip_rule(self, *, SipRuleId: str) -> GetSipRuleResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipRule).
+        Retrieves the details of a SIP rule, such as the rule ID, name, triggers, and
+        target endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_rule)
         """
 
     def get_speaker_search_task(
         self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
     ) -> GetSpeakerSearchTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSpeakerSearchTask).
+        Retrieves the details of the specified speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_speaker_search_task)
         """
 
     def get_voice_connector(self, *, VoiceConnectorId: str) -> GetVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnector).
+        Retrieves details for the specified Amazon Chime SDK Voice Connector, such as
+        timestamps,name, outbound host, and encryption requirements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector)
         """
 
     def get_voice_connector_emergency_calling_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorEmergencyCallingConfiguration).
+        Retrieves the emergency calling configuration details for the specified Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_emergency_calling_configuration)
         """
 
     def get_voice_connector_group(
         self, *, VoiceConnectorGroupId: str
     ) -> GetVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorGroup).
+        Retrieves details for the specified Amazon Chime SDK Voice Connector group, such
+        as timestamps,name, and associated `VoiceConnectorItems`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_group)
         """
 
     def get_voice_connector_logging_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorLoggingConfiguration).
+        Retrieves the logging configuration settings for the specified Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_logging_configuration)
         """
 
     def get_voice_connector_origination(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorOriginationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorOrigination).
+        Retrieves the origination settings for the specified Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_origination)
         """
 
     def get_voice_connector_proxy(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorProxyResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorProxy).
+        Retrieves the proxy configuration details for the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_proxy)
         """
 
     def get_voice_connector_streaming_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorStreamingConfiguration).
+        Retrieves the streaming configuration details for the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_streaming_configuration)
         """
 
     def get_voice_connector_termination(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorTermination).
+        Retrieves the termination setting details for the specified Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_termination)
         """
 
     def get_voice_connector_termination_health(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationHealthResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorTerminationHealth).
+        Retrieves information about the last time a `SIP OPTIONS` ping was received from
+        your SIP infrastructure for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_termination_health)
         """
 
     def get_voice_profile(self, *, VoiceProfileId: str) -> GetVoiceProfileResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceProfile).
+        Retrieves the details of the specified voice profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile)
         """
 
     def get_voice_profile_domain(
         self, *, VoiceProfileDomainId: str
     ) -> GetVoiceProfileDomainResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceProfileDomain).
+        Retrieves the details of the specified voice profile domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile_domain)
         """
 
     def get_voice_tone_analysis_task(
         self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str, IsCaller: bool
     ) -> GetVoiceToneAnalysisTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceToneAnalysisTask).
+        Retrieves the details of a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_tone_analysis_task)
         """
 
     def list_available_voice_connector_regions(
         self,
     ) -> ListAvailableVoiceConnectorRegionsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListAvailableVoiceConnectorRegions).
+        Lists the available AWS Regions in which you can create an Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_available_voice_connector_regions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_available_voice_connector_regions)
         """
 
     def list_phone_number_orders(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPhoneNumberOrdersResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListPhoneNumberOrders).
+        Lists the phone numbers for an administrator's Amazon Chime SDK account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_phone_number_orders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_phone_number_orders)
         """
 
     def list_phone_numbers(
         self,
@@ -803,193 +792,180 @@
         ProductType: PhoneNumberProductTypeType = ...,
         FilterName: PhoneNumberAssociationNameType = ...,
         FilterValue: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListPhoneNumbersResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListPhoneNumbers).
+        Lists the phone numbers for the specified Amazon Chime SDK account, Amazon Chime
+        SDK user, Amazon Chime SDK Voice Connector, or Amazon Chime SDK Voice Connector
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_phone_numbers)
         """
 
     def list_proxy_sessions(
         self,
         *,
         VoiceConnectorId: str,
         Status: ProxySessionStatusType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListProxySessionsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListProxySessions).
+        Lists the proxy sessions for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_proxy_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_proxy_sessions)
         """
 
     def list_sip_media_applications(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSipMediaApplicationsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListSipMediaApplications).
+        Lists the SIP media applications under the administrator's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_sip_media_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_sip_media_applications)
         """
 
     def list_sip_rules(
         self, *, SipMediaApplicationId: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListSipRulesResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListSipRules).
+        Lists the SIP rules under the administrator's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_sip_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_sip_rules)
         """
 
     def list_supported_phone_number_countries(
         self, *, ProductType: PhoneNumberProductTypeType
     ) -> ListSupportedPhoneNumberCountriesResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListSupportedPhoneNumberCountries).
+        Lists the countries that you can order phone numbers from.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_supported_phone_number_countries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_supported_phone_number_countries)
         """
 
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListTagsForResource).
+        Returns a list of the tags in a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_tags_for_resource)
         """
 
     def list_voice_connector_groups(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceConnectorGroupsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceConnectorGroups).
+        Lists the Amazon Chime SDK Voice Connector groups in the administrator's AWS
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connector_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connector_groups)
         """
 
     def list_voice_connector_termination_credentials(
         self, *, VoiceConnectorId: str
     ) -> ListVoiceConnectorTerminationCredentialsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceConnectorTerminationCredentials).
+        Lists the SIP credentials for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connector_termination_credentials)
         """
 
     def list_voice_connectors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceConnectorsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceConnectors).
+        Lists the Amazon Chime SDK Voice Connectors in the administrators AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connectors)
         """
 
     def list_voice_profile_domains(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceProfileDomainsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceProfileDomains).
+        Lists the specified voice profile domains in the administrator's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profile_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profile_domains)
         """
 
     def list_voice_profiles(
         self, *, VoiceProfileDomainId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceProfilesResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceProfiles).
+        Lists the voice profiles in a voice profile domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
         """
 
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
         SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutSipMediaApplicationAlexaSkillConfiguration).
+        Updates the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_alexa_skill_configuration)
         """
 
     def put_sip_media_application_logging_configuration(
         self,
         *,
         SipMediaApplicationId: str,
         SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...
     ) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutSipMediaApplicationLoggingConfiguration).
+        Updates the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_logging_configuration)
         """
 
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
         EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorEmergencyCallingConfiguration).
+        Updates a Voice Connector's emergency calling configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_emergency_calling_configuration)
         """
 
     def put_voice_connector_logging_configuration(
         self, *, VoiceConnectorId: str, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutVoiceConnectorLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorLoggingConfiguration).
+        Updates a Voice Connector's logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_logging_configuration)
         """
 
     def put_voice_connector_origination(
         self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorOrigination).
+        Updates a Voice Connector's origination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_origination)
         """
 
     def put_voice_connector_proxy(
         self,
@@ -997,58 +973,54 @@
         VoiceConnectorId: str,
         DefaultSessionExpiryMinutes: int,
         PhoneNumberPoolCountries: Sequence[str],
         FallBackPhoneNumber: str = ...,
         Disabled: bool = ...
     ) -> PutVoiceConnectorProxyResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorProxy).
+        Puts the specified proxy configuration to the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_proxy)
         """
 
     def put_voice_connector_streaming_configuration(
         self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorStreamingConfiguration).
+        Updates a Voice Connector's streaming configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_streaming_configuration)
         """
 
     def put_voice_connector_termination(
         self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorTermination).
+        Updates a Voice Connector's termination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination)
         """
 
     def put_voice_connector_termination_credentials(
         self, *, VoiceConnectorId: str, Credentials: Sequence[CredentialTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorTerminationCredentials).
+        Updates a Voice Connector's termination credentials.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination_credentials)
         """
 
     def restore_phone_number(self, *, PhoneNumberId: str) -> RestorePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/RestorePhoneNumber).
+        Restores a deleted phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.restore_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#restore_phone_number)
         """
 
     def search_available_phone_numbers(
         self,
@@ -1059,233 +1031,221 @@
         State: str = ...,
         TollFreePrefix: str = ...,
         PhoneNumberType: PhoneNumberTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/SearchAvailablePhoneNumbers).
+        Searches the provisioned phone numbers in an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#search_available_phone_numbers)
         """
 
     def start_speaker_search_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         VoiceProfileDomainId: str,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        CallLeg: CallLegTypeType = ...
     ) -> StartSpeakerSearchTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StartSpeakerSearchTask).
+        Starts a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_speaker_search_task)
         """
 
     def start_voice_tone_analysis_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         LanguageCode: Literal["en-US"],
         ClientRequestToken: str = ...
     ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StartVoiceToneAnalysisTask).
+        Starts a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_voice_tone_analysis_task)
         """
 
     def stop_speaker_search_task(
         self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StopSpeakerSearchTask).
+        Stops a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_speaker_search_task)
         """
 
     def stop_voice_tone_analysis_task(
         self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StopVoiceToneAnalysisTask).
+        Stops a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_voice_tone_analysis_task)
         """
 
     def tag_resource(
         self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/TagResource).
+        Adds a tag to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#tag_resource)
         """
 
     def untag_resource(
         self, *, ResourceARN: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UntagResource).
+        Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#untag_resource)
         """
 
     def update_global_settings(
         self, *, VoiceConnector: VoiceConnectorSettingsTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateGlobalSettings).
+        Updates global settings for the Amazon Chime SDK Voice Connectors in an AWS
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_global_settings)
         """
 
     def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         ProductType: PhoneNumberProductTypeType = ...,
         CallingName: str = ...
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdatePhoneNumber).
+        Updates phone number details, such as product type or calling name, for the
+        specified phone number ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_phone_number)
         """
 
     def update_phone_number_settings(self, *, CallingName: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdatePhoneNumberSettings).
+        Updates the phone number settings for the administrator's AWS account, such as
+        the default outbound calling name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_phone_number_settings)
         """
 
     def update_proxy_session(
         self,
         *,
         VoiceConnectorId: str,
         ProxySessionId: str,
         Capabilities: Sequence[CapabilityType],
         ExpiryMinutes: int = ...
     ) -> UpdateProxySessionResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateProxySession).
+        Updates the specified proxy session details, such as voice or SMS capabilities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_proxy_session)
         """
 
     def update_sip_media_application(
         self,
         *,
         SipMediaApplicationId: str,
         Name: str = ...,
         Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...
     ) -> UpdateSipMediaApplicationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateSipMediaApplication).
+        Updates the details of the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_media_application)
         """
 
     def update_sip_media_application_call(
         self, *, SipMediaApplicationId: str, TransactionId: str, Arguments: Mapping[str, str]
     ) -> UpdateSipMediaApplicationCallResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateSipMediaApplicationCall).
+        Invokes the AWS Lambda function associated with the SIP media application and
+        transaction ID in an update request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application_call)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_media_application_call)
         """
 
     def update_sip_rule(
         self,
         *,
         SipRuleId: str,
         Name: str,
         Disabled: bool = ...,
         TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
     ) -> UpdateSipRuleResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateSipRule).
+        Updates the details of the specified SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_rule)
         """
 
     def update_voice_connector(
         self, *, VoiceConnectorId: str, Name: str, RequireEncryption: bool
     ) -> UpdateVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceConnector).
+        Updates the details for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector)
         """
 
     def update_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         Name: str,
         VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef]
     ) -> UpdateVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceConnectorGroup).
+        Updates the settings for the specified Amazon Chime SDK Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector_group)
         """
 
     def update_voice_profile(
         self, *, VoiceProfileId: str, SpeakerSearchTaskId: str
     ) -> UpdateVoiceProfileResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceProfile).
+        Updates the specified voice profile’s voice print and refreshes its expiration
+        timestamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile)
         """
 
     def update_voice_profile_domain(
         self, *, VoiceProfileDomainId: str, Name: str = ..., Description: str = ...
     ) -> UpdateVoiceProfileDomainResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceProfileDomain).
+        Updates the settings for the specified voice profile domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile_domain)
         """
 
     def validate_e911_address(
         self,
@@ -1295,16 +1255,16 @@
         StreetInfo: str,
         City: str,
         State: str,
         Country: str,
         PostalCode: str
     ) -> ValidateE911AddressResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ValidateE911Address).
+        Validates an address to be used for 911 calls made with Amazon Chime SDK Voice
+        Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.validate_e911_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#validate_e911_address)
         """
 
     @overload
     def get_paginator(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/client.pyi` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    CallLegTypeType,
     CapabilityType,
     GeoMatchLevelType,
     NumberSelectionBehaviorType,
     PhoneNumberAssociationNameType,
     PhoneNumberProductTypeType,
     PhoneNumberTypeType,
     ProxySessionStatusType,
@@ -167,50 +168,47 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#exceptions)
         """
     def associate_phone_numbers_with_voice_connector(
         self, *, VoiceConnectorId: str, E164PhoneNumbers: Sequence[str], ForceAssociate: bool = ...
     ) -> AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/AssociatePhoneNumbersWithVoiceConnector).
+        Associates phone numbers with the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#associate_phone_numbers_with_voice_connector)
         """
     def associate_phone_numbers_with_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         E164PhoneNumbers: Sequence[str],
         ForceAssociate: bool = ...
     ) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/AssociatePhoneNumbersWithVoiceConnectorGroup).
+        Associates phone numbers with the specified Amazon Chime SDK Voice Connector
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#associate_phone_numbers_with_voice_connector_group)
         """
     def batch_delete_phone_number(
         self, *, PhoneNumberIds: Sequence[str]
     ) -> BatchDeletePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/BatchDeletePhoneNumber).
+        Moves phone numbers into the **Deletion queue**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_delete_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_delete_phone_number)
         """
     def batch_update_phone_number(
         self, *, UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef]
     ) -> BatchUpdatePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/BatchUpdatePhoneNumber).
+        Updates one or more phone numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#batch_update_phone_number)
         """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
@@ -225,16 +223,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#close)
         """
     def create_phone_number_order(
         self, *, ProductType: PhoneNumberProductTypeType, E164PhoneNumbers: Sequence[str]
     ) -> CreatePhoneNumberOrderResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreatePhoneNumberOrder).
+        Creates an order for phone numbers to be provisioned.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_phone_number_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_phone_number_order)
         """
     def create_proxy_session(
         self,
         *,
@@ -244,256 +241,257 @@
         Name: str = ...,
         ExpiryMinutes: int = ...,
         NumberSelectionBehavior: NumberSelectionBehaviorType = ...,
         GeoMatchLevel: GeoMatchLevelType = ...,
         GeoMatchParams: GeoMatchParamsTypeDef = ...
     ) -> CreateProxySessionResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateProxySession).
+        Creates a proxy session for the specified Amazon Chime SDK Voice Connector for
+        the specified participant phone numbers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_proxy_session)
         """
     def create_sip_media_application(
-        self, *, AwsRegion: str, Name: str, Endpoints: Sequence[SipMediaApplicationEndpointTypeDef]
+        self,
+        *,
+        AwsRegion: str,
+        Name: str,
+        Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],
+        Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSipMediaApplicationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateSipMediaApplication).
+        Creates a SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_media_application)
         """
     def create_sip_media_application_call(
         self,
         *,
         FromPhoneNumber: str,
         ToPhoneNumber: str,
         SipMediaApplicationId: str,
         SipHeaders: Mapping[str, str] = ...,
         ArgumentsMap: Mapping[str, str] = ...
     ) -> CreateSipMediaApplicationCallResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateSipMediaApplicationCall).
+        Creates an outbound call to a phone number from the phone number specified in
+        the request, and it invokes the endpoint of the specified
+        `sipMediaApplicationId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application_call)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_media_application_call)
         """
     def create_sip_rule(
         self,
         *,
         Name: str,
         TriggerType: SipRuleTriggerTypeType,
         TriggerValue: str,
         Disabled: bool = ...,
         TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
     ) -> CreateSipRuleResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateSipRule).
+        Creates a SIP rule, which can be used to run a SIP media application as a target
+        for a specific trigger type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_sip_rule)
         """
     def create_voice_connector(
-        self, *, Name: str, RequireEncryption: bool, AwsRegion: VoiceConnectorAwsRegionType = ...
+        self,
+        *,
+        Name: str,
+        RequireEncryption: bool,
+        AwsRegion: VoiceConnectorAwsRegionType = ...,
+        Tags: Sequence[TagTypeDef] = ...
     ) -> CreateVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceConnector).
+        Creates an Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector)
         """
     def create_voice_connector_group(
         self, *, Name: str, VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef] = ...
     ) -> CreateVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceConnectorGroup).
+        Creates an Amazon Chime SDK Voice Connector group under the administrator's AWS
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_connector_group)
         """
     def create_voice_profile(
         self, *, SpeakerSearchTaskId: str
     ) -> CreateVoiceProfileResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceProfile).
+        Creates a voice profile, which consists of an enrolled user and their latest
+        voice print.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile)
         """
     def create_voice_profile_domain(
         self,
         *,
         Name: str,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,
         Description: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateVoiceProfileDomainResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/CreateVoiceProfileDomain).
+        Creates a voice profile domain, a collection of voice profiles, their voice
+        prints, and encrypted enrollment audio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#create_voice_profile_domain)
         """
     def delete_phone_number(self, *, PhoneNumberId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeletePhoneNumber).
+        Moves the specified phone number into the **Deletion queue**.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_phone_number)
         """
     def delete_proxy_session(
         self, *, VoiceConnectorId: str, ProxySessionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteProxySession).
+        Deletes the specified proxy session from the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_proxy_session)
         """
     def delete_sip_media_application(
         self, *, SipMediaApplicationId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteSipMediaApplication).
+        Deletes a SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_sip_media_application)
         """
     def delete_sip_rule(self, *, SipRuleId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteSipRule).
+        Deletes a SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_sip_rule)
         """
     def delete_voice_connector(self, *, VoiceConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnector).
+        Deletes an Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector)
         """
     def delete_voice_connector_emergency_calling_configuration(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorEmergencyCallingConfiguration).
+        Deletes the emergency calling details from the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_emergency_calling_configuration)
         """
     def delete_voice_connector_group(
         self, *, VoiceConnectorGroupId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorGroup).
+        Deletes an Amazon Chime SDK Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_group)
         """
     def delete_voice_connector_origination(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorOrigination).
+        Deletes the origination settings for the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_origination)
         """
     def delete_voice_connector_proxy(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorProxy).
+        Deletes the proxy configuration from the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_proxy)
         """
     def delete_voice_connector_streaming_configuration(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorStreamingConfiguration).
+        Deletes a Voice Connector's streaming configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_streaming_configuration)
         """
     def delete_voice_connector_termination(
         self, *, VoiceConnectorId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorTermination).
+        Deletes the termination settings for the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_termination)
         """
     def delete_voice_connector_termination_credentials(
         self, *, VoiceConnectorId: str, Usernames: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceConnectorTerminationCredentials).
+        Deletes the specified SIP credentials used by your equipment to authenticate
+        during call termination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_connector_termination_credentials)
         """
     def delete_voice_profile(self, *, VoiceProfileId: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceProfile).
+        Deletes a voice profile, including its voice print and enrollment data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile)
         """
     def delete_voice_profile_domain(
         self, *, VoiceProfileDomainId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DeleteVoiceProfileDomain).
+        Deletes all voice profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#delete_voice_profile_domain)
         """
     def disassociate_phone_numbers_from_voice_connector(
         self, *, VoiceConnectorId: str, E164PhoneNumbers: Sequence[str]
     ) -> DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DisassociatePhoneNumbersFromVoiceConnector).
+        Disassociates the specified phone numbers from the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.disassociate_phone_numbers_from_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#disassociate_phone_numbers_from_voice_connector)
         """
     def disassociate_phone_numbers_from_voice_connector_group(
         self, *, VoiceConnectorGroupId: str, E164PhoneNumbers: Sequence[str]
     ) -> DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/DisassociatePhoneNumbersFromVoiceConnectorGroup).
+        Disassociates the specified phone numbers from the specified Amazon Chime SDK
+        Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.disassociate_phone_numbers_from_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#disassociate_phone_numbers_from_voice_connector_group)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -505,236 +503,227 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#generate_presigned_url)
         """
     def get_global_settings(self) -> GetGlobalSettingsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetGlobalSettings).
+        Retrieves the global settings for the Amazon Chime SDK Voice Connectors in an
+        AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_global_settings)
         """
     def get_phone_number(self, *, PhoneNumberId: str) -> GetPhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetPhoneNumber).
+        Retrieves details for the specified phone number ID, such as associations,
+        capabilities, and product type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_phone_number)
         """
     def get_phone_number_order(
         self, *, PhoneNumberOrderId: str
     ) -> GetPhoneNumberOrderResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetPhoneNumberOrder).
+        Retrieves details for the specified phone number order, such as the order
+        creation timestamp, phone numbers in E.164 format, product type, and order
+        status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number_order)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_phone_number_order)
         """
     def get_phone_number_settings(self) -> GetPhoneNumberSettingsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetPhoneNumberSettings).
+        Retrieves the phone number settings for the administrator's AWS account, such as
+        the default outbound calling name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_phone_number_settings)
         """
     def get_proxy_session(
         self, *, VoiceConnectorId: str, ProxySessionId: str
     ) -> GetProxySessionResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetProxySession).
+        Retrieves the specified proxy session details for the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_proxy_session)
         """
     def get_sip_media_application(
         self, *, SipMediaApplicationId: str
     ) -> GetSipMediaApplicationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipMediaApplication).
+        Retrieves the information for a SIP media application, including name, AWS
+        Region, and endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_media_application)
         """
     def get_sip_media_application_alexa_skill_configuration(
         self, *, SipMediaApplicationId: str
     ) -> GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipMediaApplicationAlexaSkillConfiguration).
+        Gets the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_media_application_alexa_skill_configuration)
         """
     def get_sip_media_application_logging_configuration(
         self, *, SipMediaApplicationId: str
     ) -> GetSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipMediaApplicationLoggingConfiguration).
+        Retrieves the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_media_application_logging_configuration)
         """
     def get_sip_rule(self, *, SipRuleId: str) -> GetSipRuleResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSipRule).
+        Retrieves the details of a SIP rule, such as the rule ID, name, triggers, and
+        target endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_sip_rule)
         """
     def get_speaker_search_task(
         self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
     ) -> GetSpeakerSearchTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetSpeakerSearchTask).
+        Retrieves the details of the specified speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_speaker_search_task)
         """
     def get_voice_connector(self, *, VoiceConnectorId: str) -> GetVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnector).
+        Retrieves details for the specified Amazon Chime SDK Voice Connector, such as
+        timestamps,name, outbound host, and encryption requirements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector)
         """
     def get_voice_connector_emergency_calling_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorEmergencyCallingConfiguration).
+        Retrieves the emergency calling configuration details for the specified Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_emergency_calling_configuration)
         """
     def get_voice_connector_group(
         self, *, VoiceConnectorGroupId: str
     ) -> GetVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorGroup).
+        Retrieves details for the specified Amazon Chime SDK Voice Connector group, such
+        as timestamps,name, and associated `VoiceConnectorItems`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_group)
         """
     def get_voice_connector_logging_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorLoggingConfiguration).
+        Retrieves the logging configuration settings for the specified Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_logging_configuration)
         """
     def get_voice_connector_origination(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorOriginationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorOrigination).
+        Retrieves the origination settings for the specified Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_origination)
         """
     def get_voice_connector_proxy(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorProxyResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorProxy).
+        Retrieves the proxy configuration details for the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_proxy)
         """
     def get_voice_connector_streaming_configuration(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorStreamingConfiguration).
+        Retrieves the streaming configuration details for the specified Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_streaming_configuration)
         """
     def get_voice_connector_termination(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorTermination).
+        Retrieves the termination setting details for the specified Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_termination)
         """
     def get_voice_connector_termination_health(
         self, *, VoiceConnectorId: str
     ) -> GetVoiceConnectorTerminationHealthResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceConnectorTerminationHealth).
+        Retrieves information about the last time a `SIP OPTIONS` ping was received from
+        your SIP infrastructure for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination_health)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_connector_termination_health)
         """
     def get_voice_profile(self, *, VoiceProfileId: str) -> GetVoiceProfileResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceProfile).
+        Retrieves the details of the specified voice profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile)
         """
     def get_voice_profile_domain(
         self, *, VoiceProfileDomainId: str
     ) -> GetVoiceProfileDomainResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceProfileDomain).
+        Retrieves the details of the specified voice profile domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_profile_domain)
         """
     def get_voice_tone_analysis_task(
         self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str, IsCaller: bool
     ) -> GetVoiceToneAnalysisTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/GetVoiceToneAnalysisTask).
+        Retrieves the details of a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#get_voice_tone_analysis_task)
         """
     def list_available_voice_connector_regions(
         self,
     ) -> ListAvailableVoiceConnectorRegionsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListAvailableVoiceConnectorRegions).
+        Lists the available AWS Regions in which you can create an Amazon Chime SDK
+        Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_available_voice_connector_regions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_available_voice_connector_regions)
         """
     def list_phone_number_orders(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListPhoneNumberOrdersResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListPhoneNumberOrders).
+        Lists the phone numbers for an administrator's Amazon Chime SDK account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_phone_number_orders)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_phone_number_orders)
         """
     def list_phone_numbers(
         self,
         *,
@@ -742,232 +731,215 @@
         ProductType: PhoneNumberProductTypeType = ...,
         FilterName: PhoneNumberAssociationNameType = ...,
         FilterValue: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListPhoneNumbersResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListPhoneNumbers).
+        Lists the phone numbers for the specified Amazon Chime SDK account, Amazon Chime
+        SDK user, Amazon Chime SDK Voice Connector, or Amazon Chime SDK Voice Connector
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_phone_numbers)
         """
     def list_proxy_sessions(
         self,
         *,
         VoiceConnectorId: str,
         Status: ProxySessionStatusType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListProxySessionsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListProxySessions).
+        Lists the proxy sessions for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_proxy_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_proxy_sessions)
         """
     def list_sip_media_applications(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSipMediaApplicationsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListSipMediaApplications).
+        Lists the SIP media applications under the administrator's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_sip_media_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_sip_media_applications)
         """
     def list_sip_rules(
         self, *, SipMediaApplicationId: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListSipRulesResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListSipRules).
+        Lists the SIP rules under the administrator's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_sip_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_sip_rules)
         """
     def list_supported_phone_number_countries(
         self, *, ProductType: PhoneNumberProductTypeType
     ) -> ListSupportedPhoneNumberCountriesResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListSupportedPhoneNumberCountries).
+        Lists the countries that you can order phone numbers from.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_supported_phone_number_countries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_supported_phone_number_countries)
         """
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListTagsForResource).
+        Returns a list of the tags in a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_tags_for_resource)
         """
     def list_voice_connector_groups(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceConnectorGroupsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceConnectorGroups).
+        Lists the Amazon Chime SDK Voice Connector groups in the administrator's AWS
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connector_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connector_groups)
         """
     def list_voice_connector_termination_credentials(
         self, *, VoiceConnectorId: str
     ) -> ListVoiceConnectorTerminationCredentialsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceConnectorTerminationCredentials).
+        Lists the SIP credentials for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connector_termination_credentials)
         """
     def list_voice_connectors(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceConnectorsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceConnectors).
+        Lists the Amazon Chime SDK Voice Connectors in the administrators AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_connectors)
         """
     def list_voice_profile_domains(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceProfileDomainsResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceProfileDomains).
+        Lists the specified voice profile domains in the administrator's AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profile_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profile_domains)
         """
     def list_voice_profiles(
         self, *, VoiceProfileDomainId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListVoiceProfilesResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ListVoiceProfiles).
+        Lists the voice profiles in a voice profile domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#list_voice_profiles)
         """
     def put_sip_media_application_alexa_skill_configuration(
         self,
         *,
         SipMediaApplicationId: str,
         SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...
     ) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutSipMediaApplicationAlexaSkillConfiguration).
+        Updates the Alexa Skill configuration for the SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_alexa_skill_configuration)
         """
     def put_sip_media_application_logging_configuration(
         self,
         *,
         SipMediaApplicationId: str,
         SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...
     ) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutSipMediaApplicationLoggingConfiguration).
+        Updates the logging configuration for the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_sip_media_application_logging_configuration)
         """
     def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
         EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorEmergencyCallingConfiguration).
+        Updates a Voice Connector's emergency calling configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_emergency_calling_configuration)
         """
     def put_voice_connector_logging_configuration(
         self, *, VoiceConnectorId: str, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutVoiceConnectorLoggingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorLoggingConfiguration).
+        Updates a Voice Connector's logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_logging_configuration)
         """
     def put_voice_connector_origination(
         self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorOrigination).
+        Updates a Voice Connector's origination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_origination)
         """
     def put_voice_connector_proxy(
         self,
         *,
         VoiceConnectorId: str,
         DefaultSessionExpiryMinutes: int,
         PhoneNumberPoolCountries: Sequence[str],
         FallBackPhoneNumber: str = ...,
         Disabled: bool = ...
     ) -> PutVoiceConnectorProxyResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorProxy).
+        Puts the specified proxy configuration to the specified Amazon Chime SDK Voice
+        Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_proxy)
         """
     def put_voice_connector_streaming_configuration(
         self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorStreamingConfiguration).
+        Updates a Voice Connector's streaming configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_streaming_configuration)
         """
     def put_voice_connector_termination(
         self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorTermination).
+        Updates a Voice Connector's termination settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination)
         """
     def put_voice_connector_termination_credentials(
         self, *, VoiceConnectorId: str, Credentials: Sequence[CredentialTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/PutVoiceConnectorTerminationCredentials).
+        Updates a Voice Connector's termination credentials.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#put_voice_connector_termination_credentials)
         """
     def restore_phone_number(self, *, PhoneNumberId: str) -> RestorePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/RestorePhoneNumber).
+        Restores a deleted phone number.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.restore_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#restore_phone_number)
         """
     def search_available_phone_numbers(
         self,
         *,
@@ -977,216 +949,204 @@
         State: str = ...,
         TollFreePrefix: str = ...,
         PhoneNumberType: PhoneNumberTypeType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SearchAvailablePhoneNumbersResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/SearchAvailablePhoneNumbers).
+        Searches the provisioned phone numbers in an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#search_available_phone_numbers)
         """
     def start_speaker_search_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         VoiceProfileDomainId: str,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
+        CallLeg: CallLegTypeType = ...
     ) -> StartSpeakerSearchTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StartSpeakerSearchTask).
+        Starts a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_speaker_search_task)
         """
     def start_voice_tone_analysis_task(
         self,
         *,
         VoiceConnectorId: str,
         TransactionId: str,
         LanguageCode: Literal["en-US"],
         ClientRequestToken: str = ...
     ) -> StartVoiceToneAnalysisTaskResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StartVoiceToneAnalysisTask).
+        Starts a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#start_voice_tone_analysis_task)
         """
     def stop_speaker_search_task(
         self, *, VoiceConnectorId: str, SpeakerSearchTaskId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StopSpeakerSearchTask).
+        Stops a speaker search task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_speaker_search_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_speaker_search_task)
         """
     def stop_voice_tone_analysis_task(
         self, *, VoiceConnectorId: str, VoiceToneAnalysisTaskId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/StopVoiceToneAnalysisTask).
+        Stops a voice tone analysis task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_voice_tone_analysis_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#stop_voice_tone_analysis_task)
         """
     def tag_resource(
         self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/TagResource).
+        Adds a tag to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#tag_resource)
         """
     def untag_resource(
         self, *, ResourceARN: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UntagResource).
+        Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#untag_resource)
         """
     def update_global_settings(
         self, *, VoiceConnector: VoiceConnectorSettingsTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateGlobalSettings).
+        Updates global settings for the Amazon Chime SDK Voice Connectors in an AWS
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_global_settings)
         """
     def update_phone_number(
         self,
         *,
         PhoneNumberId: str,
         ProductType: PhoneNumberProductTypeType = ...,
         CallingName: str = ...
     ) -> UpdatePhoneNumberResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdatePhoneNumber).
+        Updates phone number details, such as product type or calling name, for the
+        specified phone number ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_phone_number)
         """
     def update_phone_number_settings(self, *, CallingName: str) -> EmptyResponseMetadataTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdatePhoneNumberSettings).
+        Updates the phone number settings for the administrator's AWS account, such as
+        the default outbound calling name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_phone_number_settings)
         """
     def update_proxy_session(
         self,
         *,
         VoiceConnectorId: str,
         ProxySessionId: str,
         Capabilities: Sequence[CapabilityType],
         ExpiryMinutes: int = ...
     ) -> UpdateProxySessionResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateProxySession).
+        Updates the specified proxy session details, such as voice or SMS capabilities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_proxy_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_proxy_session)
         """
     def update_sip_media_application(
         self,
         *,
         SipMediaApplicationId: str,
         Name: str = ...,
         Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...
     ) -> UpdateSipMediaApplicationResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateSipMediaApplication).
+        Updates the details of the specified SIP media application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_media_application)
         """
     def update_sip_media_application_call(
         self, *, SipMediaApplicationId: str, TransactionId: str, Arguments: Mapping[str, str]
     ) -> UpdateSipMediaApplicationCallResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateSipMediaApplicationCall).
+        Invokes the AWS Lambda function associated with the SIP media application and
+        transaction ID in an update request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application_call)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_media_application_call)
         """
     def update_sip_rule(
         self,
         *,
         SipRuleId: str,
         Name: str,
         Disabled: bool = ...,
         TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...
     ) -> UpdateSipRuleResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateSipRule).
+        Updates the details of the specified SIP rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_sip_rule)
         """
     def update_voice_connector(
         self, *, VoiceConnectorId: str, Name: str, RequireEncryption: bool
     ) -> UpdateVoiceConnectorResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceConnector).
+        Updates the details for the specified Amazon Chime SDK Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector)
         """
     def update_voice_connector_group(
         self,
         *,
         VoiceConnectorGroupId: str,
         Name: str,
         VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef]
     ) -> UpdateVoiceConnectorGroupResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceConnectorGroup).
+        Updates the settings for the specified Amazon Chime SDK Voice Connector group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_connector_group)
         """
     def update_voice_profile(
         self, *, VoiceProfileId: str, SpeakerSearchTaskId: str
     ) -> UpdateVoiceProfileResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceProfile).
+        Updates the specified voice profile’s voice print and refreshes its expiration
+        timestamp.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile)
         """
     def update_voice_profile_domain(
         self, *, VoiceProfileDomainId: str, Name: str = ..., Description: str = ...
     ) -> UpdateVoiceProfileDomainResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/UpdateVoiceProfileDomain).
+        Updates the settings for the specified voice profile domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#update_voice_profile_domain)
         """
     def validate_e911_address(
         self,
         *,
@@ -1195,16 +1155,16 @@
         StreetInfo: str,
         City: str,
         State: str,
         Country: str,
         PostalCode: str
     ) -> ValidateE911AddressResponseTypeDef:
         """
-        See also: [AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/chime-
-        sdk-voice-2022-08-03/ValidateE911Address).
+        Validates an address to be used for 911 calls made with Amazon Chime SDK Voice
+        Connectors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.validate_e911_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/client/#validate_e911_address)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_sip_media_applications"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.py` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AlexaSkillStatusType",
+    "CallLegTypeType",
     "CallingNameStatusType",
     "CapabilityType",
     "ErrorCodeType",
     "GeoMatchLevelType",
     "LanguageCodeType",
     "ListSipMediaApplicationsPaginatorName",
     "ListSipRulesPaginatorName",
@@ -46,14 +47,15 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AlexaSkillStatusType = Literal["ACTIVE", "INACTIVE"]
+CallLegTypeType = Literal["Callee", "Caller"]
 CallingNameStatusType = Literal["Unassigned", "UpdateFailed", "UpdateInProgress", "UpdateSucceeded"]
 CapabilityType = Literal["SMS", "Voice"]
 ErrorCodeType = Literal[
     "AccessDenied",
     "BadRequest",
     "Conflict",
     "Forbidden",
@@ -134,14 +136,15 @@
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
@@ -181,14 +184,15 @@
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
@@ -330,14 +334,15 @@
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
@@ -356,16 +361,19 @@
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
@@ -449,15 +457,17 @@
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

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/literals.pyi` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AlexaSkillStatusType",
+    "CallLegTypeType",
     "CallingNameStatusType",
     "CapabilityType",
     "ErrorCodeType",
     "GeoMatchLevelType",
     "LanguageCodeType",
     "ListSipMediaApplicationsPaginatorName",
     "ListSipRulesPaginatorName",
@@ -44,14 +45,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AlexaSkillStatusType = Literal["ACTIVE", "INACTIVE"]
+CallLegTypeType = Literal["Callee", "Caller"]
 CallingNameStatusType = Literal["Unassigned", "UpdateFailed", "UpdateInProgress", "UpdateSucceeded"]
 CapabilityType = Literal["SMS", "Voice"]
 ErrorCodeType = Literal[
     "AccessDenied",
     "BadRequest",
     "Conflict",
     "Forbidden",
@@ -132,14 +134,15 @@
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
@@ -179,14 +182,15 @@
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
@@ -328,14 +332,15 @@
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
@@ -354,16 +359,19 @@
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
@@ -447,15 +455,17 @@
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

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.py` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListSipMediaApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSipMediaApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
         """
 
 
 class ListSipRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
     """
 
     def paginate(
-        self, *, SipMediaApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SipMediaApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSipRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
         """
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/paginator.pyi` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListSipMediaApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSipMediaApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipMediaApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsipmediaapplicationspaginator)
         """
 
 class ListSipRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
     """
 
     def paginate(
-        self, *, SipMediaApplicationId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SipMediaApplicationId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSipRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Paginator.ListSipRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/paginators/#listsiprulespaginator)
         """
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.py` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
+    CallLegTypeType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
     NotificationTargetType,
     NumberSelectionBehaviorType,
     OrderedPhoneNumberStatusType,
     OriginationRouteProtocolType,
@@ -41,36 +42,33 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "CallDetailsTypeDef",
     "CandidateAddressTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
     "SipMediaApplicationCallTypeDef",
     "SipMediaApplicationEndpointTypeDef",
+    "TagTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
-    "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
-    "TagTypeDef",
     "CreateVoiceProfileRequestRequestTypeDef",
     "VoiceProfileTypeDef",
     "CredentialTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
@@ -83,17 +81,19 @@
     "DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     "DeleteVoiceProfileDomainRequestRequestTypeDef",
     "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
@@ -110,39 +110,45 @@
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "ListVoiceProfileDomainsRequestRequestTypeDef",
     "VoiceProfileDomainSummaryTypeDef",
     "ListVoiceProfilesRequestRequestTypeDef",
     "VoiceProfileSummaryTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
+    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -156,42 +162,38 @@
     "ValidateE911AddressRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
-    "CreateSipMediaApplicationRequestRequestTypeDef",
     "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
+    "CreateSipMediaApplicationRequestRequestTypeDef",
+    "CreateVoiceConnectorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateSipRuleRequestRequestTypeDef",
     "SipRuleTypeDef",
     "UpdateSipRuleRequestRequestTypeDef",
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
-    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
@@ -206,16 +208,14 @@
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
@@ -291,43 +291,30 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
-
 class AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
-
 PhoneNumberErrorTypeDef = TypedDict(
     "PhoneNumberErrorTypeDef",
     {
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
@@ -335,22 +322,20 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
-
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
     },
 )
 
@@ -365,21 +350,19 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
-
 class UpdatePhoneNumberRequestItemTypeDef(
     _RequiredUpdatePhoneNumberRequestItemTypeDef, _OptionalUpdatePhoneNumberRequestItemTypeDef
 ):
     pass
 
-
 CallDetailsTypeDef = TypedDict(
     "CallDetailsTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "IsCaller": bool,
     },
@@ -429,22 +412,20 @@
     {
         "SipHeaders": Mapping[str, str],
         "ArgumentsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSipMediaApplicationCallRequestRequestTypeDef(
     _RequiredCreateSipMediaApplicationCallRequestRequestTypeDef,
     _OptionalCreateSipMediaApplicationCallRequestRequestTypeDef,
 ):
     pass
 
-
 SipMediaApplicationCallTypeDef = TypedDict(
     "SipMediaApplicationCallTypeDef",
     {
         "TransactionId": str,
     },
     total=False,
 )
@@ -453,14 +434,22 @@
     "SipMediaApplicationEndpointTypeDef",
     {
         "LambdaArn": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 SipRuleTargetApplicationTypeDef = TypedDict(
     "SipRuleTargetApplicationTypeDef",
     {
         "SipMediaApplicationId": str,
         "Priority": int,
         "AwsRegion": str,
     },
@@ -471,37 +460,14 @@
     "VoiceConnectorItemTypeDef",
     {
         "VoiceConnectorId": str,
         "Priority": int,
     },
 )
 
-_RequiredCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVoiceConnectorRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RequireEncryption": bool,
-    },
-)
-_OptionalCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVoiceConnectorRequestRequestTypeDef",
-    {
-        "AwsRegion": VoiceConnectorAwsRegionType,
-    },
-    total=False,
-)
-
-
-class CreateVoiceConnectorRequestRequestTypeDef(
-    _RequiredCreateVoiceConnectorRequestRequestTypeDef,
-    _OptionalCreateVoiceConnectorRequestRequestTypeDef,
-):
-    pass
-
-
 VoiceConnectorTypeDef = TypedDict(
     "VoiceConnectorTypeDef",
     {
         "VoiceConnectorId": str,
         "AwsRegion": VoiceConnectorAwsRegionType,
         "Name": str,
         "OutboundHostName": str,
@@ -516,22 +482,14 @@
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 CreateVoiceProfileRequestRequestTypeDef = TypedDict(
     "CreateVoiceProfileRequestRequestTypeDef",
     {
         "SpeakerSearchTaskId": str,
     },
 )
 
@@ -568,22 +526,20 @@
     "_OptionalDNISEmergencyCallingConfigurationTypeDef",
     {
         "TestPhoneNumber": str,
     },
     total=False,
 )
 
-
 class DNISEmergencyCallingConfigurationTypeDef(
     _RequiredDNISEmergencyCallingConfigurationTypeDef,
     _OptionalDNISEmergencyCallingConfigurationTypeDef,
 ):
     pass
 
-
 DeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "DeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -692,14 +648,21 @@
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VoiceConnectorSettingsTypeDef = TypedDict(
     "VoiceConnectorSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
@@ -714,14 +677,23 @@
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
@@ -901,14 +873,22 @@
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
         "IsCaller": bool,
     },
 )
 
+ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
+    {
+        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPhoneNumberOrdersRequestRequestTypeDef = TypedDict(
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -939,40 +919,45 @@
         "Status": ProxySessionStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListProxySessionsRequestRequestTypeDef(
     _RequiredListProxySessionsRequestRequestTypeDef, _OptionalListProxySessionsRequestRequestTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSipMediaApplicationsRequestRequestTypeDef = TypedDict(
     "ListSipMediaApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSipRulesRequestRequestTypeDef = TypedDict(
     "ListSipRulesRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1014,14 +999,22 @@
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
@@ -1060,21 +1053,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListVoiceProfilesRequestRequestTypeDef(
     _RequiredListVoiceProfilesRequestRequestTypeDef, _OptionalListVoiceProfilesRequestRequestTypeDef
 ):
     pass
 
-
 VoiceProfileSummaryTypeDef = TypedDict(
     "VoiceProfileSummaryTypeDef",
     {
         "VoiceProfileId": str,
         "VoiceProfileArn": str,
         "VoiceProfileDomainId": str,
         "CreatedTimestamp": datetime,
@@ -1110,14 +1101,24 @@
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
@@ -1159,21 +1160,30 @@
     {
         "FallBackPhoneNumber": str,
         "Disabled": bool,
     },
     total=False,
 )
 
-
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
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
 
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
@@ -1189,14 +1199,23 @@
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
 SpeakerSearchResultTypeDef = TypedDict(
     "SpeakerSearchResultTypeDef",
     {
         "ConfidenceScore": float,
         "VoiceProfileId": str,
     },
     total=False,
@@ -1210,26 +1229,25 @@
         "VoiceProfileDomainId": str,
     },
 )
 _OptionalStartSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
     "_OptionalStartSpeakerSearchTaskRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
+        "CallLeg": CallLegTypeType,
     },
     total=False,
 )
 
-
 class StartSpeakerSearchTaskRequestRequestTypeDef(
     _RequiredStartSpeakerSearchTaskRequestRequestTypeDef,
     _OptionalStartSpeakerSearchTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "LanguageCode": Literal["en-US"],
     },
@@ -1238,22 +1256,20 @@
     "_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartVoiceToneAnalysisTaskRequestRequestTypeDef(
     _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef,
     _OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef,
 ):
     pass
 
-
 StopSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1293,21 +1309,19 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
-
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
-
 UpdatePhoneNumberSettingsRequestRequestTypeDef = TypedDict(
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     {
         "CallingName": str,
     },
 )
 
@@ -1323,22 +1337,20 @@
     "_OptionalUpdateProxySessionRequestRequestTypeDef",
     {
         "ExpiryMinutes": int,
     },
     total=False,
 )
 
-
 class UpdateProxySessionRequestRequestTypeDef(
     _RequiredUpdateProxySessionRequestRequestTypeDef,
     _OptionalUpdateProxySessionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateSipMediaApplicationCallRequestRequestTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "TransactionId": str,
         "Arguments": Mapping[str, str],
     },
@@ -1364,22 +1376,20 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredUpdateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalUpdateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateVoiceProfileRequestRequestTypeDef = TypedDict(
     "UpdateVoiceProfileRequestRequestTypeDef",
     {
         "VoiceProfileId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1397,96 +1407,55 @@
     },
 )
 
 AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeletePhoneNumberResponseTypeDef = TypedDict(
     "BatchDeletePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
     "BatchUpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
-    {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
-    {
-        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    {
-        "Usernames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
@@ -1510,15 +1479,15 @@
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
 
 _RequiredCreateProxySessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1534,56 +1503,46 @@
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
         "GeoMatchParams": GeoMatchParamsTypeDef,
     },
     total=False,
 )
 
-
 class CreateProxySessionRequestRequestTypeDef(
     _RequiredCreateProxySessionRequestRequestTypeDef,
     _OptionalCreateProxySessionRequestRequestTypeDef,
 ):
     pass
 
-
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
-    },
-)
-
-CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
-    "CreateSipMediaApplicationRequestRequestTypeDef",
-    {
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SipMediaApplicationTypeDef = TypedDict(
     "SipMediaApplicationTypeDef",
     {
         "SipMediaApplicationId": str,
         "AwsRegion": str,
         "Name": str,
         "Endpoints": List[SipMediaApplicationEndpointTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
+        "SipMediaApplicationArn": str,
     },
     total=False,
 )
 
 _RequiredUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipMediaApplicationRequestRequestTypeDef",
     {
@@ -1595,21 +1554,79 @@
     {
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
     },
     total=False,
 )
 
-
 class UpdateSipMediaApplicationRequestRequestTypeDef(
     _RequiredUpdateSipMediaApplicationRequestRequestTypeDef,
     _OptionalUpdateSipMediaApplicationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSipMediaApplicationRequestRequestTypeDef",
+    {
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
+    },
+)
+_OptionalCreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSipMediaApplicationRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSipMediaApplicationRequestRequestTypeDef(
+    _RequiredCreateSipMediaApplicationRequestRequestTypeDef,
+    _OptionalCreateSipMediaApplicationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVoiceConnectorRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RequireEncryption": bool,
+    },
+)
+_OptionalCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVoiceConnectorRequestRequestTypeDef",
+    {
+        "AwsRegion": VoiceConnectorAwsRegionType,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateVoiceConnectorRequestRequestTypeDef(
+    _RequiredCreateVoiceConnectorRequestRequestTypeDef,
+    _OptionalCreateVoiceConnectorRequestRequestTypeDef,
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
 
 _RequiredCreateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSipRuleRequestRequestTypeDef",
     {
         "Name": str,
         "TriggerType": SipRuleTriggerTypeType,
         "TriggerValue": str,
@@ -1620,21 +1637,19 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
-
 class CreateSipRuleRequestRequestTypeDef(
     _RequiredCreateSipRuleRequestRequestTypeDef, _OptionalCreateSipRuleRequestRequestTypeDef
 ):
     pass
 
-
 SipRuleTypeDef = TypedDict(
     "SipRuleTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
         "Disabled": bool,
         "TriggerType": SipRuleTriggerTypeType,
@@ -1658,43 +1673,39 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateSipRuleRequestRequestTypeDef(
     _RequiredUpdateSipRuleRequestRequestTypeDef, _OptionalUpdateSipRuleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
     total=False,
 )
 
-
 class CreateVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorGroupId": str,
         "Name": str,
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
@@ -1713,57 +1724,43 @@
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
 
-VoiceProfileDomainTypeDef = TypedDict(
-    "VoiceProfileDomainTypeDef",
-    {
-        "VoiceProfileDomainId": str,
-        "VoiceProfileDomainArn": str,
-        "Name": str,
-        "Description": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceProfileDomainRequestRequestTypeDef",
     {
         "Name": str,
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
     },
 )
@@ -1773,59 +1770,55 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 CreateVoiceProfileResponseTypeDef = TypedDict(
     "CreateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceProfileResponseTypeDef = TypedDict(
     "GetVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceProfileResponseTypeDef = TypedDict(
     "UpdateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1835,35 +1828,33 @@
     "_OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "Credentials": Sequence[CredentialTypeDef],
     },
     total=False,
 )
 
-
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
-
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
         "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsRequestRequestTypeDef",
     {
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
@@ -1873,15 +1864,15 @@
 
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
@@ -1893,37 +1884,35 @@
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
     },
     total=False,
 )
 
-
 class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
     _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
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
@@ -1933,35 +1922,33 @@
     "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
     _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
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
@@ -1969,47 +1956,47 @@
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
@@ -2017,58 +2004,41 @@
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
 
-ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceProfilesResponseTypeDef = TypedDict(
     "ListVoiceProfilesResponseTypeDef",
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
@@ -2153,165 +2123,163 @@
     {
         "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
         "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
-
 GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
         "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
     "StartVoiceToneAnalysisTaskResponseTypeDef",
     {
         "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
 
 CreateVoiceProfileDomainResponseTypeDef = TypedDict(
     "CreateVoiceProfileDomainResponseTypeDef",
     {
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceProfileDomainResponseTypeDef = TypedDict(
     "GetVoiceProfileDomainResponseTypeDef",
     {
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
     "UpdateVoiceProfileDomainResponseTypeDef",
     {
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
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
@@ -2319,48 +2287,48 @@
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
@@ -2368,81 +2336,81 @@
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
 
 SpeakerSearchTaskTypeDef = TypedDict(
     "SpeakerSearchTaskTypeDef",
     {
         "SpeakerSearchTaskId": str,
@@ -2457,15 +2425,15 @@
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
@@ -2473,26 +2441,26 @@
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
 
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSpeakerSearchTaskResponseTypeDef = TypedDict(
     "StartSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice/type_defs.pyi` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AlexaSkillStatusType,
     CallingNameStatusType,
+    CallLegTypeType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
     NotificationTargetType,
     NumberSelectionBehaviorType,
     OrderedPhoneNumberStatusType,
     OriginationRouteProtocolType,
@@ -41,35 +42,34 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddressTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberRequestItemTypeDef",
     "CallDetailsTypeDef",
     "CandidateAddressTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
     "SipMediaApplicationCallTypeDef",
     "SipMediaApplicationEndpointTypeDef",
+    "TagTypeDef",
     "SipRuleTargetApplicationTypeDef",
     "VoiceConnectorItemTypeDef",
-    "CreateVoiceConnectorRequestRequestTypeDef",
     "VoiceConnectorTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
-    "TagTypeDef",
     "CreateVoiceProfileRequestRequestTypeDef",
     "VoiceProfileTypeDef",
     "CredentialTypeDef",
     "DNISEmergencyCallingConfigurationTypeDef",
     "DeletePhoneNumberRequestRequestTypeDef",
     "DeleteProxySessionRequestRequestTypeDef",
     "DeleteSipMediaApplicationRequestRequestTypeDef",
@@ -82,17 +82,19 @@
     "DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "DeleteVoiceConnectorTerminationRequestRequestTypeDef",
     "DeleteVoiceProfileDomainRequestRequestTypeDef",
     "DeleteVoiceProfileRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     "SipMediaApplicationAlexaSkillConfigurationTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
@@ -109,39 +111,45 @@
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     "TerminationTypeDef",
     "GetVoiceProfileDomainRequestRequestTypeDef",
     "GetVoiceProfileRequestRequestTypeDef",
     "GetVoiceToneAnalysisTaskRequestRequestTypeDef",
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     "ListPhoneNumbersRequestRequestTypeDef",
     "ListProxySessionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "ListVoiceProfileDomainsRequestRequestTypeDef",
     "VoiceProfileDomainSummaryTypeDef",
     "ListVoiceProfilesRequestRequestTypeDef",
     "VoiceProfileSummaryTypeDef",
     "MediaInsightsConfigurationTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
+    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     "SpeakerSearchResultTypeDef",
     "StartSpeakerSearchTaskRequestRequestTypeDef",
     "StartVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     "StopVoiceToneAnalysisTaskRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -155,42 +163,38 @@
     "ValidateE911AddressRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     "VoiceToneAnalysisTaskTypeDef",
     "ValidateE911AddressResponseTypeDef",
     "CreateProxySessionRequestRequestTypeDef",
     "CreateSipMediaApplicationCallResponseTypeDef",
     "UpdateSipMediaApplicationCallResponseTypeDef",
-    "CreateSipMediaApplicationRequestRequestTypeDef",
     "SipMediaApplicationTypeDef",
     "UpdateSipMediaApplicationRequestRequestTypeDef",
+    "CreateSipMediaApplicationRequestRequestTypeDef",
+    "CreateVoiceConnectorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateSipRuleRequestRequestTypeDef",
     "SipRuleTypeDef",
     "UpdateSipRuleRequestRequestTypeDef",
     "CreateVoiceConnectorGroupRequestRequestTypeDef",
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
-    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileDomainRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "VoiceProfileDomainTypeDef",
     "CreateVoiceProfileResponseTypeDef",
     "GetVoiceProfileResponseTypeDef",
     "UpdateVoiceProfileResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
@@ -205,16 +209,14 @@
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
     "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "ListVoiceProfileDomainsResponseTypeDef",
     "ListVoiceProfilesResponseTypeDef",
     "PhoneNumberOrderTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
@@ -290,41 +292,32 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
+
 class AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
+
 PhoneNumberErrorTypeDef = TypedDict(
     "PhoneNumberErrorTypeDef",
     {
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
@@ -332,20 +325,22 @@
     "_OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "ForceAssociate": bool,
     },
     total=False,
 )
 
+
 class AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef(
     _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     _OptionalAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
 ):
     pass
 
+
 BatchDeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchDeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
     },
 )
 
@@ -360,19 +355,21 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
+
 class UpdatePhoneNumberRequestItemTypeDef(
     _RequiredUpdatePhoneNumberRequestItemTypeDef, _OptionalUpdatePhoneNumberRequestItemTypeDef
 ):
     pass
 
+
 CallDetailsTypeDef = TypedDict(
     "CallDetailsTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "IsCaller": bool,
     },
@@ -422,20 +419,22 @@
     {
         "SipHeaders": Mapping[str, str],
         "ArgumentsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSipMediaApplicationCallRequestRequestTypeDef(
     _RequiredCreateSipMediaApplicationCallRequestRequestTypeDef,
     _OptionalCreateSipMediaApplicationCallRequestRequestTypeDef,
 ):
     pass
 
+
 SipMediaApplicationCallTypeDef = TypedDict(
     "SipMediaApplicationCallTypeDef",
     {
         "TransactionId": str,
     },
     total=False,
 )
@@ -444,14 +443,22 @@
     "SipMediaApplicationEndpointTypeDef",
     {
         "LambdaArn": str,
     },
     total=False,
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 SipRuleTargetApplicationTypeDef = TypedDict(
     "SipRuleTargetApplicationTypeDef",
     {
         "SipMediaApplicationId": str,
         "Priority": int,
         "AwsRegion": str,
     },
@@ -462,35 +469,14 @@
     "VoiceConnectorItemTypeDef",
     {
         "VoiceConnectorId": str,
         "Priority": int,
     },
 )
 
-_RequiredCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVoiceConnectorRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RequireEncryption": bool,
-    },
-)
-_OptionalCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVoiceConnectorRequestRequestTypeDef",
-    {
-        "AwsRegion": VoiceConnectorAwsRegionType,
-    },
-    total=False,
-)
-
-class CreateVoiceConnectorRequestRequestTypeDef(
-    _RequiredCreateVoiceConnectorRequestRequestTypeDef,
-    _OptionalCreateVoiceConnectorRequestRequestTypeDef,
-):
-    pass
-
 VoiceConnectorTypeDef = TypedDict(
     "VoiceConnectorTypeDef",
     {
         "VoiceConnectorId": str,
         "AwsRegion": VoiceConnectorAwsRegionType,
         "Name": str,
         "OutboundHostName": str,
@@ -505,22 +491,14 @@
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 CreateVoiceProfileRequestRequestTypeDef = TypedDict(
     "CreateVoiceProfileRequestRequestTypeDef",
     {
         "SpeakerSearchTaskId": str,
     },
 )
 
@@ -557,20 +535,22 @@
     "_OptionalDNISEmergencyCallingConfigurationTypeDef",
     {
         "TestPhoneNumber": str,
     },
     total=False,
 )
 
+
 class DNISEmergencyCallingConfigurationTypeDef(
     _RequiredDNISEmergencyCallingConfigurationTypeDef,
     _OptionalDNISEmergencyCallingConfigurationTypeDef,
 ):
     pass
 
+
 DeletePhoneNumberRequestRequestTypeDef = TypedDict(
     "DeletePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -679,14 +659,21 @@
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VoiceConnectorSettingsTypeDef = TypedDict(
     "VoiceConnectorSettingsTypeDef",
     {
         "CdrBucket": str,
     },
     total=False,
 )
@@ -701,14 +688,23 @@
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
@@ -888,14 +884,22 @@
     {
         "VoiceConnectorId": str,
         "VoiceToneAnalysisTaskId": str,
         "IsCaller": bool,
     },
 )
 
+ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
+    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
+    {
+        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPhoneNumberOrdersRequestRequestTypeDef = TypedDict(
     "ListPhoneNumberOrdersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -926,38 +930,47 @@
         "Status": ProxySessionStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListProxySessionsRequestRequestTypeDef(
     _RequiredListProxySessionsRequestRequestTypeDef, _OptionalListProxySessionsRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
+    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSipMediaApplicationsRequestRequestTypeDef = TypedDict(
     "ListSipMediaApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
+    "ListSipRulesRequestListSipRulesPaginateTypeDef",
+    {
+        "SipMediaApplicationId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSipRulesRequestRequestTypeDef = TypedDict(
     "ListSipRulesRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -999,14 +1012,22 @@
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
@@ -1045,19 +1066,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListVoiceProfilesRequestRequestTypeDef(
     _RequiredListVoiceProfilesRequestRequestTypeDef, _OptionalListVoiceProfilesRequestRequestTypeDef
 ):
     pass
 
+
 VoiceProfileSummaryTypeDef = TypedDict(
     "VoiceProfileSummaryTypeDef",
     {
         "VoiceProfileId": str,
         "VoiceProfileArn": str,
         "VoiceProfileDomainId": str,
         "CreatedTimestamp": datetime,
@@ -1093,14 +1116,24 @@
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
@@ -1142,20 +1175,33 @@
     {
         "FallBackPhoneNumber": str,
         "Disabled": bool,
     },
     total=False,
 )
 
+
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -1170,14 +1216,23 @@
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
 SpeakerSearchResultTypeDef = TypedDict(
     "SpeakerSearchResultTypeDef",
     {
         "ConfidenceScore": float,
         "VoiceProfileId": str,
     },
     total=False,
@@ -1191,24 +1246,27 @@
         "VoiceProfileDomainId": str,
     },
 )
 _OptionalStartSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
     "_OptionalStartSpeakerSearchTaskRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
+        "CallLeg": CallLegTypeType,
     },
     total=False,
 )
 
+
 class StartSpeakerSearchTaskRequestRequestTypeDef(
     _RequiredStartSpeakerSearchTaskRequestRequestTypeDef,
     _OptionalStartSpeakerSearchTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "TransactionId": str,
         "LanguageCode": Literal["en-US"],
     },
@@ -1217,20 +1275,22 @@
     "_OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartVoiceToneAnalysisTaskRequestRequestTypeDef(
     _RequiredStartVoiceToneAnalysisTaskRequestRequestTypeDef,
     _OptionalStartVoiceToneAnalysisTaskRequestRequestTypeDef,
 ):
     pass
 
+
 StopSpeakerSearchTaskRequestRequestTypeDef = TypedDict(
     "StopSpeakerSearchTaskRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1270,19 +1330,21 @@
     {
         "ProductType": PhoneNumberProductTypeType,
         "CallingName": str,
     },
     total=False,
 )
 
+
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
+
 UpdatePhoneNumberSettingsRequestRequestTypeDef = TypedDict(
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     {
         "CallingName": str,
     },
 )
 
@@ -1298,20 +1360,22 @@
     "_OptionalUpdateProxySessionRequestRequestTypeDef",
     {
         "ExpiryMinutes": int,
     },
     total=False,
 )
 
+
 class UpdateProxySessionRequestRequestTypeDef(
     _RequiredUpdateProxySessionRequestRequestTypeDef,
     _OptionalUpdateProxySessionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateSipMediaApplicationCallRequestRequestTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
         "TransactionId": str,
         "Arguments": Mapping[str, str],
     },
@@ -1337,20 +1401,22 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredUpdateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalUpdateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateVoiceProfileRequestRequestTypeDef = TypedDict(
     "UpdateVoiceProfileRequestRequestTypeDef",
     {
         "VoiceProfileId": str,
         "SpeakerSearchTaskId": str,
     },
 )
@@ -1368,96 +1434,55 @@
     },
 )
 
 AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeletePhoneNumberResponseTypeDef = TypedDict(
     "BatchDeletePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
     "BatchUpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
     {
         "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
-    {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAvailableVoiceConnectorRegionsResponseTypeDef = TypedDict(
-    "ListAvailableVoiceConnectorRegionsResponseTypeDef",
-    {
-        "VoiceConnectorRegions": List[VoiceConnectorAwsRegionType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    {
-        "Usernames": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
-    {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
@@ -1481,15 +1506,15 @@
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
 
 _RequiredCreateProxySessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1505,54 +1530,48 @@
         "NumberSelectionBehavior": NumberSelectionBehaviorType,
         "GeoMatchLevel": GeoMatchLevelType,
         "GeoMatchParams": GeoMatchParamsTypeDef,
     },
     total=False,
 )
 
+
 class CreateProxySessionRequestRequestTypeDef(
     _RequiredCreateProxySessionRequestRequestTypeDef,
     _OptionalCreateProxySessionRequestRequestTypeDef,
 ):
     pass
 
+
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
-    },
-)
-
-CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
-    "CreateSipMediaApplicationRequestRequestTypeDef",
-    {
-        "AwsRegion": str,
-        "Name": str,
-        "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SipMediaApplicationTypeDef = TypedDict(
     "SipMediaApplicationTypeDef",
     {
         "SipMediaApplicationId": str,
         "AwsRegion": str,
         "Name": str,
         "Endpoints": List[SipMediaApplicationEndpointTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
+        "SipMediaApplicationArn": str,
     },
     total=False,
 )
 
 _RequiredUpdateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSipMediaApplicationRequestRequestTypeDef",
     {
@@ -1564,20 +1583,86 @@
     {
         "Name": str,
         "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
     },
     total=False,
 )
 
+
 class UpdateSipMediaApplicationRequestRequestTypeDef(
     _RequiredUpdateSipMediaApplicationRequestRequestTypeDef,
     _OptionalUpdateSipMediaApplicationRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredCreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSipMediaApplicationRequestRequestTypeDef",
+    {
+        "AwsRegion": str,
+        "Name": str,
+        "Endpoints": Sequence[SipMediaApplicationEndpointTypeDef],
+    },
+)
+_OptionalCreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSipMediaApplicationRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSipMediaApplicationRequestRequestTypeDef(
+    _RequiredCreateSipMediaApplicationRequestRequestTypeDef,
+    _OptionalCreateSipMediaApplicationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVoiceConnectorRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RequireEncryption": bool,
+    },
+)
+_OptionalCreateVoiceConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVoiceConnectorRequestRequestTypeDef",
+    {
+        "AwsRegion": VoiceConnectorAwsRegionType,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVoiceConnectorRequestRequestTypeDef(
+    _RequiredCreateVoiceConnectorRequestRequestTypeDef,
+    _OptionalCreateVoiceConnectorRequestRequestTypeDef,
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 _RequiredCreateSipRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSipRuleRequestRequestTypeDef",
     {
         "Name": str,
         "TriggerType": SipRuleTriggerTypeType,
         "TriggerValue": str,
     },
@@ -1587,19 +1672,21 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
+
 class CreateSipRuleRequestRequestTypeDef(
     _RequiredCreateSipRuleRequestRequestTypeDef, _OptionalCreateSipRuleRequestRequestTypeDef
 ):
     pass
 
+
 SipRuleTypeDef = TypedDict(
     "SipRuleTypeDef",
     {
         "SipRuleId": str,
         "Name": str,
         "Disabled": bool,
         "TriggerType": SipRuleTriggerTypeType,
@@ -1623,39 +1710,43 @@
     {
         "Disabled": bool,
         "TargetApplications": Sequence[SipRuleTargetApplicationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateSipRuleRequestRequestTypeDef(
     _RequiredUpdateSipRuleRequestRequestTypeDef, _OptionalUpdateSipRuleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
     total=False,
 )
 
+
 class CreateVoiceConnectorGroupRequestRequestTypeDef(
     _RequiredCreateVoiceConnectorGroupRequestRequestTypeDef,
     _OptionalCreateVoiceConnectorGroupRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateVoiceConnectorGroupRequestRequestTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     {
         "VoiceConnectorGroupId": str,
         "Name": str,
         "VoiceConnectorItems": Sequence[VoiceConnectorItemTypeDef],
     },
@@ -1674,57 +1765,43 @@
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
 
-VoiceProfileDomainTypeDef = TypedDict(
-    "VoiceProfileDomainTypeDef",
-    {
-        "VoiceProfileDomainId": str,
-        "VoiceProfileDomainArn": str,
-        "Name": str,
-        "Description": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateVoiceProfileDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVoiceProfileDomainRequestRequestTypeDef",
     {
         "Name": str,
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
     },
 )
@@ -1734,57 +1811,57 @@
         "Description": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVoiceProfileDomainRequestRequestTypeDef(
     _RequiredCreateVoiceProfileDomainRequestRequestTypeDef,
     _OptionalCreateVoiceProfileDomainRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+VoiceProfileDomainTypeDef = TypedDict(
+    "VoiceProfileDomainTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "VoiceProfileDomainId": str,
+        "VoiceProfileDomainArn": str,
+        "Name": str,
+        "Description": str,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
     },
+    total=False,
 )
 
 CreateVoiceProfileResponseTypeDef = TypedDict(
     "CreateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceProfileResponseTypeDef = TypedDict(
     "GetVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceProfileResponseTypeDef = TypedDict(
     "UpdateVoiceProfileResponseTypeDef",
     {
         "VoiceProfile": VoiceProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -1794,33 +1871,35 @@
     "_OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "Credentials": Sequence[CredentialTypeDef],
     },
     total=False,
 )
 
+
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
+
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
         "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsRequestRequestTypeDef",
     {
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
@@ -1830,15 +1909,15 @@
 
 GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
@@ -1850,35 +1929,37 @@
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
     },
     total=False,
 )
 
+
 class PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef(
     _RequiredPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     _OptionalPutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef",
     {
         "SipMediaApplicationAlexaSkillConfiguration": (
             SipMediaApplicationAlexaSkillConfigurationTypeDef
         ),
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
@@ -1888,33 +1969,35 @@
     "_OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef(
     _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     _OptionalPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
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
@@ -1922,47 +2005,47 @@
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
@@ -1970,58 +2053,41 @@
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
 
-ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef = TypedDict(
-    "ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSipRulesRequestListSipRulesPaginateTypeDef = TypedDict(
-    "ListSipRulesRequestListSipRulesPaginateTypeDef",
-    {
-        "SipMediaApplicationId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceProfileDomainsResponseTypeDef = TypedDict(
     "ListVoiceProfileDomainsResponseTypeDef",
     {
         "VoiceProfileDomains": List[VoiceProfileDomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVoiceProfilesResponseTypeDef = TypedDict(
     "ListVoiceProfilesResponseTypeDef",
     {
         "VoiceProfiles": List[VoiceProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PhoneNumberOrderTypeDef = TypedDict(
     "PhoneNumberOrderTypeDef",
     {
         "PhoneNumberOrderId": str,
@@ -2106,163 +2172,165 @@
     {
         "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
         "MediaInsightsConfiguration": MediaInsightsConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
     pass
 
+
 GetVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
     "GetVoiceToneAnalysisTaskResponseTypeDef",
     {
         "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartVoiceToneAnalysisTaskResponseTypeDef = TypedDict(
     "StartVoiceToneAnalysisTaskResponseTypeDef",
     {
         "VoiceToneAnalysisTask": VoiceToneAnalysisTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
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
 
 CreateVoiceProfileDomainResponseTypeDef = TypedDict(
     "CreateVoiceProfileDomainResponseTypeDef",
     {
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVoiceProfileDomainResponseTypeDef = TypedDict(
     "GetVoiceProfileDomainResponseTypeDef",
     {
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVoiceProfileDomainResponseTypeDef = TypedDict(
     "UpdateVoiceProfileDomainResponseTypeDef",
     {
         "VoiceProfileDomain": VoiceProfileDomainTypeDef,
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
@@ -2270,48 +2338,48 @@
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
@@ -2319,81 +2387,81 @@
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
 
 SpeakerSearchTaskTypeDef = TypedDict(
     "SpeakerSearchTaskTypeDef",
     {
         "SpeakerSearchTaskId": str,
@@ -2408,15 +2476,15 @@
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
@@ -2424,26 +2492,26 @@
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
 
 GetSpeakerSearchTaskResponseTypeDef = TypedDict(
     "GetSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSpeakerSearchTaskResponseTypeDef = TypedDict(
     "StartSpeakerSearchTaskResponseTypeDef",
     {
         "SpeakerSearchTask": SpeakerSearchTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-voice
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKVoice 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKVoice 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-voice"></a>
 
 # mypy-boto3-chime-sdk-voice
 
 [![PyPI - mypy-boto3-chime-sdk-voice](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-voice.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-voice)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-voice?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKVoice 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
+[boto3.ChimeSDKVoice 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
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
 [mypy-boto3-chime-sdk-voice docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,14 +305,15 @@
 
 `mypy_boto3_chime_sdk_voice.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.literals import (
     AlexaSkillStatusType,
+    CallLegTypeType,
     CallingNameStatusType,
     CapabilityType,
     ErrorCodeType,
     GeoMatchLevelType,
     LanguageCodeType,
     ListSipMediaApplicationsPaginatorName,
     ListSipRulesPaginatorName,
@@ -349,31 +350,29 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_voice.type_defs import (
     AddressTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
-    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     BatchDeletePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberRequestItemTypeDef,
     CallDetailsTypeDef,
     CandidateAddressTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
     SipMediaApplicationCallTypeDef,
     SipMediaApplicationEndpointTypeDef,
+    TagTypeDef,
     SipRuleTargetApplicationTypeDef,
     VoiceConnectorItemTypeDef,
-    CreateVoiceConnectorRequestRequestTypeDef,
     VoiceConnectorTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    TagTypeDef,
     CreateVoiceProfileRequestRequestTypeDef,
     VoiceProfileTypeDef,
     CredentialTypeDef,
     DNISEmergencyCallingConfigurationTypeDef,
     DeletePhoneNumberRequestRequestTypeDef,
     DeleteProxySessionRequestRequestTypeDef,
     DeleteSipMediaApplicationRequestRequestTypeDef,
@@ -386,17 +385,19 @@
     DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     DeleteVoiceConnectorTerminationRequestRequestTypeDef,
     DeleteVoiceProfileDomainRequestRequestTypeDef,
     DeleteVoiceProfileRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef,
     SipMediaApplicationAlexaSkillConfigurationTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -413,39 +414,45 @@
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
     TerminationTypeDef,
     GetVoiceProfileDomainRequestRequestTypeDef,
     GetVoiceProfileRequestRequestTypeDef,
     GetVoiceToneAnalysisTaskRequestRequestTypeDef,
+    ListAvailableVoiceConnectorRegionsResponseTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
     ListPhoneNumbersRequestRequestTypeDef,
     ListProxySessionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
+    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     ListVoiceProfileDomainsRequestRequestTypeDef,
     VoiceProfileDomainSummaryTypeDef,
     ListVoiceProfilesRequestRequestTypeDef,
     VoiceProfileSummaryTypeDef,
     MediaInsightsConfigurationTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
+    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
     SpeakerSearchResultTypeDef,
     StartSpeakerSearchTaskRequestRequestTypeDef,
     StartVoiceToneAnalysisTaskRequestRequestTypeDef,
     StopSpeakerSearchTaskRequestRequestTypeDef,
     StopVoiceToneAnalysisTaskRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -459,42 +466,38 @@
     ValidateE911AddressRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
-    ListAvailableVoiceConnectorRegionsResponseTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
     BatchUpdatePhoneNumberRequestRequestTypeDef,
     VoiceToneAnalysisTaskTypeDef,
     ValidateE911AddressResponseTypeDef,
     CreateProxySessionRequestRequestTypeDef,
     CreateSipMediaApplicationCallResponseTypeDef,
     UpdateSipMediaApplicationCallResponseTypeDef,
-    CreateSipMediaApplicationRequestRequestTypeDef,
     SipMediaApplicationTypeDef,
     UpdateSipMediaApplicationRequestRequestTypeDef,
+    CreateSipMediaApplicationRequestRequestTypeDef,
+    CreateVoiceConnectorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateSipRuleRequestRequestTypeDef,
     SipRuleTypeDef,
     UpdateSipRuleRequestRequestTypeDef,
     CreateVoiceConnectorGroupRequestRequestTypeDef,
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
-    VoiceProfileDomainTypeDef,
     CreateVoiceProfileDomainRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    VoiceProfileDomainTypeDef,
     CreateVoiceProfileResponseTypeDef,
     GetVoiceProfileResponseTypeDef,
     UpdateVoiceProfileResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     EmergencyCallingConfigurationTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
@@ -509,16 +512,14 @@
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
     PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
-    ListSipMediaApplicationsRequestListSipMediaApplicationsPaginateTypeDef,
-    ListSipRulesRequestListSipRulesPaginateTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     ListVoiceProfileDomainsResponseTypeDef,
     ListVoiceProfilesResponseTypeDef,
     PhoneNumberOrderTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-voice-1.27.0/mypy_boto3_chime_sdk_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-voice-1.26.98/setup.py` & `mypy-boto3-chime-sdk-voice-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-voice",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_chime_sdk_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKVoice 1.26.98 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.ChimeSDKVoice 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


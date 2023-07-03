# Comparing `tmp/mypy-boto3-voice-id-1.26.100.tar.gz` & `tmp/mypy-boto3-voice-id-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-voice-id-1.26.100.tar", last modified: Mon Mar 27 19:33:18 2023, max compression
+gzip compressed data, was "mypy-boto3-voice-id-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
```

## Comparing `mypy-boto3-voice-id-1.26.100.tar` & `mypy-boto3-voice-id-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:33:18.948113 mypy-boto3-voice-id-1.26.100/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-03-27 19:33:18.948113 mypy-boto3-voice-id-1.26.100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15931 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:33:18.948113 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32427 2023-03-27 19:33:07.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32390 2023-03-27 19:33:07.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:33:18.948113 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-03-27 19:33:18.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-27 19:33:18.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:33:18.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:33:18.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 19:33:18.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 19:33:18.000000 mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:33:18.948113 mypy-boto3-voice-id-1.26.100/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-27 19:33:06.000000 mypy-boto3-voice-id-1.26.100/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-03 19:49:19.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32487 2023-07-03 19:49:19.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32450 2023-07-03 19:49:19.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/setup.py
```

### Comparing `mypy-boto3-voice-id-1.26.100/LICENSE` & `mypy-boto3-voice-id-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.26.100/PKG-INFO` & `mypy-boto3-voice-id-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.26.100
-Summary: Type annotations for boto3.VoiceID 1.26.100 service generated with mypy-boto3-builder 7.14.4
+Version: 1.27.0
+Summary: Type annotations for boto3.VoiceID 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.26.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,15 +353,14 @@
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
-    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -373,42 +372,49 @@
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     RegistrationConfigTypeDef,
     FraudsterSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
@@ -420,20 +426,14 @@
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.26.100/README.md` & `mypy-boto3-voice-id-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.26.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,15 +321,14 @@
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
-    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -341,42 +340,49 @@
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     RegistrationConfigTypeDef,
     FraudsterSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
@@ -388,20 +394,14 @@
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/__init__.py` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/__init__.pyi` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/__main__.py` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VoiceID 1.26.100\nVersion:         1.26.100\nBuilder version:"
-        " 7.14.4\nDocs:           "
+        "Type annotations for boto3.VoiceID 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.100")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/client.py` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/client.pyi` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/literals.py` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -310,16 +313,19 @@
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
@@ -403,15 +409,17 @@
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

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/literals.pyi` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,15 @@
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
@@ -133,14 +134,15 @@
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
@@ -282,14 +284,15 @@
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
@@ -308,16 +311,19 @@
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
@@ -401,15 +407,17 @@
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

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/paginator.py` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,118 +49,110 @@
     "ListFraudsterRegistrationJobsPaginator",
     "ListFraudstersPaginator",
     "ListSpeakerEnrollmentJobsPaginator",
     "ListSpeakersPaginator",
     "ListWatchlistsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
         """
 
-
 class ListFraudsterRegistrationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterregistrationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
-
 class ListFraudstersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterspaginator)
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterspaginator)
         """
 
-
 class ListSpeakerEnrollmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerenrollmentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
-
 class ListSpeakersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpeakersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
         """
 
-
 class ListWatchlistsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWatchlistsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
         """
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/paginator.pyi` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,110 +49,118 @@
     "ListFraudsterRegistrationJobsPaginator",
     "ListFraudstersPaginator",
     "ListSpeakerEnrollmentJobsPaginator",
     "ListSpeakersPaginator",
     "ListWatchlistsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listdomainspaginator)
         """
 
+
 class ListFraudsterRegistrationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterregistrationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
+
 class ListFraudstersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterspaginator)
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listfraudsterspaginator)
         """
 
+
 class ListSpeakerEnrollmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerenrollmentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
+
 class ListSpeakersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSpeakersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listspeakerspaginator)
         """
 
+
 class ListWatchlistsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWatchlistsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/paginators/#listwatchlistspaginator)
         """
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/type_defs.py` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
-    "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
     "CreateWatchlistRequestRequestTypeDef",
     "WatchlistTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteFraudsterRequestRequestTypeDef",
@@ -55,42 +54,49 @@
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "RegistrationConfigTypeDef",
     "FraudsterSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
+    "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListFraudstersRequestRequestTypeDef",
+    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
+    "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
@@ -102,20 +108,14 @@
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
     "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-    "ListFraudstersRequestListFraudstersPaginateTypeDef",
-    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    "ListSpeakersRequestListSpeakersPaginateTypeDef",
-    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
@@ -146,25 +146,14 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
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
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "AcceptanceThreshold": int,
     },
 )
 
@@ -334,14 +323,21 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
         "WatchlistIds": List[str],
     },
@@ -453,33 +449,58 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "DomainId": str,
+        },
+    )
+)
+_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "JobStatus": FraudsterRegistrationJobStatusType,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+
+class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
+    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudsterRegistrationJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
@@ -496,14 +517,37 @@
 class ListFraudsterRegistrationJobsRequestRequestTypeDef(
     _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef,
     _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
+    {
+        "WatchlistId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFraudstersRequestListFraudstersPaginateTypeDef(
+    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
+    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFraudstersRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudstersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudstersRequestRequestTypeDef = TypedDict(
@@ -519,14 +563,37 @@
 
 class ListFraudstersRequestRequestTypeDef(
     _RequiredListFraudstersRequestRequestTypeDef, _OptionalListFraudstersRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "JobStatus": SpeakerEnrollmentJobStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
+    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
@@ -543,14 +610,36 @@
 class ListSpeakerEnrollmentJobsRequestRequestTypeDef(
     _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef,
     _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSpeakersRequestListSpeakersPaginateTypeDef(
+    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
+    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSpeakersRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakersRequestRequestTypeDef = TypedDict(
@@ -586,14 +675,36 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
+    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -630,14 +741,35 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -665,38 +797,31 @@
     pass
 
 
 AssociateFraudsterResponseTypeDef = TypedDict(
     "AssociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFraudsterResponseTypeDef = TypedDict(
     "DescribeFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateFraudsterResponseTypeDef = TypedDict(
     "DisassociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthenticationResultTypeDef = TypedDict(
     "AuthenticationResultTypeDef",
     {
         "AudioAggregationEndedAt": datetime,
@@ -758,15 +883,15 @@
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
         "ResourceArn": str,
@@ -774,47 +899,47 @@
     },
 )
 
 CreateWatchlistResponseTypeDef = TypedDict(
     "CreateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWatchlistResponseTypeDef = TypedDict(
     "DescribeWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWatchlistResponseTypeDef = TypedDict(
     "UpdateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSpeakerResponseTypeDef = TypedDict(
     "DescribeSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OptOutSpeakerResponseTypeDef = TypedDict(
     "OptOutSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "Arn": str,
@@ -942,191 +1067,66 @@
 
 
 ListFraudstersResponseTypeDef = TypedDict(
     "ListFraudstersResponseTypeDef",
     {
         "FraudsterSummaries": List[FraudsterSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "DomainId": str,
-        },
-    )
-)
-_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "JobStatus": FraudsterRegistrationJobStatusType,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-
-class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
-    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "WatchlistId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFraudstersRequestListFraudstersPaginateTypeDef(
-    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
-    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "JobStatus": SpeakerEnrollmentJobStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
-    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSpeakersRequestListSpeakersPaginateTypeDef(
-    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
-    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
-    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
-):
-    pass
-
-
 ListSpeakersResponseTypeDef = TypedDict(
     "ListSpeakersResponseTypeDef",
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
@@ -1187,64 +1187,64 @@
 )
 
 ListFraudsterRegistrationJobsResponseTypeDef = TypedDict(
     "ListFraudsterRegistrationJobsResponseTypeDef",
     {
         "JobSummaries": List[FraudsterRegistrationJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSpeakerEnrollmentJobsResponseTypeDef = TypedDict(
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     {
         "JobSummaries": List[SpeakerEnrollmentJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "StartFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "StartSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EvaluateSessionResponseTypeDef = TypedDict(
     "EvaluateSessionResponseTypeDef",
     {
         "AuthenticationResult": AuthenticationResultTypeDef,
         "DomainId": str,
         "FraudDetectionResult": FraudDetectionResultTypeDef,
         "SessionId": str,
         "SessionName": str,
         "StreamingStatus": StreamingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id/type_defs.pyi` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
-    "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
     "CreateWatchlistRequestRequestTypeDef",
     "WatchlistTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteFraudsterRequestRequestTypeDef",
@@ -54,42 +53,49 @@
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "RegistrationConfigTypeDef",
     "FraudsterSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
+    "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListFraudstersRequestRequestTypeDef",
+    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
+    "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
@@ -101,20 +107,14 @@
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
     "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-    "ListFraudstersRequestListFraudstersPaginateTypeDef",
-    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    "ListSpeakersRequestListSpeakersPaginateTypeDef",
-    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
@@ -145,25 +145,14 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
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
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "AcceptanceThreshold": int,
     },
 )
 
@@ -331,14 +320,21 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
         "WatchlistIds": List[str],
     },
@@ -446,33 +442,56 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "DomainId": str,
+        },
+    )
+)
+_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "JobStatus": FraudsterRegistrationJobStatusType,
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
+    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudsterRegistrationJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
@@ -487,14 +506,35 @@
 
 class ListFraudsterRegistrationJobsRequestRequestTypeDef(
     _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef,
     _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
+    {
+        "WatchlistId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFraudstersRequestListFraudstersPaginateTypeDef(
+    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
+    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
+):
+    pass
+
 _RequiredListFraudstersRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudstersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudstersRequestRequestTypeDef = TypedDict(
@@ -508,14 +548,35 @@
 )
 
 class ListFraudstersRequestRequestTypeDef(
     _RequiredListFraudstersRequestRequestTypeDef, _OptionalListFraudstersRequestRequestTypeDef
 ):
     pass
 
+_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "JobStatus": SpeakerEnrollmentJobStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
+    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
@@ -530,14 +591,34 @@
 
 class ListSpeakerEnrollmentJobsRequestRequestTypeDef(
     _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef,
     _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSpeakersRequestListSpeakersPaginateTypeDef(
+    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
+    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
+):
+    pass
+
 _RequiredListSpeakersRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakersRequestRequestTypeDef = TypedDict(
@@ -571,14 +652,34 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
+    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
+):
+    pass
+
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -613,14 +714,35 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -646,38 +768,31 @@
 ):
     pass
 
 AssociateFraudsterResponseTypeDef = TypedDict(
     "AssociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFraudsterResponseTypeDef = TypedDict(
     "DescribeFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateFraudsterResponseTypeDef = TypedDict(
     "DisassociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthenticationResultTypeDef = TypedDict(
     "AuthenticationResultTypeDef",
     {
         "AudioAggregationEndedAt": datetime,
@@ -735,15 +850,15 @@
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
         "ResourceArn": str,
@@ -751,47 +866,47 @@
     },
 )
 
 CreateWatchlistResponseTypeDef = TypedDict(
     "CreateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWatchlistResponseTypeDef = TypedDict(
     "DescribeWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWatchlistResponseTypeDef = TypedDict(
     "UpdateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSpeakerResponseTypeDef = TypedDict(
     "DescribeSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OptOutSpeakerResponseTypeDef = TypedDict(
     "OptOutSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "Arn": str,
@@ -917,181 +1032,66 @@
     pass
 
 ListFraudstersResponseTypeDef = TypedDict(
     "ListFraudstersResponseTypeDef",
     {
         "FraudsterSummaries": List[FraudsterSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "DomainId": str,
-        },
-    )
-)
-_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "JobStatus": FraudsterRegistrationJobStatusType,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
-    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "WatchlistId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFraudstersRequestListFraudstersPaginateTypeDef(
-    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
-    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
-):
-    pass
-
-_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "JobStatus": SpeakerEnrollmentJobStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
-    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListSpeakersRequestListSpeakersPaginateTypeDef(
-    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
-    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
-):
-    pass
-
-_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
-    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
-):
-    pass
-
 ListSpeakersResponseTypeDef = TypedDict(
     "ListSpeakersResponseTypeDef",
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
@@ -1150,64 +1150,64 @@
 )
 
 ListFraudsterRegistrationJobsResponseTypeDef = TypedDict(
     "ListFraudsterRegistrationJobsResponseTypeDef",
     {
         "JobSummaries": List[FraudsterRegistrationJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSpeakerEnrollmentJobsResponseTypeDef = TypedDict(
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     {
         "JobSummaries": List[SpeakerEnrollmentJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "StartFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "StartSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EvaluateSessionResponseTypeDef = TypedDict(
     "EvaluateSessionResponseTypeDef",
     {
         "AuthenticationResult": AuthenticationResultTypeDef,
         "DomainId": str,
         "FraudDetectionResult": FraudDetectionResultTypeDef,
         "SessionId": str,
         "SessionName": str,
         "StreamingStatus": StreamingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/PKG-INFO` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.26.100
-Summary: Type annotations for boto3.VoiceID 1.26.100 service generated with mypy-boto3-builder 7.14.4
+Version: 1.27.0
+Summary: Type annotations for boto3.VoiceID 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.26.100](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,15 +353,14 @@
 `mypy_boto3_voice_id.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
-    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -373,42 +372,49 @@
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     RegistrationConfigTypeDef,
     FraudsterSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
@@ -420,20 +426,14 @@
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.26.100/mypy_boto3_voice_id.egg-info/SOURCES.txt` & `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.26.100/setup.py` & `mypy-boto3-voice-id-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-voice-id",
-    version="1.26.100",
+    version="1.27.0",
     packages=["mypy_boto3_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VoiceID 1.26.100 service generated with mypy-boto3-builder"
-        " 7.14.4"
+        "Type annotations for boto3.VoiceID 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


# Comparing `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-pinpoint-sms-voice-v2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:51 2022, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-sms-voice-v2-1.27.0.tar", last modified: Mon Jul  3 19:51:15 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1.tar` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:51.012841 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20860 2022-11-01 21:43:51.000841 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19366 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:51.000841 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/
--rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39760 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    39699 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12524 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12522 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14977 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14964 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    46825 2022-11-01 21:39:17.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    46778 2022-11-01 21:39:16.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:51.000841 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20860 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-01 21:43:50.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:51.012841 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-11-01 21:39:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.499808 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20896 2023-07-03 19:51:15.495808 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19358 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.487807 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39760 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39699 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-07-03 19:43:42.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46929 2023-07-03 19:43:43.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46882 2023-07-03 19:43:42.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:40.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.495808 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20896 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 19:51:15.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:15.499808 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-03 19:43:39.000000 mypy-boto3-pinpoint-sms-voice-v2-1.27.0/setup.py
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/LICENSE` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/PKG-INFO` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
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
 
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-sms-voice-v2?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,104 +394,104 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateOriginationIdentityResultTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
+    DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
+    DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
+    DeleteKeywordResultTypeDef,
     DeleteOptOutListRequestRequestTypeDef,
+    DeleteOptOutListResultTypeDef,
     DeleteOptedOutNumberRequestRequestTypeDef,
+    DeleteOptedOutNumberResultTypeDef,
     DeletePoolRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DeletePoolResultTypeDef,
+    DeleteTextMessageSpendLimitOverrideResultTypeDef,
+    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
+    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
     DescribeAccountAttributesRequestRequestTypeDef,
+    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsRequestRequestTypeDef,
     KeywordFilterTypeDef,
     KeywordInformationTypeDef,
+    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeOptOutListsRequestRequestTypeDef,
     OptOutListInformationTypeDef,
     OptedOutFilterTypeDef,
     OptedOutNumberInformationTypeDef,
     PhoneNumberFilterTypeDef,
     PhoneNumberInformationTypeDef,
     PoolFilterTypeDef,
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
+    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
+    DisassociateOriginationIdentityResultTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutKeywordRequestRequestTypeDef,
+    PutKeywordResultTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
+    PutOptedOutNumberResultTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
+    ReleasePhoneNumberResultTypeDef,
+    ResponseMetadataTypeDef,
     SendTextMessageRequestRequestTypeDef,
+    SendTextMessageResultTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
+    SendVoiceMessageResultTypeDef,
     SetDefaultMessageTypeRequestRequestTypeDef,
+    SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdRequestRequestTypeDef,
+    SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideRequestRequestTypeDef,
+    SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef,
+    SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
+    UpdatePhoneNumberResultTypeDef,
     UpdatePoolRequestRequestTypeDef,
-    AssociateOriginationIdentityResultTypeDef,
-    DeleteDefaultMessageTypeResultTypeDef,
-    DeleteDefaultSenderIdResultTypeDef,
-    DeleteKeywordResultTypeDef,
-    DeleteOptOutListResultTypeDef,
-    DeleteOptedOutNumberResultTypeDef,
-    DeletePoolResultTypeDef,
-    DeleteTextMessageSpendLimitOverrideResultTypeDef,
-    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
+    UpdatePoolResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
-    DisassociateOriginationIdentityResultTypeDef,
-    PutKeywordResultTypeDef,
-    PutOptedOutNumberResultTypeDef,
-    ReleasePhoneNumberResultTypeDef,
-    SendTextMessageResultTypeDef,
-    SendVoiceMessageResultTypeDef,
-    SetDefaultMessageTypeResultTypeDef,
-    SetDefaultSenderIdResultTypeDef,
-    SetTextMessageSpendLimitOverrideResultTypeDef,
-    SetVoiceMessageSpendLimitOverrideResultTypeDef,
-    UpdatePhoneNumberResultTypeDef,
-    UpdatePoolResultTypeDef,
+    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateConfigurationSetResultTypeDef,
     CreateOptOutListRequestRequestTypeDef,
     CreateOptOutListResultTypeDef,
     CreatePoolRequestRequestTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
     RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
     EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
-    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
-    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
-    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
-    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
-    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     DescribeKeywordsRequestRequestTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     DescribeOptedOutNumbersRequestRequestTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
@@ -523,42 +524,42 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/README.md` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-pinpoint-sms-voice-v2
+Version: 1.27.0
+Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 pinpoint-sms-voice-v2 type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-sms-voice-v2?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,104 +394,104 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateOriginationIdentityResultTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
+    DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
+    DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
+    DeleteKeywordResultTypeDef,
     DeleteOptOutListRequestRequestTypeDef,
+    DeleteOptOutListResultTypeDef,
     DeleteOptedOutNumberRequestRequestTypeDef,
+    DeleteOptedOutNumberResultTypeDef,
     DeletePoolRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DeletePoolResultTypeDef,
+    DeleteTextMessageSpendLimitOverrideResultTypeDef,
+    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
+    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
     DescribeAccountAttributesRequestRequestTypeDef,
+    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsRequestRequestTypeDef,
     KeywordFilterTypeDef,
     KeywordInformationTypeDef,
+    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeOptOutListsRequestRequestTypeDef,
     OptOutListInformationTypeDef,
     OptedOutFilterTypeDef,
     OptedOutNumberInformationTypeDef,
     PhoneNumberFilterTypeDef,
     PhoneNumberInformationTypeDef,
     PoolFilterTypeDef,
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
+    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
+    DisassociateOriginationIdentityResultTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutKeywordRequestRequestTypeDef,
+    PutKeywordResultTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
+    PutOptedOutNumberResultTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
+    ReleasePhoneNumberResultTypeDef,
+    ResponseMetadataTypeDef,
     SendTextMessageRequestRequestTypeDef,
+    SendTextMessageResultTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
+    SendVoiceMessageResultTypeDef,
     SetDefaultMessageTypeRequestRequestTypeDef,
+    SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdRequestRequestTypeDef,
+    SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideRequestRequestTypeDef,
+    SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef,
+    SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
+    UpdatePhoneNumberResultTypeDef,
     UpdatePoolRequestRequestTypeDef,
-    AssociateOriginationIdentityResultTypeDef,
-    DeleteDefaultMessageTypeResultTypeDef,
-    DeleteDefaultSenderIdResultTypeDef,
-    DeleteKeywordResultTypeDef,
-    DeleteOptOutListResultTypeDef,
-    DeleteOptedOutNumberResultTypeDef,
-    DeletePoolResultTypeDef,
-    DeleteTextMessageSpendLimitOverrideResultTypeDef,
-    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
+    UpdatePoolResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
-    DisassociateOriginationIdentityResultTypeDef,
-    PutKeywordResultTypeDef,
-    PutOptedOutNumberResultTypeDef,
-    ReleasePhoneNumberResultTypeDef,
-    SendTextMessageResultTypeDef,
-    SendVoiceMessageResultTypeDef,
-    SetDefaultMessageTypeResultTypeDef,
-    SetDefaultSenderIdResultTypeDef,
-    SetTextMessageSpendLimitOverrideResultTypeDef,
-    SetVoiceMessageSpendLimitOverrideResultTypeDef,
-    UpdatePhoneNumberResultTypeDef,
-    UpdatePoolResultTypeDef,
+    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateConfigurationSetResultTypeDef,
     CreateOptOutListRequestRequestTypeDef,
     CreateOptOutListResultTypeDef,
     CreatePoolRequestRequestTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
     RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
     EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
-    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
-    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
-    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
-    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
-    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     DescribeKeywordsRequestRequestTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     DescribeOptedOutNumbersRequestRequestTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
@@ -492,42 +524,42 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/__init__.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/client.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/client.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/literals.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,23 +212,25 @@
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
@@ -238,30 +240,35 @@
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
@@ -287,14 +294,15 @@
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
@@ -339,51 +347,57 @@
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
@@ -396,14 +410,15 @@
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
@@ -415,28 +430,35 @@
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
@@ -445,14 +467,15 @@
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
@@ -463,55 +486,64 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -210,23 +210,25 @@
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
@@ -236,30 +238,35 @@
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
@@ -285,14 +292,15 @@
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
@@ -337,51 +345,57 @@
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
@@ -394,14 +408,15 @@
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
@@ -413,28 +428,35 @@
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
@@ -443,14 +465,15 @@
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
@@ -461,55 +484,64 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/paginator.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,30 +94,30 @@
 class DescribeAccountAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountAttributesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
         """
 
 
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
 
@@ -148,15 +148,15 @@
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
 
@@ -166,15 +166,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
 
@@ -186,15 +186,15 @@
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
 
@@ -205,15 +205,15 @@
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
 
@@ -224,15 +224,15 @@
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
 
@@ -243,30 +243,30 @@
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
 
 class DescribeSpendLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSpendLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
         """
 
 
@@ -277,13 +277,13 @@
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,29 +91,29 @@
 class DescribeAccountAttributesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountAttributesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountattributespaginator)
         """
 
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeConfigurationSetsPaginator(Paginator):
@@ -123,15 +123,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationSetNames: Sequence[str] = ...,
         Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeConfigurationSetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeconfigurationsetspaginator)
         """
 
 class DescribeKeywordsPaginator(Paginator):
@@ -142,15 +142,15 @@
 
     def paginate(
         self,
         *,
         OriginationIdentity: str,
         Keywords: Sequence[str] = ...,
         Filters: Sequence[KeywordFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeKeywordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describekeywordspaginator)
         """
 
 class DescribeOptOutListsPaginator(Paginator):
@@ -159,15 +159,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
     """
 
     def paginate(
         self,
         *,
         OptOutListNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOptOutListsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptoutlistspaginator)
         """
 
 class DescribeOptedOutNumbersPaginator(Paginator):
@@ -178,15 +178,15 @@
 
     def paginate(
         self,
         *,
         OptOutListName: str,
         OptedOutNumbers: Sequence[str] = ...,
         Filters: Sequence[OptedOutFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOptedOutNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describeoptedoutnumberspaginator)
         """
 
 class DescribePhoneNumbersPaginator(Paginator):
@@ -196,15 +196,15 @@
     """
 
     def paginate(
         self,
         *,
         PhoneNumberIds: Sequence[str] = ...,
         Filters: Sequence[PhoneNumberFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describephonenumberspaginator)
         """
 
 class DescribePoolsPaginator(Paginator):
@@ -214,15 +214,15 @@
     """
 
     def paginate(
         self,
         *,
         PoolIds: Sequence[str] = ...,
         Filters: Sequence[PoolFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePoolsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describepoolspaginator)
         """
 
 class DescribeSenderIdsPaginator(Paginator):
@@ -232,29 +232,29 @@
     """
 
     def paginate(
         self,
         *,
         SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,
         Filters: Sequence[SenderIdFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSenderIdsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describesenderidspaginator)
         """
 
 class DescribeSpendLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSpendLimitsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#describespendlimitspaginator)
         """
 
 class ListPoolOriginationIdentitiesPaginator(Paginator):
@@ -264,13 +264,13 @@
     """
 
     def paginate(
         self,
         *,
         PoolId: str,
         Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPoolOriginationIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/paginators/#listpooloriginationidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,104 +46,104 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateOriginationIdentityResultTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
+    "DeleteDefaultMessageTypeResultTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
+    "DeleteDefaultSenderIdResultTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
+    "DeleteKeywordResultTypeDef",
     "DeleteOptOutListRequestRequestTypeDef",
+    "DeleteOptOutListResultTypeDef",
     "DeleteOptedOutNumberRequestRequestTypeDef",
+    "DeleteOptedOutNumberResultTypeDef",
     "DeletePoolRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DeletePoolResultTypeDef",
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
     "DescribeAccountAttributesRequestRequestTypeDef",
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsRequestRequestTypeDef",
     "KeywordFilterTypeDef",
     "KeywordInformationTypeDef",
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
     "DescribeOptOutListsRequestRequestTypeDef",
     "OptOutListInformationTypeDef",
     "OptedOutFilterTypeDef",
     "OptedOutNumberInformationTypeDef",
     "PhoneNumberFilterTypeDef",
     "PhoneNumberInformationTypeDef",
     "PoolFilterTypeDef",
     "PoolInformationTypeDef",
     "SenderIdAndCountryTypeDef",
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
+    "DisassociateOriginationIdentityResultTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutKeywordRequestRequestTypeDef",
+    "PutKeywordResultTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
+    "PutOptedOutNumberResultTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
+    "ReleasePhoneNumberResultTypeDef",
+    "ResponseMetadataTypeDef",
     "SendTextMessageRequestRequestTypeDef",
+    "SendTextMessageResultTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
+    "SendVoiceMessageResultTypeDef",
     "SetDefaultMessageTypeRequestRequestTypeDef",
+    "SetDefaultMessageTypeResultTypeDef",
     "SetDefaultSenderIdRequestRequestTypeDef",
+    "SetDefaultSenderIdResultTypeDef",
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
+    "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolRequestRequestTypeDef",
-    "AssociateOriginationIdentityResultTypeDef",
-    "DeleteDefaultMessageTypeResultTypeDef",
-    "DeleteDefaultSenderIdResultTypeDef",
-    "DeleteKeywordResultTypeDef",
-    "DeleteOptOutListResultTypeDef",
-    "DeleteOptedOutNumberResultTypeDef",
-    "DeletePoolResultTypeDef",
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    "UpdatePoolResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "DescribeAccountLimitsResultTypeDef",
-    "DisassociateOriginationIdentityResultTypeDef",
-    "PutKeywordResultTypeDef",
-    "PutOptedOutNumberResultTypeDef",
-    "ReleasePhoneNumberResultTypeDef",
-    "SendTextMessageResultTypeDef",
-    "SendVoiceMessageResultTypeDef",
-    "SetDefaultMessageTypeResultTypeDef",
-    "SetDefaultSenderIdResultTypeDef",
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
-    "UpdatePhoneNumberResultTypeDef",
-    "UpdatePoolResultTypeDef",
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetResultTypeDef",
     "CreateOptOutListRequestRequestTypeDef",
     "CreateOptOutListResultTypeDef",
     "CreatePoolRequestRequestTypeDef",
     "CreatePoolResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "RequestPhoneNumberRequestRequestTypeDef",
     "RequestPhoneNumberResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateEventDestinationRequestRequestTypeDef",
     "EventDestinationTypeDef",
     "UpdateEventDestinationRequestRequestTypeDef",
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     "DescribeKeywordsRequestRequestTypeDef",
     "DescribeKeywordsResultTypeDef",
     "DescribeOptOutListsResultTypeDef",
     "DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     "DescribeOptedOutNumbersRequestRequestTypeDef",
     "DescribeOptedOutNumbersResultTypeDef",
@@ -205,22 +205,23 @@
 class AssociateOriginationIdentityRequestRequestTypeDef(
     _RequiredAssociateOriginationIdentityRequestRequestTypeDef,
     _OptionalAssociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateOriginationIdentityResultTypeDef = TypedDict(
+    "AssociateOriginationIdentityResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
@@ -269,21 +270,41 @@
 DeleteDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+DeleteDefaultMessageTypeResultTypeDef = TypedDict(
+    "DeleteDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+DeleteDefaultSenderIdResultTypeDef = TypedDict(
+    "DeleteDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -292,55 +313,128 @@
     "DeleteKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
     },
 )
 
+DeleteKeywordResultTypeDef = TypedDict(
+    "DeleteKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteOptOutListRequestRequestTypeDef = TypedDict(
     "DeleteOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 
+DeleteOptOutListResultTypeDef = TypedDict(
+    "DeleteOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteOptedOutNumberRequestRequestTypeDef = TypedDict(
     "DeleteOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
+DeleteOptedOutNumberResultTypeDef = TypedDict(
+    "DeleteOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePoolRequestRequestTypeDef = TypedDict(
     "DeletePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeletePoolResultTypeDef = TypedDict(
+    "DeletePoolResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountAttributesRequestRequestTypeDef = TypedDict(
     "DescribeAccountAttributesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAccountLimitsRequestRequestTypeDef = TypedDict(
     "DescribeAccountLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -359,14 +453,23 @@
     {
         "Keyword": str,
         "KeywordMessage": str,
         "KeywordAction": KeywordActionType,
     },
 )
 
+DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
+    {
+        "OptOutListNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeOptOutListsRequestRequestTypeDef = TypedDict(
     "DescribeOptOutListsRequestRequestTypeDef",
     {
         "OptOutListNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -501,14 +604,22 @@
         "SenderId": str,
         "IsoCountryCode": str,
         "MessageTypes": List[MessageTypeType],
         "MonthlyLeasingPrice": str,
     },
 )
 
+DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSpendLimitsRequestRequestTypeDef = TypedDict(
     "DescribeSpendLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -544,14 +655,26 @@
 class DisassociateOriginationIdentityRequestRequestTypeDef(
     _RequiredDisassociateOriginationIdentityRequestRequestTypeDef,
     _OptionalDisassociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
 
+DisassociateOriginationIdentityResultTypeDef = TypedDict(
+    "DisassociateOriginationIdentityResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -569,14 +692,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 _RequiredPutKeywordRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
     },
@@ -592,29 +725,85 @@
 
 class PutKeywordRequestRequestTypeDef(
     _RequiredPutKeywordRequestRequestTypeDef, _OptionalPutKeywordRequestRequestTypeDef
 ):
     pass
 
 
+PutKeywordResultTypeDef = TypedDict(
+    "PutKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutOptedOutNumberRequestRequestTypeDef = TypedDict(
     "PutOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
+PutOptedOutNumberResultTypeDef = TypedDict(
+    "PutOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReleasePhoneNumberRequestRequestTypeDef = TypedDict(
     "ReleasePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
+ReleasePhoneNumberResultTypeDef = TypedDict(
+    "ReleasePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
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
 _RequiredSendTextMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendTextMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
     },
 )
 _OptionalSendTextMessageRequestRequestTypeDef = TypedDict(
@@ -637,14 +826,22 @@
 
 class SendTextMessageRequestRequestTypeDef(
     _RequiredSendTextMessageRequestRequestTypeDef, _OptionalSendTextMessageRequestRequestTypeDef
 ):
     pass
 
 
+SendTextMessageResultTypeDef = TypedDict(
+    "SendTextMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendVoiceMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendVoiceMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": str,
     },
 )
@@ -666,44 +863,88 @@
 
 class SendVoiceMessageRequestRequestTypeDef(
     _RequiredSendVoiceMessageRequestRequestTypeDef, _OptionalSendVoiceMessageRequestRequestTypeDef
 ):
     pass
 
 
+SendVoiceMessageResultTypeDef = TypedDict(
+    "SendVoiceMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "SetDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
     },
 )
 
+SetDefaultMessageTypeResultTypeDef = TypedDict(
+    "SetDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "SetDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "SenderId": str,
     },
 )
 
+SetDefaultSenderIdResultTypeDef = TypedDict(
+    "SetDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetTextMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
+SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
+SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -729,14 +970,36 @@
 
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
 
+UpdatePhoneNumberResultTypeDef = TypedDict(
+    "UpdatePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "DeletionProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 _OptionalUpdatePoolRequestRequestTypeDef = TypedDict(
@@ -755,278 +1018,58 @@
 
 class UpdatePoolRequestRequestTypeDef(
     _RequiredUpdatePoolRequestRequestTypeDef, _OptionalUpdatePoolRequestRequestTypeDef
 ):
     pass
 
 
-AssociateOriginationIdentityResultTypeDef = TypedDict(
-    "AssociateOriginationIdentityResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDefaultMessageTypeResultTypeDef = TypedDict(
-    "DeleteDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDefaultSenderIdResultTypeDef = TypedDict(
-    "DeleteDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteKeywordResultTypeDef = TypedDict(
-    "DeleteKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteOptOutListResultTypeDef = TypedDict(
-    "DeleteOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteOptedOutNumberResultTypeDef = TypedDict(
-    "DeleteOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePoolResultTypeDef = TypedDict(
-    "DeletePoolResultTypeDef",
+UpdatePoolResultTypeDef = TypedDict(
+    "UpdatePoolResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "Status": PoolStatusType,
         "MessageType": MessageTypeType,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountLimitsResultTypeDef = TypedDict(
     "DescribeAccountLimitsResultTypeDef",
     {
         "AccountLimits": List[AccountLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateOriginationIdentityResultTypeDef = TypedDict(
-    "DisassociateOriginationIdentityResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutKeywordResultTypeDef = TypedDict(
-    "PutKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutOptedOutNumberResultTypeDef = TypedDict(
-    "PutOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReleasePhoneNumberResultTypeDef = TypedDict(
-    "ReleasePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendTextMessageResultTypeDef = TypedDict(
-    "SendTextMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendVoiceMessageResultTypeDef = TypedDict(
-    "SendVoiceMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetDefaultMessageTypeResultTypeDef = TypedDict(
-    "SetDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetDefaultSenderIdResultTypeDef = TypedDict(
-    "SetDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePhoneNumberResultTypeDef = TypedDict(
-    "UpdatePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "DeletionProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePoolResultTypeDef = TypedDict(
-    "UpdatePoolResultTypeDef",
+DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
     {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ConfigurationSetNames": Sequence[str],
+        "Filters": Sequence[ConfigurationSetFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 DescribeConfigurationSetsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationSetsRequestRequestTypeDef",
     {
         "ConfigurationSetNames": Sequence[str],
         "Filters": Sequence[ConfigurationSetFilterTypeDef],
@@ -1062,15 +1105,15 @@
 CreateConfigurationSetResultTypeDef = TypedDict(
     "CreateConfigurationSetResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateOptOutListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
@@ -1095,15 +1138,15 @@
 CreateOptOutListResultTypeDef = TypedDict(
     "CreateOptOutListResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePoolRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
@@ -1139,24 +1182,24 @@
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRequestPhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredRequestPhoneNumberRequestRequestTypeDef",
     {
         "IsoCountryCode": str,
@@ -1202,15 +1245,15 @@
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "DeletionProtectionEnabled": bool,
         "PoolId": str,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1291,69 +1334,26 @@
 class UpdateEventDestinationRequestRequestTypeDef(
     _RequiredUpdateEventDestinationRequestRequestTypeDef,
     _OptionalUpdateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
-    {
-        "ConfigurationSetNames": Sequence[str],
-        "Filters": Sequence[ConfigurationSetFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
-    {
-        "OptOutListNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "OriginationIdentity": str,
     },
 )
 _OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "Keywords": Sequence[str],
         "Filters": Sequence[KeywordFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef(
     _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -1389,39 +1389,39 @@
 DescribeKeywordsResultTypeDef = TypedDict(
     "DescribeKeywordsResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keywords": List[KeywordInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOptOutListsResultTypeDef = TypedDict(
     "DescribeOptOutListsResultTypeDef",
     {
         "OptOutLists": List[OptOutListInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptedOutNumbers": Sequence[str],
         "Filters": Sequence[OptedOutFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef(
     _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
@@ -1458,24 +1458,24 @@
 DescribeOptedOutNumbersResultTypeDef = TypedDict(
     "DescribeOptedOutNumbersResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "OptedOutNumbers": List[OptedOutNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = TypedDict(
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
         "Filters": Sequence[PhoneNumberFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePhoneNumbersRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumbersRequestRequestTypeDef",
     {
@@ -1488,24 +1488,24 @@
 )
 
 DescribePhoneNumbersResultTypeDef = TypedDict(
     "DescribePhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePoolsRequestDescribePoolsPaginateTypeDef = TypedDict(
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     {
         "PoolIds": Sequence[str],
         "Filters": Sequence[PoolFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePoolsRequestRequestTypeDef = TypedDict(
     "DescribePoolsRequestRequestTypeDef",
     {
@@ -1518,24 +1518,24 @@
 )
 
 DescribePoolsResultTypeDef = TypedDict(
     "DescribePoolsResultTypeDef",
     {
         "Pools": List[PoolInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = TypedDict(
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     {
         "SenderIds": Sequence[SenderIdAndCountryTypeDef],
         "Filters": Sequence[SenderIdFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeSenderIdsRequestRequestTypeDef = TypedDict(
     "DescribeSenderIdsRequestRequestTypeDef",
     {
@@ -1548,24 +1548,24 @@
 )
 
 DescribeSenderIdsResultTypeDef = TypedDict(
     "DescribeSenderIdsResultTypeDef",
     {
         "SenderIds": List[SenderIdInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSpendLimitsResultTypeDef = TypedDict(
     "DescribeSpendLimitsResultTypeDef",
     {
         "SpendLimits": List[SpendLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
@@ -1574,15 +1574,15 @@
     )
 )
 _OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "Filters": Sequence[PoolOriginationIdentitiesFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
 
 class ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef(
@@ -1619,15 +1619,15 @@
 ListPoolOriginationIdentitiesResultTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentities": List[OriginationIdentityMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfigurationSetInformationTypeDef = TypedDict(
     "_RequiredConfigurationSetInformationTypeDef",
     {
         "ConfigurationSetArn": str,
@@ -1654,52 +1654,52 @@
 
 CreateEventDestinationResultTypeDef = TypedDict(
     "CreateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteConfigurationSetResultTypeDef = TypedDict(
     "DeleteConfigurationSetResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestinations": List[EventDestinationTypeDef],
         "DefaultMessageType": MessageTypeType,
         "DefaultSenderId": str,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventDestinationResultTypeDef = TypedDict(
     "DeleteEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventDestinationResultTypeDef = TypedDict(
     "UpdateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConfigurationSetsResultTypeDef = TypedDict(
     "DescribeConfigurationSetsResultTypeDef",
     {
         "ConfigurationSets": List[ConfigurationSetInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -45,104 +45,104 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAttributeTypeDef",
     "AccountLimitTypeDef",
     "AssociateOriginationIdentityRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateOriginationIdentityResultTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "ConfigurationSetFilterTypeDef",
     "TagTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
+    "DeleteDefaultMessageTypeResultTypeDef",
     "DeleteDefaultSenderIdRequestRequestTypeDef",
+    "DeleteDefaultSenderIdResultTypeDef",
     "DeleteEventDestinationRequestRequestTypeDef",
     "DeleteKeywordRequestRequestTypeDef",
+    "DeleteKeywordResultTypeDef",
     "DeleteOptOutListRequestRequestTypeDef",
+    "DeleteOptOutListResultTypeDef",
     "DeleteOptedOutNumberRequestRequestTypeDef",
+    "DeleteOptedOutNumberResultTypeDef",
     "DeletePoolRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DeletePoolResultTypeDef",
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
     "DescribeAccountAttributesRequestRequestTypeDef",
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsRequestRequestTypeDef",
     "KeywordFilterTypeDef",
     "KeywordInformationTypeDef",
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
     "DescribeOptOutListsRequestRequestTypeDef",
     "OptOutListInformationTypeDef",
     "OptedOutFilterTypeDef",
     "OptedOutNumberInformationTypeDef",
     "PhoneNumberFilterTypeDef",
     "PhoneNumberInformationTypeDef",
     "PoolFilterTypeDef",
     "PoolInformationTypeDef",
     "SenderIdAndCountryTypeDef",
     "SenderIdFilterTypeDef",
     "SenderIdInformationTypeDef",
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeSpendLimitsRequestRequestTypeDef",
     "SpendLimitTypeDef",
     "DisassociateOriginationIdentityRequestRequestTypeDef",
+    "DisassociateOriginationIdentityResultTypeDef",
     "PoolOriginationIdentitiesFilterTypeDef",
     "OriginationIdentityMetadataTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutKeywordRequestRequestTypeDef",
+    "PutKeywordResultTypeDef",
     "PutOptedOutNumberRequestRequestTypeDef",
+    "PutOptedOutNumberResultTypeDef",
     "ReleasePhoneNumberRequestRequestTypeDef",
+    "ReleasePhoneNumberResultTypeDef",
+    "ResponseMetadataTypeDef",
     "SendTextMessageRequestRequestTypeDef",
+    "SendTextMessageResultTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
+    "SendVoiceMessageResultTypeDef",
     "SetDefaultMessageTypeRequestRequestTypeDef",
+    "SetDefaultMessageTypeResultTypeDef",
     "SetDefaultSenderIdRequestRequestTypeDef",
+    "SetDefaultSenderIdResultTypeDef",
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
+    "UpdatePhoneNumberResultTypeDef",
     "UpdatePoolRequestRequestTypeDef",
-    "AssociateOriginationIdentityResultTypeDef",
-    "DeleteDefaultMessageTypeResultTypeDef",
-    "DeleteDefaultSenderIdResultTypeDef",
-    "DeleteKeywordResultTypeDef",
-    "DeleteOptOutListResultTypeDef",
-    "DeleteOptedOutNumberResultTypeDef",
-    "DeletePoolResultTypeDef",
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    "UpdatePoolResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "DescribeAccountLimitsResultTypeDef",
-    "DisassociateOriginationIdentityResultTypeDef",
-    "PutKeywordResultTypeDef",
-    "PutOptedOutNumberResultTypeDef",
-    "ReleasePhoneNumberResultTypeDef",
-    "SendTextMessageResultTypeDef",
-    "SendVoiceMessageResultTypeDef",
-    "SetDefaultMessageTypeResultTypeDef",
-    "SetDefaultSenderIdResultTypeDef",
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
-    "UpdatePhoneNumberResultTypeDef",
-    "UpdatePoolResultTypeDef",
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
     "DescribeConfigurationSetsRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetResultTypeDef",
     "CreateOptOutListRequestRequestTypeDef",
     "CreateOptOutListResultTypeDef",
     "CreatePoolRequestRequestTypeDef",
     "CreatePoolResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "RequestPhoneNumberRequestRequestTypeDef",
     "RequestPhoneNumberResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateEventDestinationRequestRequestTypeDef",
     "EventDestinationTypeDef",
     "UpdateEventDestinationRequestRequestTypeDef",
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
     "DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     "DescribeKeywordsRequestRequestTypeDef",
     "DescribeKeywordsResultTypeDef",
     "DescribeOptOutListsResultTypeDef",
     "DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     "DescribeOptedOutNumbersRequestRequestTypeDef",
     "DescribeOptedOutNumbersResultTypeDef",
@@ -202,22 +202,23 @@
 
 class AssociateOriginationIdentityRequestRequestTypeDef(
     _RequiredAssociateOriginationIdentityRequestRequestTypeDef,
     _OptionalAssociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateOriginationIdentityResultTypeDef = TypedDict(
+    "AssociateOriginationIdentityResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CloudWatchLogsDestinationTypeDef = TypedDict(
     "CloudWatchLogsDestinationTypeDef",
     {
         "IamRoleArn": str,
@@ -266,21 +267,41 @@
 DeleteDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "DeleteDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+DeleteDefaultMessageTypeResultTypeDef = TypedDict(
+    "DeleteDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "DeleteDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+DeleteDefaultSenderIdResultTypeDef = TypedDict(
+    "DeleteDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -289,55 +310,128 @@
     "DeleteKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
     },
 )
 
+DeleteKeywordResultTypeDef = TypedDict(
+    "DeleteKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteOptOutListRequestRequestTypeDef = TypedDict(
     "DeleteOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
     },
 )
 
+DeleteOptOutListResultTypeDef = TypedDict(
+    "DeleteOptOutListResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteOptedOutNumberRequestRequestTypeDef = TypedDict(
     "DeleteOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
+DeleteOptedOutNumberResultTypeDef = TypedDict(
+    "DeleteOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePoolRequestRequestTypeDef = TypedDict(
     "DeletePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeletePoolResultTypeDef = TypedDict(
+    "DeletePoolResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PoolArn": str,
+        "PoolId": str,
+        "Status": PoolStatusType,
+        "MessageType": MessageTypeType,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "SharedRoutesEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
+    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountAttributesRequestRequestTypeDef = TypedDict(
     "DescribeAccountAttributesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAccountLimitsRequestRequestTypeDef = TypedDict(
     "DescribeAccountLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -356,14 +450,23 @@
     {
         "Keyword": str,
         "KeywordMessage": str,
         "KeywordAction": KeywordActionType,
     },
 )
 
+DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
+    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
+    {
+        "OptOutListNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeOptOutListsRequestRequestTypeDef = TypedDict(
     "DescribeOptOutListsRequestRequestTypeDef",
     {
         "OptOutListNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -494,14 +597,22 @@
         "SenderId": str,
         "IsoCountryCode": str,
         "MessageTypes": List[MessageTypeType],
         "MonthlyLeasingPrice": str,
     },
 )
 
+DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
+    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSpendLimitsRequestRequestTypeDef = TypedDict(
     "DescribeSpendLimitsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -535,14 +646,26 @@
 
 class DisassociateOriginationIdentityRequestRequestTypeDef(
     _RequiredDisassociateOriginationIdentityRequestRequestTypeDef,
     _OptionalDisassociateOriginationIdentityRequestRequestTypeDef,
 ):
     pass
 
+DisassociateOriginationIdentityResultTypeDef = TypedDict(
+    "DisassociateOriginationIdentityResultTypeDef",
+    {
+        "PoolArn": str,
+        "PoolId": str,
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "IsoCountryCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PoolOriginationIdentitiesFilterTypeDef = TypedDict(
     "PoolOriginationIdentitiesFilterTypeDef",
     {
         "Name": PoolOriginationIdentitiesFilterNameType,
         "Values": Sequence[str],
     },
 )
@@ -560,14 +683,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 _RequiredPutKeywordRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeywordRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
         "Keyword": str,
         "KeywordMessage": str,
     },
@@ -581,29 +714,85 @@
 )
 
 class PutKeywordRequestRequestTypeDef(
     _RequiredPutKeywordRequestRequestTypeDef, _OptionalPutKeywordRequestRequestTypeDef
 ):
     pass
 
+PutKeywordResultTypeDef = TypedDict(
+    "PutKeywordResultTypeDef",
+    {
+        "OriginationIdentityArn": str,
+        "OriginationIdentity": str,
+        "Keyword": str,
+        "KeywordMessage": str,
+        "KeywordAction": KeywordActionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutOptedOutNumberRequestRequestTypeDef = TypedDict(
     "PutOptedOutNumberRequestRequestTypeDef",
     {
         "OptOutListName": str,
         "OptedOutNumber": str,
     },
 )
 
+PutOptedOutNumberResultTypeDef = TypedDict(
+    "PutOptedOutNumberResultTypeDef",
+    {
+        "OptOutListArn": str,
+        "OptOutListName": str,
+        "OptedOutNumber": str,
+        "OptedOutTimestamp": datetime,
+        "EndUserOptedOut": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReleasePhoneNumberRequestRequestTypeDef = TypedDict(
     "ReleasePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
+ReleasePhoneNumberResultTypeDef = TypedDict(
+    "ReleasePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "CreatedTimestamp": datetime,
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
 _RequiredSendTextMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendTextMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
     },
 )
 _OptionalSendTextMessageRequestRequestTypeDef = TypedDict(
@@ -624,14 +813,22 @@
 )
 
 class SendTextMessageRequestRequestTypeDef(
     _RequiredSendTextMessageRequestRequestTypeDef, _OptionalSendTextMessageRequestRequestTypeDef
 ):
     pass
 
+SendTextMessageResultTypeDef = TypedDict(
+    "SendTextMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSendVoiceMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendVoiceMessageRequestRequestTypeDef",
     {
         "DestinationPhoneNumber": str,
         "OriginationIdentity": str,
     },
 )
@@ -651,44 +848,88 @@
 )
 
 class SendVoiceMessageRequestRequestTypeDef(
     _RequiredSendVoiceMessageRequestRequestTypeDef, _OptionalSendVoiceMessageRequestRequestTypeDef
 ):
     pass
 
+SendVoiceMessageResultTypeDef = TypedDict(
+    "SendVoiceMessageResultTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetDefaultMessageTypeRequestRequestTypeDef = TypedDict(
     "SetDefaultMessageTypeRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "MessageType": MessageTypeType,
     },
 )
 
+SetDefaultMessageTypeResultTypeDef = TypedDict(
+    "SetDefaultMessageTypeResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "MessageType": MessageTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetDefaultSenderIdRequestRequestTypeDef = TypedDict(
     "SetDefaultSenderIdRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "SenderId": str,
     },
 )
 
+SetDefaultSenderIdResultTypeDef = TypedDict(
+    "SetDefaultSenderIdResultTypeDef",
+    {
+        "ConfigurationSetArn": str,
+        "ConfigurationSetName": str,
+        "SenderId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetTextMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetTextMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
+SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetTextMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef = TypedDict(
     "SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef",
     {
         "MonthlyLimit": int,
     },
 )
 
+SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
+    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
+    {
+        "MonthlyLimit": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -712,14 +953,36 @@
 )
 
 class UpdatePhoneNumberRequestRequestTypeDef(
     _RequiredUpdatePhoneNumberRequestRequestTypeDef, _OptionalUpdatePhoneNumberRequestRequestTypeDef
 ):
     pass
 
+UpdatePhoneNumberResultTypeDef = TypedDict(
+    "UpdatePhoneNumberResultTypeDef",
+    {
+        "PhoneNumberArn": str,
+        "PhoneNumberId": str,
+        "PhoneNumber": str,
+        "Status": NumberStatusType,
+        "IsoCountryCode": str,
+        "MessageType": MessageTypeType,
+        "NumberCapabilities": List[NumberCapabilityType],
+        "NumberType": NumberTypeType,
+        "MonthlyLeasingPrice": str,
+        "TwoWayEnabled": bool,
+        "TwoWayChannelArn": str,
+        "SelfManagedOptOutsEnabled": bool,
+        "OptOutListName": str,
+        "DeletionProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePoolRequestRequestTypeDef",
     {
         "PoolId": str,
     },
 )
 _OptionalUpdatePoolRequestRequestTypeDef = TypedDict(
@@ -736,278 +999,58 @@
 )
 
 class UpdatePoolRequestRequestTypeDef(
     _RequiredUpdatePoolRequestRequestTypeDef, _OptionalUpdatePoolRequestRequestTypeDef
 ):
     pass
 
-AssociateOriginationIdentityResultTypeDef = TypedDict(
-    "AssociateOriginationIdentityResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDefaultMessageTypeResultTypeDef = TypedDict(
-    "DeleteDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDefaultSenderIdResultTypeDef = TypedDict(
-    "DeleteDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteKeywordResultTypeDef = TypedDict(
-    "DeleteKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteOptOutListResultTypeDef = TypedDict(
-    "DeleteOptOutListResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteOptedOutNumberResultTypeDef = TypedDict(
-    "DeleteOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePoolResultTypeDef = TypedDict(
-    "DeletePoolResultTypeDef",
+UpdatePoolResultTypeDef = TypedDict(
+    "UpdatePoolResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "Status": PoolStatusType,
         "MessageType": MessageTypeType,
         "TwoWayEnabled": bool,
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
+        "DeletionProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "DeleteVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccountLimitsResultTypeDef = TypedDict(
     "DescribeAccountLimitsResultTypeDef",
     {
         "AccountLimits": List[AccountLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateOriginationIdentityResultTypeDef = TypedDict(
-    "DisassociateOriginationIdentityResultTypeDef",
-    {
-        "PoolArn": str,
-        "PoolId": str,
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "IsoCountryCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutKeywordResultTypeDef = TypedDict(
-    "PutKeywordResultTypeDef",
-    {
-        "OriginationIdentityArn": str,
-        "OriginationIdentity": str,
-        "Keyword": str,
-        "KeywordMessage": str,
-        "KeywordAction": KeywordActionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutOptedOutNumberResultTypeDef = TypedDict(
-    "PutOptedOutNumberResultTypeDef",
-    {
-        "OptOutListArn": str,
-        "OptOutListName": str,
-        "OptedOutNumber": str,
-        "OptedOutTimestamp": datetime,
-        "EndUserOptedOut": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ReleasePhoneNumberResultTypeDef = TypedDict(
-    "ReleasePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendTextMessageResultTypeDef = TypedDict(
-    "SendTextMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendVoiceMessageResultTypeDef = TypedDict(
-    "SendVoiceMessageResultTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetDefaultMessageTypeResultTypeDef = TypedDict(
-    "SetDefaultMessageTypeResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "MessageType": MessageTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetDefaultSenderIdResultTypeDef = TypedDict(
-    "SetDefaultSenderIdResultTypeDef",
-    {
-        "ConfigurationSetArn": str,
-        "ConfigurationSetName": str,
-        "SenderId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetTextMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetTextMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetVoiceMessageSpendLimitOverrideResultTypeDef = TypedDict(
-    "SetVoiceMessageSpendLimitOverrideResultTypeDef",
-    {
-        "MonthlyLimit": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePhoneNumberResultTypeDef = TypedDict(
-    "UpdatePhoneNumberResultTypeDef",
-    {
-        "PhoneNumberArn": str,
-        "PhoneNumberId": str,
-        "PhoneNumber": str,
-        "Status": NumberStatusType,
-        "IsoCountryCode": str,
-        "MessageType": MessageTypeType,
-        "NumberCapabilities": List[NumberCapabilityType],
-        "NumberType": NumberTypeType,
-        "MonthlyLeasingPrice": str,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "DeletionProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePoolResultTypeDef = TypedDict(
-    "UpdatePoolResultTypeDef",
+DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
     {
-        "PoolArn": str,
-        "PoolId": str,
-        "Status": PoolStatusType,
-        "MessageType": MessageTypeType,
-        "TwoWayEnabled": bool,
-        "TwoWayChannelArn": str,
-        "SelfManagedOptOutsEnabled": bool,
-        "OptOutListName": str,
-        "SharedRoutesEnabled": bool,
-        "DeletionProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ConfigurationSetNames": Sequence[str],
+        "Filters": Sequence[ConfigurationSetFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
 DescribeConfigurationSetsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationSetsRequestRequestTypeDef",
     {
         "ConfigurationSetNames": Sequence[str],
         "Filters": Sequence[ConfigurationSetFilterTypeDef],
@@ -1041,15 +1084,15 @@
 CreateConfigurationSetResultTypeDef = TypedDict(
     "CreateConfigurationSetResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateOptOutListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOptOutListRequestRequestTypeDef",
     {
         "OptOutListName": str,
@@ -1072,15 +1115,15 @@
 CreateOptOutListResultTypeDef = TypedDict(
     "CreateOptOutListResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePoolRequestRequestTypeDef",
     {
         "OriginationIdentity": str,
@@ -1114,24 +1157,24 @@
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "SharedRoutesEnabled": bool,
         "DeletionProtectionEnabled": bool,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRequestPhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredRequestPhoneNumberRequestRequestTypeDef",
     {
         "IsoCountryCode": str,
@@ -1175,15 +1218,15 @@
         "TwoWayChannelArn": str,
         "SelfManagedOptOutsEnabled": bool,
         "OptOutListName": str,
         "DeletionProtectionEnabled": bool,
         "PoolId": str,
         "Tags": List[TagTypeDef],
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1258,69 +1301,26 @@
 
 class UpdateEventDestinationRequestRequestTypeDef(
     _RequiredUpdateEventDestinationRequestRequestTypeDef,
     _OptionalUpdateEventDestinationRequestRequestTypeDef,
 ):
     pass
 
-DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = TypedDict(
-    "DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef",
-    {
-        "ConfigurationSetNames": Sequence[str],
-        "Filters": Sequence[ConfigurationSetFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = TypedDict(
-    "DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef",
-    {
-        "OptOutListNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = TypedDict(
-    "DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "OriginationIdentity": str,
     },
 )
 _OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = TypedDict(
     "_OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef",
     {
         "Keywords": Sequence[str],
         "Filters": Sequence[KeywordFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef(
     _RequiredDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     _OptionalDescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
@@ -1352,39 +1352,39 @@
 DescribeKeywordsResultTypeDef = TypedDict(
     "DescribeKeywordsResultTypeDef",
     {
         "OriginationIdentityArn": str,
         "OriginationIdentity": str,
         "Keywords": List[KeywordInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOptOutListsResultTypeDef = TypedDict(
     "DescribeOptOutListsResultTypeDef",
     {
         "OptOutLists": List[OptOutListInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptOutListName": str,
     },
 )
 _OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = TypedDict(
     "_OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef",
     {
         "OptedOutNumbers": Sequence[str],
         "Filters": Sequence[OptedOutFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef(
     _RequiredDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     _OptionalDescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
@@ -1417,24 +1417,24 @@
 DescribeOptedOutNumbersResultTypeDef = TypedDict(
     "DescribeOptedOutNumbersResultTypeDef",
     {
         "OptOutListArn": str,
         "OptOutListName": str,
         "OptedOutNumbers": List[OptedOutNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = TypedDict(
     "DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef",
     {
         "PhoneNumberIds": Sequence[str],
         "Filters": Sequence[PhoneNumberFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePhoneNumbersRequestRequestTypeDef = TypedDict(
     "DescribePhoneNumbersRequestRequestTypeDef",
     {
@@ -1447,24 +1447,24 @@
 )
 
 DescribePhoneNumbersResultTypeDef = TypedDict(
     "DescribePhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePoolsRequestDescribePoolsPaginateTypeDef = TypedDict(
     "DescribePoolsRequestDescribePoolsPaginateTypeDef",
     {
         "PoolIds": Sequence[str],
         "Filters": Sequence[PoolFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribePoolsRequestRequestTypeDef = TypedDict(
     "DescribePoolsRequestRequestTypeDef",
     {
@@ -1477,24 +1477,24 @@
 )
 
 DescribePoolsResultTypeDef = TypedDict(
     "DescribePoolsResultTypeDef",
     {
         "Pools": List[PoolInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = TypedDict(
     "DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef",
     {
         "SenderIds": Sequence[SenderIdAndCountryTypeDef],
         "Filters": Sequence[SenderIdFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeSenderIdsRequestRequestTypeDef = TypedDict(
     "DescribeSenderIdsRequestRequestTypeDef",
     {
@@ -1507,24 +1507,24 @@
 )
 
 DescribeSenderIdsResultTypeDef = TypedDict(
     "DescribeSenderIdsResultTypeDef",
     {
         "SenderIds": List[SenderIdInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSpendLimitsResultTypeDef = TypedDict(
     "DescribeSpendLimitsResultTypeDef",
     {
         "SpendLimits": List[SpendLimitTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
@@ -1533,15 +1533,15 @@
     )
 )
 _OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = (
     TypedDict(
         "_OptionalListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef",
         {
             "Filters": Sequence[PoolOriginationIdentitiesFilterTypeDef],
-            "PaginationConfig": PaginatorConfigTypeDef,
+            "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
 class ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef(
     _RequiredListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef,
@@ -1574,15 +1574,15 @@
 ListPoolOriginationIdentitiesResultTypeDef = TypedDict(
     "ListPoolOriginationIdentitiesResultTypeDef",
     {
         "PoolArn": str,
         "PoolId": str,
         "OriginationIdentities": List[OriginationIdentityMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfigurationSetInformationTypeDef = TypedDict(
     "_RequiredConfigurationSetInformationTypeDef",
     {
         "ConfigurationSetArn": str,
@@ -1607,52 +1607,52 @@
 
 CreateEventDestinationResultTypeDef = TypedDict(
     "CreateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteConfigurationSetResultTypeDef = TypedDict(
     "DeleteConfigurationSetResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestinations": List[EventDestinationTypeDef],
         "DefaultMessageType": MessageTypeType,
         "DefaultSenderId": str,
         "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventDestinationResultTypeDef = TypedDict(
     "DeleteEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEventDestinationResultTypeDef = TypedDict(
     "UpdateEventDestinationResultTypeDef",
     {
         "ConfigurationSetArn": str,
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConfigurationSetsResultTypeDef = TypedDict(
     "DescribeConfigurationSetsResultTypeDef",
     {
         "ConfigurationSets": List[ConfigurationSetInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-pinpoint-sms-voice-v2
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.PinpointSMSVoiceV2 1.26.0 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pinpoint-sms-voice-v2 type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-pinpoint-sms-voice-v2"></a>
 
 # mypy-boto3-pinpoint-sms-voice-v2
 
 [![PyPI - mypy-boto3-pinpoint-sms-voice-v2](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-sms-voice-v2.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-sms-voice-v2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-sms-voice-v2?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-sms-voice-v2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointSMSVoiceV2 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
+[boto3.PinpointSMSVoiceV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#PinpointSMSVoiceV2)
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
 [mypy-boto3-pinpoint-sms-voice-v2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,104 +362,104 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_sms_voice_v2.type_defs import (
     AccountAttributeTypeDef,
     AccountLimitTypeDef,
     AssociateOriginationIdentityRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateOriginationIdentityResultTypeDef,
     CloudWatchLogsDestinationTypeDef,
     ConfigurationSetFilterTypeDef,
     TagTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDefaultMessageTypeRequestRequestTypeDef,
+    DeleteDefaultMessageTypeResultTypeDef,
     DeleteDefaultSenderIdRequestRequestTypeDef,
+    DeleteDefaultSenderIdResultTypeDef,
     DeleteEventDestinationRequestRequestTypeDef,
     DeleteKeywordRequestRequestTypeDef,
+    DeleteKeywordResultTypeDef,
     DeleteOptOutListRequestRequestTypeDef,
+    DeleteOptOutListResultTypeDef,
     DeleteOptedOutNumberRequestRequestTypeDef,
+    DeleteOptedOutNumberResultTypeDef,
     DeletePoolRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DeletePoolResultTypeDef,
+    DeleteTextMessageSpendLimitOverrideResultTypeDef,
+    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
+    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
     DescribeAccountAttributesRequestRequestTypeDef,
+    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsRequestRequestTypeDef,
     KeywordFilterTypeDef,
     KeywordInformationTypeDef,
+    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
     DescribeOptOutListsRequestRequestTypeDef,
     OptOutListInformationTypeDef,
     OptedOutFilterTypeDef,
     OptedOutNumberInformationTypeDef,
     PhoneNumberFilterTypeDef,
     PhoneNumberInformationTypeDef,
     PoolFilterTypeDef,
     PoolInformationTypeDef,
     SenderIdAndCountryTypeDef,
     SenderIdFilterTypeDef,
     SenderIdInformationTypeDef,
+    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeSpendLimitsRequestRequestTypeDef,
     SpendLimitTypeDef,
     DisassociateOriginationIdentityRequestRequestTypeDef,
+    DisassociateOriginationIdentityResultTypeDef,
     PoolOriginationIdentitiesFilterTypeDef,
     OriginationIdentityMetadataTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutKeywordRequestRequestTypeDef,
+    PutKeywordResultTypeDef,
     PutOptedOutNumberRequestRequestTypeDef,
+    PutOptedOutNumberResultTypeDef,
     ReleasePhoneNumberRequestRequestTypeDef,
+    ReleasePhoneNumberResultTypeDef,
+    ResponseMetadataTypeDef,
     SendTextMessageRequestRequestTypeDef,
+    SendTextMessageResultTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
+    SendVoiceMessageResultTypeDef,
     SetDefaultMessageTypeRequestRequestTypeDef,
+    SetDefaultMessageTypeResultTypeDef,
     SetDefaultSenderIdRequestRequestTypeDef,
+    SetDefaultSenderIdResultTypeDef,
     SetTextMessageSpendLimitOverrideRequestRequestTypeDef,
+    SetTextMessageSpendLimitOverrideResultTypeDef,
     SetVoiceMessageSpendLimitOverrideRequestRequestTypeDef,
+    SetVoiceMessageSpendLimitOverrideResultTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
+    UpdatePhoneNumberResultTypeDef,
     UpdatePoolRequestRequestTypeDef,
-    AssociateOriginationIdentityResultTypeDef,
-    DeleteDefaultMessageTypeResultTypeDef,
-    DeleteDefaultSenderIdResultTypeDef,
-    DeleteKeywordResultTypeDef,
-    DeleteOptOutListResultTypeDef,
-    DeleteOptedOutNumberResultTypeDef,
-    DeletePoolResultTypeDef,
-    DeleteTextMessageSpendLimitOverrideResultTypeDef,
-    DeleteVoiceMessageSpendLimitOverrideResultTypeDef,
+    UpdatePoolResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeAccountLimitsResultTypeDef,
-    DisassociateOriginationIdentityResultTypeDef,
-    PutKeywordResultTypeDef,
-    PutOptedOutNumberResultTypeDef,
-    ReleasePhoneNumberResultTypeDef,
-    SendTextMessageResultTypeDef,
-    SendVoiceMessageResultTypeDef,
-    SetDefaultMessageTypeResultTypeDef,
-    SetDefaultSenderIdResultTypeDef,
-    SetTextMessageSpendLimitOverrideResultTypeDef,
-    SetVoiceMessageSpendLimitOverrideResultTypeDef,
-    UpdatePhoneNumberResultTypeDef,
-    UpdatePoolResultTypeDef,
+    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
     DescribeConfigurationSetsRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateConfigurationSetResultTypeDef,
     CreateOptOutListRequestRequestTypeDef,
     CreateOptOutListResultTypeDef,
     CreatePoolRequestRequestTypeDef,
     CreatePoolResultTypeDef,
     ListTagsForResourceResultTypeDef,
     RequestPhoneNumberRequestRequestTypeDef,
     RequestPhoneNumberResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateEventDestinationRequestRequestTypeDef,
     EventDestinationTypeDef,
     UpdateEventDestinationRequestRequestTypeDef,
-    DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef,
-    DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef,
-    DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef,
-    DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef,
-    DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef,
     DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef,
     DescribeKeywordsRequestRequestTypeDef,
     DescribeKeywordsResultTypeDef,
     DescribeOptOutListsResultTypeDef,
     DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef,
     DescribeOptedOutNumbersRequestRequestTypeDef,
     DescribeOptedOutNumbersResultTypeDef,
@@ -523,42 +492,42 @@
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

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/mypy_boto3_pinpoint_sms_voice_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-sms-voice-v2-1.26.0.post1/setup.py` & `mypy-boto3-pinpoint-sms-voice-v2-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-pinpoint-sms-voice-v2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-sms-voice-v2",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_pinpoint_sms_voice_v2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointSMSVoiceV2 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.PinpointSMSVoiceV2 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 pinpoint-sms-voice-v2 type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_pinpoint_sms_voice_v2": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_pinpoint_sms_voice_v2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_sms_voice_v2/"
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


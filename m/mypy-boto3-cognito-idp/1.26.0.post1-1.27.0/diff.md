# Comparing `tmp/mypy-boto3-cognito-idp-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cognito-idp-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-idp-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:16 2022, max compression
+gzip compressed data, was "mypy-boto3-cognito-idp-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-cognito-idp-1.26.0.post1.tar` & `mypy-boto3-cognito-idp-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:16.144819 mypy-boto3-cognito-idp-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    25152 2022-11-01 21:43:16.144819 mypy-boto3-cognito-idp-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23683 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:16.144819 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    78755 2022-11-01 21:32:05.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    78638 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12898 2022-11-01 21:32:05.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    12896 2022-11-01 21:32:05.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11048 2022-11-01 21:32:05.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11037 2022-11-01 21:32:05.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    97256 2022-11-01 21:32:07.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    97117 2022-11-01 21:32:06.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:16.144819 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    25152 2022-11-01 21:43:15.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-01 21:43:15.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:15.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-01 21:43:15.000000 mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:16.144819 mypy-boto3-cognito-idp-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-11-01 21:32:04.000000 mypy-boto3-cognito-idp-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.179028 mypy-boto3-cognito-idp-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-03 19:50:34.179028 mypy-boto3-cognito-idp-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.175028 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-03 19:34:35.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-03 19:34:35.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97444 2023-07-03 19:34:37.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97305 2023-07-03 19:34:36.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.179028 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-03 19:50:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-03 19:50:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 19:50:34.000000 mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.179028 mypy-boto3-cognito-idp-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-03 19:34:34.000000 mypy-boto3-cognito-idp-1.27.0/setup.py
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/LICENSE` & `mypy-boto3-cognito-idp-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/PKG-INFO` & `mypy-boto3-cognito-idp-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
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
 
 <a id="mypy-boto3-cognito-idp"></a>
 
 # mypy-boto3-cognito-idp
 
 [![PyPI - mypy-boto3-cognito-idp](https://img.shields.io/pypi/v/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,59 +400,62 @@
 from mypy_boto3_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
-    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
+    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -468,88 +472,85 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
+    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
+    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
+    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
+    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
-    ConfirmDeviceResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
@@ -645,42 +646,42 @@
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

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/README.md` & `mypy-boto3-cognito-idp-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cognito-idp"></a>
 
 # mypy-boto3-cognito-idp
 
 [![PyPI - mypy-boto3-cognito-idp](https://img.shields.io/pypi/v/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,59 +368,62 @@
 from mypy_boto3_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
-    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
+    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -437,88 +440,85 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
+    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
+    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
+    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
+    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
-    ConfirmDeviceResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
@@ -614,42 +614,42 @@
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

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/__init__.py` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/__init__.pyi` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/__main__.py` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentityProvider 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CognitoIdentityProvider 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/client.py` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,16 +365,16 @@
         self,
         *,
         UserPoolId: str,
         DestinationUser: ProviderUserIdentifierTypeTypeDef,
         SourceUser: ProviderUserIdentifierTypeTypeDef
     ) -> Dict[str, Any]:
         """
-        Links an existing user account in a user pool (`DestinationUser` ) to an
-        identity from an external IdP (`SourceUser` ) based on a specified attribute
+        Links an existing user account in a user pool ( `DestinationUser`) to an
+        identity from an external IdP ( `SourceUser`) based on a specified attribute
         name and value from the external IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_link_provider_for_user)
         """
 
     def admin_list_devices(
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/client.pyi` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         self,
         *,
         UserPoolId: str,
         DestinationUser: ProviderUserIdentifierTypeTypeDef,
         SourceUser: ProviderUserIdentifierTypeTypeDef
     ) -> Dict[str, Any]:
         """
-        Links an existing user account in a user pool (`DestinationUser` ) to an
-        identity from an external IdP (`SourceUser` ) based on a specified attribute
+        Links an existing user account in a user pool ( `DestinationUser`) to an
+        identity from an external IdP ( `SourceUser`) based on a specified attribute
         name and value from the external IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_link_provider_for_user)
         """
     def admin_list_devices(
         self, *, UserPoolId: str, Username: str, Limit: int = ..., PaginationToken: str = ...
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/literals.py` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountTakeoverEventActionTypeType",
     "AdminListGroupsForUserPaginatorName",
     "AdminListUserAuthEventsPaginatorName",
     "AdvancedSecurityModeTypeType",
     "AliasAttributeTypeType",
     "AttributeDataTypeType",
@@ -69,15 +68,14 @@
     "CognitoIdentityProviderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccountTakeoverEventActionTypeType = Literal[
     "BLOCK", "MFA_IF_CONFIGURED", "MFA_REQUIRED", "NO_ACTION"
 ]
 AdminListGroupsForUserPaginatorName = Literal["admin_list_groups_for_user"]
 AdminListUserAuthEventsPaginatorName = Literal["admin_list_user_auth_events"]
 AdvancedSecurityModeTypeType = Literal["AUDIT", "ENFORCED", "OFF"]
 AliasAttributeTypeType = Literal["email", "phone_number", "preferred_username"]
@@ -174,23 +172,25 @@
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
@@ -200,30 +200,35 @@
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
@@ -249,14 +254,15 @@
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
@@ -301,51 +307,57 @@
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
@@ -358,14 +370,15 @@
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
@@ -377,28 +390,35 @@
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
@@ -407,14 +427,15 @@
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
@@ -425,55 +446,64 @@
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
@@ -511,14 +541,15 @@
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/literals.pyi` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/literals.py`

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
     "AccountTakeoverEventActionTypeType",
     "AdminListGroupsForUserPaginatorName",
     "AdminListUserAuthEventsPaginatorName",
     "AdvancedSecurityModeTypeType",
     "AliasAttributeTypeType",
     "AttributeDataTypeType",
@@ -68,14 +69,15 @@
     "CognitoIdentityProviderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AccountTakeoverEventActionTypeType = Literal[
     "BLOCK", "MFA_IF_CONFIGURED", "MFA_REQUIRED", "NO_ACTION"
 ]
 AdminListGroupsForUserPaginatorName = Literal["admin_list_groups_for_user"]
 AdminListUserAuthEventsPaginatorName = Literal["admin_list_user_auth_events"]
 AdvancedSecurityModeTypeType = Literal["AUDIT", "ENFORCED", "OFF"]
 AliasAttributeTypeType = Literal["email", "phone_number", "preferred_username"]
@@ -172,23 +174,25 @@
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
@@ -198,30 +202,35 @@
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
@@ -247,14 +256,15 @@
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
@@ -299,51 +309,57 @@
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
@@ -356,14 +372,15 @@
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
@@ -375,28 +392,35 @@
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
@@ -405,14 +429,15 @@
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
@@ -423,55 +448,64 @@
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
@@ -509,14 +543,15 @@
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/paginator.py` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,156 +60,145 @@
     "ListResourceServersPaginator",
     "ListUserPoolClientsPaginator",
     "ListUserPoolsPaginator",
     "ListUsersPaginator",
     "ListUsersInGroupPaginator",
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
 class AdminListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Username: str, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
-
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, Username: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
-
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
-
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
-
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
-
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
-
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
-
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
     """
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
-
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/paginator.pyi` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,145 +60,156 @@
     "ListResourceServersPaginator",
     "ListUserPoolClientsPaginator",
     "ListUserPoolsPaginator",
     "ListUsersPaginator",
     "ListUsersInGroupPaginator",
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
 class AdminListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Username: str, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
+
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, Username: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
+
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
+
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
+
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
+
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
+
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
+
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
     """
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
+
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, UserPoolId: str, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/type_defs.py` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -60,67 +60,69 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
     "GroupTypeTypeDef",
+    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
     "ChallengeResponseTypeTypeDef",
     "EventContextDataTypeTypeDef",
     "EventFeedbackTypeTypeDef",
     "EventRiskTypeTypeDef",
     "NewDeviceMetadataTypeTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
+    "ConfirmDeviceResponseTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
     "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
@@ -137,88 +139,85 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
+    "GetCSVHeaderResponseTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
+    "GetSigningCertificateResponseTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
     "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ProviderDescriptionTypeDef",
+    "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
+    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
     "UserPoolClientDescriptionTypeDef",
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
+    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
+    "PaginatorConfigTypeDef",
     "PasswordPolicyTypeTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeTokenRequestRequestTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
-    "ConfirmDeviceResponseTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCSVHeaderResponseTypeDef",
-    "GetSigningCertificateResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
     "AdminGetUserResponseTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
     "UserTypeTypeDef",
-    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListResourceServersRequestListResourceServersPaginateTypeDef",
-    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "AdminListGroupsForUserResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
@@ -342,22 +341,20 @@
     "_OptionalAdminConfirmSignUpRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AdminConfirmSignUpRequestRequestTypeDef(
     _RequiredAdminConfirmSignUpRequestRequestTypeDef,
     _OptionalAdminConfirmSignUpRequestRequestTypeDef,
 ):
     pass
 
-
 MessageTemplateTypeTypeDef = TypedDict(
     "MessageTemplateTypeTypeDef",
     {
         "SMSMessage": str,
         "EmailMessage": str,
         "EmailSubject": str,
     },
@@ -374,30 +371,17 @@
     "_OptionalAttributeTypeTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeTypeDef(_RequiredAttributeTypeTypeDef, _OptionalAttributeTypeTypeDef):
     pass
 
-
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
 AdminDeleteUserAttributesRequestRequestTypeDef = TypedDict(
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributeNames": Sequence[str],
     },
@@ -492,31 +476,40 @@
     {
         "Limit": int,
         "PaginationToken": str,
     },
     total=False,
 )
 
-
 class AdminListDevicesRequestRequestTypeDef(
     _RequiredAdminListDevicesRequestRequestTypeDef, _OptionalAdminListDevicesRequestRequestTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Username": str,
+        "UserPoolId": str,
+    },
+)
+_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
+    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+):
+    pass
+
 _RequiredAdminListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestRequestTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
     },
 )
@@ -525,36 +518,55 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class AdminListGroupsForUserRequestRequestTypeDef(
     _RequiredAdminListGroupsForUserRequestRequestTypeDef,
     _OptionalAdminListGroupsForUserRequestRequestTypeDef,
 ):
     pass
 
-
 GroupTypeTypeDef = TypedDict(
     "GroupTypeTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
+_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+    },
+)
+_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
+    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+):
+    pass
+
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -563,22 +575,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class AdminListUserAuthEventsRequestRequestTypeDef(
     _RequiredAdminListUserAuthEventsRequestRequestTypeDef,
     _OptionalAdminListUserAuthEventsRequestRequestTypeDef,
 ):
     pass
 
-
 AdminRemoveUserFromGroupRequestRequestTypeDef = TypedDict(
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "GroupName": str,
     },
@@ -595,22 +605,20 @@
     "_OptionalAdminResetUserPasswordRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AdminResetUserPasswordRequestRequestTypeDef(
     _RequiredAdminResetUserPasswordRequestRequestTypeDef,
     _OptionalAdminResetUserPasswordRequestRequestTypeDef,
 ):
     pass
 
-
 SMSMfaSettingsTypeTypeDef = TypedDict(
     "SMSMfaSettingsTypeTypeDef",
     {
         "Enabled": bool,
         "PreferredMfa": bool,
     },
     total=False,
@@ -637,22 +645,20 @@
     "_OptionalAdminSetUserPasswordRequestRequestTypeDef",
     {
         "Permanent": bool,
     },
     total=False,
 )
 
-
 class AdminSetUserPasswordRequestRequestTypeDef(
     _RequiredAdminSetUserPasswordRequestRequestTypeDef,
     _OptionalAdminSetUserPasswordRequestRequestTypeDef,
 ):
     pass
 
-
 AdminUpdateAuthEventFeedbackRequestRequestTypeDef = TypedDict(
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "EventId": str,
         "FeedbackValue": FeedbackValueTypeType,
@@ -671,22 +677,20 @@
     "_OptionalAdminUpdateDeviceStatusRequestRequestTypeDef",
     {
         "DeviceRememberedStatus": DeviceRememberedStatusTypeType,
     },
     total=False,
 )
 
-
 class AdminUpdateDeviceStatusRequestRequestTypeDef(
     _RequiredAdminUpdateDeviceStatusRequestRequestTypeDef,
     _OptionalAdminUpdateDeviceStatusRequestRequestTypeDef,
 ):
     pass
 
-
 AdminUserGlobalSignOutRequestRequestTypeDef = TypedDict(
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -708,14 +712,23 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
+    {
+        "SecretCode": str,
+        "Session": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
     total=False,
@@ -744,21 +757,19 @@
     "_OptionalEventFeedbackTypeTypeDef",
     {
         "FeedbackDate": datetime,
     },
     total=False,
 )
 
-
 class EventFeedbackTypeTypeDef(
     _RequiredEventFeedbackTypeTypeDef, _OptionalEventFeedbackTypeTypeDef
 ):
     pass
 
-
 EventRiskTypeTypeDef = TypedDict(
     "EventRiskTypeTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
@@ -805,14 +816,22 @@
     {
         "PasswordVerifier": str,
         "Salt": str,
     },
     total=False,
 )
 
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
+    {
+        "UserConfirmationNecessary": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UserContextDataTypeTypeDef = TypedDict(
     "UserContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "EncodedData": str,
     },
     total=False,
@@ -840,21 +859,19 @@
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Mapping[str, str],
@@ -865,22 +882,20 @@
     {
         "AttributeMapping": Mapping[str, str],
         "IdpIdentifiers": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 IdentityProviderTypeTypeDef = TypedDict(
     "IdentityProviderTypeTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
@@ -942,14 +957,22 @@
 CustomDomainConfigTypeTypeDef = TypedDict(
     "CustomDomainConfigTypeTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceConfigurationTypeTypeDef = TypedDict(
     "DeviceConfigurationTypeTypeDef",
     {
         "ChallengeRequiredOnNewDevice": bool,
         "DeviceOnlyRememberedOnUserPrompt": bool,
     },
     total=False,
@@ -978,21 +1001,19 @@
     {
         "ExternalId": str,
         "SnsRegion": str,
     },
     total=False,
 )
 
-
 class SmsConfigurationTypeTypeDef(
     _RequiredSmsConfigurationTypeTypeDef, _OptionalSmsConfigurationTypeTypeDef
 ):
     pass
 
-
 UserAttributeUpdateSettingsTypeTypeDef = TypedDict(
     "UserAttributeUpdateSettingsTypeTypeDef",
     {
         "AttributesRequireVerificationBeforeUpdate": Sequence[VerifiedAttributeTypeType],
     },
     total=False,
 )
@@ -1128,22 +1149,20 @@
     "_OptionalDescribeRiskConfigurationRequestRequestTypeDef",
     {
         "ClientId": str,
     },
     total=False,
 )
 
-
 class DescribeRiskConfigurationRequestRequestTypeDef(
     _RequiredDescribeRiskConfigurationRequestRequestTypeDef,
     _OptionalDescribeRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeUserImportJobRequestRequestTypeDef = TypedDict(
     "DescribeUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1166,63 +1185,75 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalForgetDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
     total=False,
 )
 
-
 class ForgetDeviceRequestRequestTypeDef(
     _RequiredForgetDeviceRequestRequestTypeDef, _OptionalForgetDeviceRequestRequestTypeDef
 ):
     pass
 
-
 GetCSVHeaderRequestRequestTypeDef = TypedDict(
     "GetCSVHeaderRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
+    {
+        "UserPoolId": str,
+        "CSVHeader": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalGetDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalGetDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
     total=False,
 )
 
-
 class GetDeviceRequestRequestTypeDef(
     _RequiredGetDeviceRequestRequestTypeDef, _OptionalGetDeviceRequestRequestTypeDef
 ):
     pass
 
-
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
     },
 )
@@ -1238,36 +1269,42 @@
 GetSigningCertificateRequestRequestTypeDef = TypedDict(
     "GetSigningCertificateRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
+    {
+        "Certificate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetUICustomizationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_OptionalGetUICustomizationRequestRequestTypeDef",
     {
         "ClientId": str,
     },
     total=False,
 )
 
-
 class GetUICustomizationRequestRequestTypeDef(
     _RequiredGetUICustomizationRequestRequestTypeDef,
     _OptionalGetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
-
 UICustomizationTypeTypeDef = TypedDict(
     "UICustomizationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
@@ -1289,22 +1326,20 @@
     "_OptionalGetUserAttributeVerificationCodeRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetUserAttributeVerificationCodeRequestRequestTypeDef(
     _RequiredGetUserAttributeVerificationCodeRequestRequestTypeDef,
     _OptionalGetUserAttributeVerificationCodeRequestRequestTypeDef,
 ):
     pass
 
-
 GetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
@@ -1341,20 +1376,38 @@
     {
         "Limit": int,
         "PaginationToken": str,
     },
     total=False,
 )
 
-
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
 
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
@@ -1363,20 +1416,38 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
+    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+):
+    pass
 
 _RequiredListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProvidersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
@@ -1385,33 +1456,51 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
-
 ProviderDescriptionTypeDef = TypedDict(
     "ProviderDescriptionTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
+_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListResourceServersRequestListResourceServersPaginateTypeDef(
+    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
+    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
+):
+    pass
+
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListResourceServersRequestRequestTypeDef = TypedDict(
@@ -1419,29 +1508,35 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceServersRequestRequestTypeDef(
     _RequiredListResourceServersRequestRequestTypeDef,
     _OptionalListResourceServersRequestRequestTypeDef,
 ):
     pass
 
-
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
 _RequiredListUserImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserImportJobsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "MaxResults": int,
     },
 )
@@ -1449,21 +1544,39 @@
     "_OptionalListUserImportJobsRequestRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
-
 class ListUserImportJobsRequestRequestTypeDef(
     _RequiredListUserImportJobsRequestRequestTypeDef,
     _OptionalListUserImportJobsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
+    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+):
+    pass
 
 _RequiredListUserPoolClientsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolClientsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
@@ -1472,52 +1585,77 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListUserPoolClientsRequestRequestTypeDef(
     _RequiredListUserPoolClientsRequestRequestTypeDef,
     _OptionalListUserPoolClientsRequestRequestTypeDef,
 ):
     pass
 
-
 UserPoolClientDescriptionTypeDef = TypedDict(
     "UserPoolClientDescriptionTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
     total=False,
 )
 
+ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListUserPoolsRequestRequestTypeDef = TypedDict(
     "_OptionalListUserPoolsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListUserPoolsRequestRequestTypeDef(
     _RequiredListUserPoolsRequestRequestTypeDef, _OptionalListUserPoolsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "GroupName": str,
+    },
+)
+_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
+    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+):
+    pass
 
 _RequiredListUsersInGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersInGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "GroupName": str,
     },
@@ -1527,20 +1665,40 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListUsersInGroupRequestRequestTypeDef(
     _RequiredListUsersInGroupRequestRequestTypeDef, _OptionalListUsersInGroupRequestRequestTypeDef
 ):
     pass
 
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AttributesToGet": Sequence[str],
+        "Filter": str,
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
 
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
@@ -1551,21 +1709,19 @@
         "Limit": int,
         "PaginationToken": str,
         "Filter": str,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredNotifyEmailTypeTypeDef = TypedDict(
     "_RequiredNotifyEmailTypeTypeDef",
     {
         "Subject": str,
     },
 )
 _OptionalNotifyEmailTypeTypeDef = TypedDict(
@@ -1573,41 +1729,60 @@
     {
         "HtmlBody": str,
         "TextBody": str,
     },
     total=False,
 )
 
-
 class NotifyEmailTypeTypeDef(_RequiredNotifyEmailTypeTypeDef, _OptionalNotifyEmailTypeTypeDef):
     pass
 
-
 NumberAttributeConstraintsTypeTypeDef = TypedDict(
     "NumberAttributeConstraintsTypeTypeDef",
     {
         "MinValue": str,
         "MaxValue": str,
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
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
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
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1615,21 +1790,19 @@
     "_OptionalRevokeTokenRequestRequestTypeDef",
     {
         "ClientSecret": str,
     },
     total=False,
 )
 
-
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
-
 RiskExceptionConfigurationTypeTypeDef = TypedDict(
     "RiskExceptionConfigurationTypeTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
     total=False,
@@ -1656,22 +1829,20 @@
         "ClientId": str,
         "CSS": str,
         "ImageFile": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class SetUICustomizationRequestRequestTypeDef(
     _RequiredSetUICustomizationRequestRequestTypeDef,
     _OptionalSetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
-
 StartUserImportJobRequestRequestTypeDef = TypedDict(
     "StartUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1722,22 +1893,20 @@
     "_OptionalUpdateDeviceStatusRequestRequestTypeDef",
     {
         "DeviceRememberedStatus": DeviceRememberedStatusTypeType,
     },
     total=False,
 )
 
-
 class UpdateDeviceStatusRequestRequestTypeDef(
     _RequiredUpdateDeviceStatusRequestRequestTypeDef,
     _OptionalUpdateDeviceStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
     },
 )
@@ -1747,21 +1916,19 @@
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
     },
     total=False,
 )
 
-
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
     },
 )
@@ -1771,21 +1938,27 @@
         "ProviderDetails": Mapping[str, str],
         "AttributeMapping": Mapping[str, str],
         "IdpIdentifiers": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
@@ -1795,21 +1968,28 @@
         "AccessToken": str,
         "Session": str,
         "FriendlyDeviceName": str,
     },
     total=False,
 )
 
-
 class VerifySoftwareTokenRequestRequestTypeDef(
     _RequiredVerifySoftwareTokenRequestRequestTypeDef,
     _OptionalVerifySoftwareTokenRequestRequestTypeDef,
 ):
     pass
 
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
+    {
+        "Status": VerifySoftwareTokenResponseTypeType,
+        "Session": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 VerifyUserAttributeRequestRequestTypeDef = TypedDict(
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
@@ -1861,21 +2041,19 @@
         "MessageAction": MessageActionTypeType,
         "DesiredDeliveryMediums": Sequence[DeliveryMediumTypeType],
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AdminCreateUserRequestRequestTypeDef(
     _RequiredAdminCreateUserRequestRequestTypeDef, _OptionalAdminCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAdminUpdateUserAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredAdminUpdateUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributes": Sequence[AttributeTypeTypeDef],
     },
@@ -1884,22 +2062,20 @@
     "_OptionalAdminUpdateUserAttributesRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AdminUpdateUserAttributesRequestRequestTypeDef(
     _RequiredAdminUpdateUserAttributesRequestRequestTypeDef,
     _OptionalAdminUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 DeviceTypeTypeDef = TypedDict(
     "DeviceTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceAttributes": List[AttributeTypeTypeDef],
         "DeviceCreateDate": datetime,
         "DeviceLastModifiedDate": datetime,
@@ -1919,96 +2095,20 @@
     "_OptionalUpdateUserAttributesRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
-
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
-    {
-        "SecretCode": str,
-        "Session": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
-    {
-        "UserConfirmationNecessary": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
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
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
-    {
-        "UserPoolId": str,
-        "CSVHeader": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
-    {
-        "Certificate": str,
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
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
-    {
-        "Status": VerifySoftwareTokenResponseTypeType,
-        "Session": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AdminDisableProviderForUserRequestRequestTypeDef = TypedDict(
     "AdminDisableProviderForUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "User": ProviderUserIdentifierTypeTypeDef,
     },
 )
@@ -2030,15 +2130,15 @@
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
     "AdminSetUserSettingsRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2051,15 +2151,15 @@
     "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeTypeDef],
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetUserSettingsRequestRequestTypeDef = TypedDict(
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
@@ -2077,242 +2177,53 @@
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
     total=False,
 )
 
-_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "Username": str,
-        "UserPoolId": str,
-    },
-)
-_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
-    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-):
-    pass
-
-
-_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-    },
-)
-_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
-    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
-    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResourceServersRequestListResourceServersPaginateTypeDef(
-    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
-    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
-    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-):
-    pass
-
-
-ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "GroupName": str,
-    },
-)
-_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
-    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "Filter": str,
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
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "Username": str,
@@ -2324,22 +2235,20 @@
     {
         "SMSMfaSettings": SMSMfaSettingsTypeTypeDef,
         "SoftwareTokenMfaSettings": SoftwareTokenMfaSettingsTypeTypeDef,
     },
     total=False,
 )
 
-
 class AdminSetUserMFAPreferenceRequestRequestTypeDef(
     _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef,
     _OptionalAdminSetUserMFAPreferenceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
 )
 _OptionalSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
@@ -2347,22 +2256,20 @@
     {
         "SMSMfaSettings": SMSMfaSettingsTypeTypeDef,
         "SoftwareTokenMfaSettings": SoftwareTokenMfaSettingsTypeTypeDef,
     },
     total=False,
 )
 
-
 class SetUserMFAPreferenceRequestRequestTypeDef(
     _RequiredSetUserMFAPreferenceRequestRequestTypeDef,
     _OptionalSetUserMFAPreferenceRequestRequestTypeDef,
 ):
     pass
 
-
 AuthEventTypeTypeDef = TypedDict(
     "AuthEventTypeTypeDef",
     {
         "EventId": str,
         "EventType": EventTypeType,
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
@@ -2387,49 +2294,49 @@
     total=False,
 )
 
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
     "GetUserAttributeVerificationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResendConfirmationCodeResponseTypeDef = TypedDict(
     "ResendConfirmationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SignUpResponseTypeDef = TypedDict(
     "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
@@ -2439,22 +2346,20 @@
     "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "EventFilter": List[EventFilterTypeType],
     },
     total=False,
 )
 
-
 class CompromisedCredentialsRiskConfigurationTypeTypeDef(
     _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
     _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
 ):
     pass
 
-
 _RequiredConfirmDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
     },
 )
@@ -2463,21 +2368,19 @@
     {
         "DeviceSecretVerifierConfig": DeviceSecretVerifierConfigTypeTypeDef,
         "DeviceName": str,
     },
     total=False,
 )
 
-
 class ConfirmDeviceRequestRequestTypeDef(
     _RequiredConfirmDeviceRequestRequestTypeDef, _OptionalConfirmDeviceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredConfirmForgotPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmForgotPasswordRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
         "ConfirmationCode": str,
         "Password": str,
@@ -2490,22 +2393,20 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ConfirmForgotPasswordRequestRequestTypeDef(
     _RequiredConfirmForgotPasswordRequestRequestTypeDef,
     _OptionalConfirmForgotPasswordRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredConfirmSignUpRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmSignUpRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
         "ConfirmationCode": str,
     },
@@ -2518,21 +2419,19 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ConfirmSignUpRequestRequestTypeDef(
     _RequiredConfirmSignUpRequestRequestTypeDef, _OptionalConfirmSignUpRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredForgotPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredForgotPasswordRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
     },
 )
@@ -2543,21 +2442,19 @@
         "UserContextData": UserContextDataTypeTypeDef,
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ForgotPasswordRequestRequestTypeDef(
     _RequiredForgotPasswordRequestRequestTypeDef, _OptionalForgotPasswordRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredInitiateAuthRequestRequestTypeDef",
     {
         "AuthFlow": AuthFlowTypeType,
         "ClientId": str,
     },
 )
@@ -2568,21 +2465,19 @@
         "ClientMetadata": Mapping[str, str],
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
     },
     total=False,
 )
 
-
 class InitiateAuthRequestRequestTypeDef(
     _RequiredInitiateAuthRequestRequestTypeDef, _OptionalInitiateAuthRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredResendConfirmationCodeRequestRequestTypeDef = TypedDict(
     "_RequiredResendConfirmationCodeRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
     },
 )
@@ -2593,22 +2488,20 @@
         "UserContextData": UserContextDataTypeTypeDef,
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ResendConfirmationCodeRequestRequestTypeDef(
     _RequiredResendConfirmationCodeRequestRequestTypeDef,
     _OptionalResendConfirmationCodeRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRespondToAuthChallengeRequestRequestTypeDef = TypedDict(
     "_RequiredRespondToAuthChallengeRequestRequestTypeDef",
     {
         "ClientId": str,
         "ChallengeName": ChallengeNameTypeType,
     },
 )
@@ -2620,22 +2513,20 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RespondToAuthChallengeRequestRequestTypeDef(
     _RequiredRespondToAuthChallengeRequestRequestTypeDef,
     _OptionalRespondToAuthChallengeRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSignUpRequestRequestTypeDef = TypedDict(
     "_RequiredSignUpRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
         "Password": str,
     },
@@ -2649,21 +2540,19 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class SignUpRequestRequestTypeDef(
     _RequiredSignUpRequestRequestTypeDef, _OptionalSignUpRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredContextDataTypeTypeDef = TypedDict(
     "_RequiredContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "ServerName": str,
         "ServerPath": str,
         "HttpHeaders": Sequence[HttpHeaderTypeDef],
@@ -2673,48 +2562,46 @@
     "_OptionalContextDataTypeTypeDef",
     {
         "EncodedData": str,
     },
     total=False,
 )
 
-
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
-
 CreateIdentityProviderResponseTypeDef = TypedDict(
     "CreateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIdentityProviderResponseTypeDef = TypedDict(
     "DescribeIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
     "GetIdentityProviderByIdentifierResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2726,22 +2613,20 @@
     "_OptionalCreateResourceServerRequestRequestTypeDef",
     {
         "Scopes": Sequence[ResourceServerScopeTypeTypeDef],
     },
     total=False,
 )
 
-
 class CreateResourceServerRequestRequestTypeDef(
     _RequiredCreateResourceServerRequestRequestTypeDef,
     _OptionalCreateResourceServerRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceServerTypeTypeDef = TypedDict(
     "ResourceServerTypeTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
         "Scopes": List[ResourceServerScopeTypeTypeDef],
@@ -2761,60 +2646,58 @@
     "_OptionalUpdateResourceServerRequestRequestTypeDef",
     {
         "Scopes": Sequence[ResourceServerScopeTypeTypeDef],
     },
     total=False,
 )
 
-
 class UpdateResourceServerRequestRequestTypeDef(
     _RequiredUpdateResourceServerRequestRequestTypeDef,
     _OptionalUpdateResourceServerRequestRequestTypeDef,
 ):
     pass
 
-
 CreateUserImportJobResponseTypeDef = TypedDict(
     "CreateUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserImportJobResponseTypeDef = TypedDict(
     "DescribeUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserImportJobsResponseTypeDef = TypedDict(
     "ListUserImportJobsResponseTypeDef",
     {
         "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartUserImportJobResponseTypeDef = TypedDict(
     "StartUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopUserImportJobResponseTypeDef = TypedDict(
     "StopUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2844,22 +2727,20 @@
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
     total=False,
 )
 
-
 class CreateUserPoolClientRequestRequestTypeDef(
     _RequiredCreateUserPoolClientRequestRequestTypeDef,
     _OptionalCreateUserPoolClientRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
     },
 )
@@ -2886,22 +2767,20 @@
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
     total=False,
 )
 
-
 class UpdateUserPoolClientRequestRequestTypeDef(
     _RequiredUpdateUserPoolClientRequestRequestTypeDef,
     _OptionalUpdateUserPoolClientRequestRequestTypeDef,
 ):
     pass
 
-
 UserPoolClientTypeTypeDef = TypedDict(
     "UserPoolClientTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientName": str,
         "ClientId": str,
         "ClientSecret": str,
@@ -2941,22 +2820,20 @@
     "_OptionalCreateUserPoolDomainRequestRequestTypeDef",
     {
         "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
     },
     total=False,
 )
 
-
 class CreateUserPoolDomainRequestRequestTypeDef(
     _RequiredCreateUserPoolDomainRequestRequestTypeDef,
     _OptionalCreateUserPoolDomainRequestRequestTypeDef,
 ):
     pass
 
-
 DomainDescriptionTypeTypeDef = TypedDict(
     "DomainDescriptionTypeTypeDef",
     {
         "UserPoolId": str,
         "AWSAccountId": str,
         "Domain": str,
         "S3Bucket": str,
@@ -3006,41 +2883,41 @@
     total=False,
 )
 
 GetUICustomizationResponseTypeDef = TypedDict(
     "GetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetUICustomizationResponseTypeDef = TypedDict(
     "SetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNotifyConfigurationTypeTypeDef = TypedDict(
     "_RequiredNotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
@@ -3054,21 +2931,19 @@
         "BlockEmail": NotifyEmailTypeTypeDef,
         "NoActionEmail": NotifyEmailTypeTypeDef,
         "MfaEmail": NotifyEmailTypeTypeDef,
     },
     total=False,
 )
 
-
 class NotifyConfigurationTypeTypeDef(
     _RequiredNotifyConfigurationTypeTypeDef, _OptionalNotifyConfigurationTypeTypeDef
 ):
     pass
 
-
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
@@ -3087,120 +2962,120 @@
     total=False,
 )
 
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminListDevicesResponseTypeDef = TypedDict(
     "AdminListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeviceResponseTypeDef = TypedDict(
     "GetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminCreateUserResponseTypeDef = TypedDict(
     "AdminCreateUserResponseTypeDef",
     {
         "User": UserTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
     "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InitiateAuthResponseTypeDef = TypedDict(
     "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RespondToAuthChallengeResponseTypeDef = TypedDict(
     "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3215,21 +3090,19 @@
         "ClientMetadata": Mapping[str, str],
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ContextData": ContextDataTypeTypeDef,
     },
     total=False,
 )
 
-
 class AdminInitiateAuthRequestRequestTypeDef(
     _RequiredAdminInitiateAuthRequestRequestTypeDef, _OptionalAdminInitiateAuthRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAdminRespondToAuthChallengeRequestRequestTypeDef = TypedDict(
     "_RequiredAdminRespondToAuthChallengeRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ChallengeName": ChallengeNameTypeType,
     },
@@ -3242,94 +3115,92 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ContextData": ContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AdminRespondToAuthChallengeRequestRequestTypeDef(
     _RequiredAdminRespondToAuthChallengeRequestRequestTypeDef,
     _OptionalAdminRespondToAuthChallengeRequestRequestTypeDef,
 ):
     pass
 
-
 CreateResourceServerResponseTypeDef = TypedDict(
     "CreateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourceServerResponseTypeDef = TypedDict(
     "DescribeResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUserPoolClientResponseTypeDef = TypedDict(
     "CreateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserPoolClientResponseTypeDef = TypedDict(
     "DescribeUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserPoolClientResponseTypeDef = TypedDict(
     "UpdateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserPoolDomainResponseTypeDef = TypedDict(
     "DescribeUserPoolDomainResponseTypeDef",
     {
         "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3341,29 +3212,27 @@
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
     },
     total=False,
 )
 
-
 class SetUserPoolMfaConfigRequestRequestTypeDef(
     _RequiredSetUserPoolMfaConfigRequestRequestTypeDef,
     _OptionalSetUserPoolMfaConfigRequestRequestTypeDef,
 ):
     pass
 
-
 SetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserPoolDescriptionTypeTypeDef = TypedDict(
     "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
@@ -3386,22 +3255,20 @@
     "_OptionalAccountTakeoverRiskConfigurationTypeTypeDef",
     {
         "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class AccountTakeoverRiskConfigurationTypeTypeDef(
     _RequiredAccountTakeoverRiskConfigurationTypeTypeDef,
     _OptionalAccountTakeoverRiskConfigurationTypeTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserPoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalUpdateUserPoolRequestRequestTypeDef = TypedDict(
@@ -3425,21 +3292,19 @@
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
     total=False,
 )
 
-
 class UpdateUserPoolRequestRequestTypeDef(
     _RequiredUpdateUserPoolRequestRequestTypeDef, _OptionalUpdateUserPoolRequestRequestTypeDef
 ):
     pass
 
-
 AddCustomAttributesRequestRequestTypeDef = TypedDict(
     "AddCustomAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "CustomAttributes": Sequence[SchemaAttributeTypeTypeDef],
     },
 )
@@ -3475,21 +3340,19 @@
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
     total=False,
 )
 
-
 class CreateUserPoolRequestRequestTypeDef(
     _RequiredCreateUserPoolRequestRequestTypeDef, _OptionalCreateUserPoolRequestRequestTypeDef
 ):
     pass
 
-
 UserPoolTypeTypeDef = TypedDict(
     "UserPoolTypeTypeDef",
     {
         "Id": str,
         "Name": str,
         "Policies": UserPoolPolicyTypeTypeDef,
         "DeletionProtection": DeletionProtectionTypeType,
@@ -3527,24 +3390,26 @@
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
-        "CompromisedCredentialsRiskConfiguration": CompromisedCredentialsRiskConfigurationTypeTypeDef,
+        "CompromisedCredentialsRiskConfiguration": (
+            CompromisedCredentialsRiskConfigurationTypeTypeDef
+        ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
         "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
         "LastModifiedDate": datetime,
     },
     total=False,
 )
 
@@ -3554,53 +3419,53 @@
         "UserPoolId": str,
     },
 )
 _OptionalSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalSetRiskConfigurationRequestRequestTypeDef",
     {
         "ClientId": str,
-        "CompromisedCredentialsRiskConfiguration": CompromisedCredentialsRiskConfigurationTypeTypeDef,
+        "CompromisedCredentialsRiskConfiguration": (
+            CompromisedCredentialsRiskConfigurationTypeTypeDef
+        ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
         "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class SetRiskConfigurationRequestRequestTypeDef(
     _RequiredSetRiskConfigurationRequestRequestTypeDef,
     _OptionalSetRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 CreateUserPoolResponseTypeDef = TypedDict(
     "CreateUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserPoolResponseTypeDef = TypedDict(
     "DescribeUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRiskConfigurationResponseTypeDef = TypedDict(
     "DescribeRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetRiskConfigurationResponseTypeDef = TypedDict(
     "SetRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -60,66 +60,70 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
     "GroupTypeTypeDef",
+    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
     "ChallengeResponseTypeTypeDef",
     "EventContextDataTypeTypeDef",
     "EventFeedbackTypeTypeDef",
     "EventRiskTypeTypeDef",
     "NewDeviceMetadataTypeTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
+    "ConfirmDeviceResponseTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
     "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
@@ -136,88 +140,85 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
+    "GetCSVHeaderResponseTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
+    "GetSigningCertificateResponseTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
     "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ProviderDescriptionTypeDef",
+    "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
+    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
     "UserPoolClientDescriptionTypeDef",
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
+    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
+    "PaginatorConfigTypeDef",
     "PasswordPolicyTypeTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeTokenRequestRequestTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
-    "ConfirmDeviceResponseTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCSVHeaderResponseTypeDef",
-    "GetSigningCertificateResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
     "AdminGetUserResponseTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
     "UserTypeTypeDef",
-    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListResourceServersRequestListResourceServersPaginateTypeDef",
-    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "AdminListGroupsForUserResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
@@ -341,20 +342,22 @@
     "_OptionalAdminConfirmSignUpRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AdminConfirmSignUpRequestRequestTypeDef(
     _RequiredAdminConfirmSignUpRequestRequestTypeDef,
     _OptionalAdminConfirmSignUpRequestRequestTypeDef,
 ):
     pass
 
+
 MessageTemplateTypeTypeDef = TypedDict(
     "MessageTemplateTypeTypeDef",
     {
         "SMSMessage": str,
         "EmailMessage": str,
         "EmailSubject": str,
     },
@@ -371,27 +374,18 @@
     "_OptionalAttributeTypeTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeTypeDef(_RequiredAttributeTypeTypeDef, _OptionalAttributeTypeTypeDef):
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
 
 AdminDeleteUserAttributesRequestRequestTypeDef = TypedDict(
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributeNames": Sequence[str],
@@ -487,29 +481,44 @@
     {
         "Limit": int,
         "PaginationToken": str,
     },
     total=False,
 )
 
+
 class AdminListDevicesRequestRequestTypeDef(
     _RequiredAdminListDevicesRequestRequestTypeDef, _OptionalAdminListDevicesRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Username": str,
+        "UserPoolId": str,
+    },
+)
+_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
+    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+
 _RequiredAdminListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestRequestTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
     },
 )
@@ -518,34 +527,59 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class AdminListGroupsForUserRequestRequestTypeDef(
     _RequiredAdminListGroupsForUserRequestRequestTypeDef,
     _OptionalAdminListGroupsForUserRequestRequestTypeDef,
 ):
     pass
 
+
 GroupTypeTypeDef = TypedDict(
     "GroupTypeTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
+_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+    },
+)
+_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
+    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -554,20 +588,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class AdminListUserAuthEventsRequestRequestTypeDef(
     _RequiredAdminListUserAuthEventsRequestRequestTypeDef,
     _OptionalAdminListUserAuthEventsRequestRequestTypeDef,
 ):
     pass
 
+
 AdminRemoveUserFromGroupRequestRequestTypeDef = TypedDict(
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "GroupName": str,
     },
@@ -584,20 +620,22 @@
     "_OptionalAdminResetUserPasswordRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AdminResetUserPasswordRequestRequestTypeDef(
     _RequiredAdminResetUserPasswordRequestRequestTypeDef,
     _OptionalAdminResetUserPasswordRequestRequestTypeDef,
 ):
     pass
 
+
 SMSMfaSettingsTypeTypeDef = TypedDict(
     "SMSMfaSettingsTypeTypeDef",
     {
         "Enabled": bool,
         "PreferredMfa": bool,
     },
     total=False,
@@ -624,20 +662,22 @@
     "_OptionalAdminSetUserPasswordRequestRequestTypeDef",
     {
         "Permanent": bool,
     },
     total=False,
 )
 
+
 class AdminSetUserPasswordRequestRequestTypeDef(
     _RequiredAdminSetUserPasswordRequestRequestTypeDef,
     _OptionalAdminSetUserPasswordRequestRequestTypeDef,
 ):
     pass
 
+
 AdminUpdateAuthEventFeedbackRequestRequestTypeDef = TypedDict(
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "EventId": str,
         "FeedbackValue": FeedbackValueTypeType,
@@ -656,20 +696,22 @@
     "_OptionalAdminUpdateDeviceStatusRequestRequestTypeDef",
     {
         "DeviceRememberedStatus": DeviceRememberedStatusTypeType,
     },
     total=False,
 )
 
+
 class AdminUpdateDeviceStatusRequestRequestTypeDef(
     _RequiredAdminUpdateDeviceStatusRequestRequestTypeDef,
     _OptionalAdminUpdateDeviceStatusRequestRequestTypeDef,
 ):
     pass
 
+
 AdminUserGlobalSignOutRequestRequestTypeDef = TypedDict(
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -691,14 +733,23 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
+    {
+        "SecretCode": str,
+        "Session": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
     total=False,
@@ -727,19 +778,21 @@
     "_OptionalEventFeedbackTypeTypeDef",
     {
         "FeedbackDate": datetime,
     },
     total=False,
 )
 
+
 class EventFeedbackTypeTypeDef(
     _RequiredEventFeedbackTypeTypeDef, _OptionalEventFeedbackTypeTypeDef
 ):
     pass
 
+
 EventRiskTypeTypeDef = TypedDict(
     "EventRiskTypeTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
@@ -786,14 +839,22 @@
     {
         "PasswordVerifier": str,
         "Salt": str,
     },
     total=False,
 )
 
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
+    {
+        "UserConfirmationNecessary": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UserContextDataTypeTypeDef = TypedDict(
     "UserContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "EncodedData": str,
     },
     total=False,
@@ -821,19 +882,21 @@
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Mapping[str, str],
@@ -844,20 +907,22 @@
     {
         "AttributeMapping": Mapping[str, str],
         "IdpIdentifiers": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 IdentityProviderTypeTypeDef = TypedDict(
     "IdentityProviderTypeTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
@@ -919,14 +984,22 @@
 CustomDomainConfigTypeTypeDef = TypedDict(
     "CustomDomainConfigTypeTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceConfigurationTypeTypeDef = TypedDict(
     "DeviceConfigurationTypeTypeDef",
     {
         "ChallengeRequiredOnNewDevice": bool,
         "DeviceOnlyRememberedOnUserPrompt": bool,
     },
     total=False,
@@ -955,19 +1028,21 @@
     {
         "ExternalId": str,
         "SnsRegion": str,
     },
     total=False,
 )
 
+
 class SmsConfigurationTypeTypeDef(
     _RequiredSmsConfigurationTypeTypeDef, _OptionalSmsConfigurationTypeTypeDef
 ):
     pass
 
+
 UserAttributeUpdateSettingsTypeTypeDef = TypedDict(
     "UserAttributeUpdateSettingsTypeTypeDef",
     {
         "AttributesRequireVerificationBeforeUpdate": Sequence[VerifiedAttributeTypeType],
     },
     total=False,
 )
@@ -1103,20 +1178,22 @@
     "_OptionalDescribeRiskConfigurationRequestRequestTypeDef",
     {
         "ClientId": str,
     },
     total=False,
 )
 
+
 class DescribeRiskConfigurationRequestRequestTypeDef(
     _RequiredDescribeRiskConfigurationRequestRequestTypeDef,
     _OptionalDescribeRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeUserImportJobRequestRequestTypeDef = TypedDict(
     "DescribeUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1139,59 +1216,79 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalForgetDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
     total=False,
 )
 
+
 class ForgetDeviceRequestRequestTypeDef(
     _RequiredForgetDeviceRequestRequestTypeDef, _OptionalForgetDeviceRequestRequestTypeDef
 ):
     pass
 
+
 GetCSVHeaderRequestRequestTypeDef = TypedDict(
     "GetCSVHeaderRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
+    {
+        "UserPoolId": str,
+        "CSVHeader": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalGetDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalGetDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
     total=False,
 )
 
+
 class GetDeviceRequestRequestTypeDef(
     _RequiredGetDeviceRequestRequestTypeDef, _OptionalGetDeviceRequestRequestTypeDef
 ):
     pass
 
+
 GetGroupRequestRequestTypeDef = TypedDict(
     "GetGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
     },
 )
@@ -1207,34 +1304,44 @@
 GetSigningCertificateRequestRequestTypeDef = TypedDict(
     "GetSigningCertificateRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
+    {
+        "Certificate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetUICustomizationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_OptionalGetUICustomizationRequestRequestTypeDef",
     {
         "ClientId": str,
     },
     total=False,
 )
 
+
 class GetUICustomizationRequestRequestTypeDef(
     _RequiredGetUICustomizationRequestRequestTypeDef,
     _OptionalGetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
+
 UICustomizationTypeTypeDef = TypedDict(
     "UICustomizationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
@@ -1256,20 +1363,22 @@
     "_OptionalGetUserAttributeVerificationCodeRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetUserAttributeVerificationCodeRequestRequestTypeDef(
     _RequiredGetUserAttributeVerificationCodeRequestRequestTypeDef,
     _OptionalGetUserAttributeVerificationCodeRequestRequestTypeDef,
 ):
     pass
 
+
 GetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
@@ -1306,19 +1415,43 @@
     {
         "Limit": int,
         "PaginationToken": str,
     },
     total=False,
 )
 
+
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1326,19 +1459,43 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
+    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProvidersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListIdentityProvidersRequestRequestTypeDef = TypedDict(
@@ -1346,31 +1503,55 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
+
 ProviderDescriptionTypeDef = TypedDict(
     "ProviderDescriptionTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
+_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListResourceServersRequestListResourceServersPaginateTypeDef(
+    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
+    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListResourceServersRequestRequestTypeDef = TypedDict(
@@ -1378,27 +1559,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceServersRequestRequestTypeDef(
     _RequiredListResourceServersRequestRequestTypeDef,
     _OptionalListResourceServersRequestRequestTypeDef,
 ):
     pass
 
+
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
 _RequiredListUserImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserImportJobsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "MaxResults": int,
     },
 )
@@ -1406,20 +1597,44 @@
     "_OptionalListUserImportJobsRequestRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
+
 class ListUserImportJobsRequestRequestTypeDef(
     _RequiredListUserImportJobsRequestRequestTypeDef,
     _OptionalListUserImportJobsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
+    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListUserPoolClientsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolClientsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUserPoolClientsRequestRequestTypeDef = TypedDict(
@@ -1427,49 +1642,84 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListUserPoolClientsRequestRequestTypeDef(
     _RequiredListUserPoolClientsRequestRequestTypeDef,
     _OptionalListUserPoolClientsRequestRequestTypeDef,
 ):
     pass
 
+
 UserPoolClientDescriptionTypeDef = TypedDict(
     "UserPoolClientDescriptionTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
     total=False,
 )
 
+ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListUserPoolsRequestRequestTypeDef = TypedDict(
     "_OptionalListUserPoolsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListUserPoolsRequestRequestTypeDef(
     _RequiredListUserPoolsRequestRequestTypeDef, _OptionalListUserPoolsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "GroupName": str,
+    },
+)
+_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
+    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListUsersInGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersInGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "GroupName": str,
     },
 )
@@ -1478,19 +1728,45 @@
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListUsersInGroupRequestRequestTypeDef(
     _RequiredListUsersInGroupRequestRequestTypeDef, _OptionalListUsersInGroupRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AttributesToGet": Sequence[str],
+        "Filter": str,
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
         "UserPoolId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1500,19 +1776,21 @@
         "Limit": int,
         "PaginationToken": str,
         "Filter": str,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredNotifyEmailTypeTypeDef = TypedDict(
     "_RequiredNotifyEmailTypeTypeDef",
     {
         "Subject": str,
     },
 )
 _OptionalNotifyEmailTypeTypeDef = TypedDict(
@@ -1520,39 +1798,62 @@
     {
         "HtmlBody": str,
         "TextBody": str,
     },
     total=False,
 )
 
+
 class NotifyEmailTypeTypeDef(_RequiredNotifyEmailTypeTypeDef, _OptionalNotifyEmailTypeTypeDef):
     pass
 
+
 NumberAttributeConstraintsTypeTypeDef = TypedDict(
     "NumberAttributeConstraintsTypeTypeDef",
     {
         "MinValue": str,
         "MaxValue": str,
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
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
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
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1560,19 +1861,21 @@
     "_OptionalRevokeTokenRequestRequestTypeDef",
     {
         "ClientSecret": str,
     },
     total=False,
 )
 
+
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
+
 RiskExceptionConfigurationTypeTypeDef = TypedDict(
     "RiskExceptionConfigurationTypeTypeDef",
     {
         "BlockedIPRangeList": List[str],
         "SkippedIPRangeList": List[str],
     },
     total=False,
@@ -1599,20 +1902,22 @@
         "ClientId": str,
         "CSS": str,
         "ImageFile": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class SetUICustomizationRequestRequestTypeDef(
     _RequiredSetUICustomizationRequestRequestTypeDef,
     _OptionalSetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
+
 StartUserImportJobRequestRequestTypeDef = TypedDict(
     "StartUserImportJobRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "JobId": str,
     },
 )
@@ -1663,20 +1968,22 @@
     "_OptionalUpdateDeviceStatusRequestRequestTypeDef",
     {
         "DeviceRememberedStatus": DeviceRememberedStatusTypeType,
     },
     total=False,
 )
 
+
 class UpdateDeviceStatusRequestRequestTypeDef(
     _RequiredUpdateDeviceStatusRequestRequestTypeDef,
     _OptionalUpdateDeviceStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
     },
 )
@@ -1686,19 +1993,21 @@
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
     },
     total=False,
 )
 
+
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
     },
 )
@@ -1708,20 +2017,30 @@
         "ProviderDetails": Mapping[str, str],
         "AttributeMapping": Mapping[str, str],
         "IdpIdentifiers": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -1730,20 +2049,31 @@
         "AccessToken": str,
         "Session": str,
         "FriendlyDeviceName": str,
     },
     total=False,
 )
 
+
 class VerifySoftwareTokenRequestRequestTypeDef(
     _RequiredVerifySoftwareTokenRequestRequestTypeDef,
     _OptionalVerifySoftwareTokenRequestRequestTypeDef,
 ):
     pass
 
+
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
+    {
+        "Status": VerifySoftwareTokenResponseTypeType,
+        "Session": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VerifyUserAttributeRequestRequestTypeDef = TypedDict(
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
@@ -1794,19 +2124,21 @@
         "MessageAction": MessageActionTypeType,
         "DesiredDeliveryMediums": Sequence[DeliveryMediumTypeType],
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AdminCreateUserRequestRequestTypeDef(
     _RequiredAdminCreateUserRequestRequestTypeDef, _OptionalAdminCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAdminUpdateUserAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredAdminUpdateUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributes": Sequence[AttributeTypeTypeDef],
     },
@@ -1815,20 +2147,22 @@
     "_OptionalAdminUpdateUserAttributesRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AdminUpdateUserAttributesRequestRequestTypeDef(
     _RequiredAdminUpdateUserAttributesRequestRequestTypeDef,
     _OptionalAdminUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 DeviceTypeTypeDef = TypedDict(
     "DeviceTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceAttributes": List[AttributeTypeTypeDef],
         "DeviceCreateDate": datetime,
         "DeviceLastModifiedDate": datetime,
@@ -1848,93 +2182,21 @@
     "_OptionalUpdateUserAttributesRequestRequestTypeDef",
     {
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
-    {
-        "SecretCode": str,
-        "Session": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
-    {
-        "UserConfirmationNecessary": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
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
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
-    {
-        "UserPoolId": str,
-        "CSVHeader": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
-    {
-        "Certificate": str,
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
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
-    {
-        "Status": VerifySoftwareTokenResponseTypeType,
-        "Session": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 AdminDisableProviderForUserRequestRequestTypeDef = TypedDict(
     "AdminDisableProviderForUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "User": ProviderUserIdentifierTypeTypeDef,
     },
@@ -1957,15 +2219,15 @@
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
     "AdminSetUserSettingsRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -1978,15 +2240,15 @@
     "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeTypeDef],
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetUserSettingsRequestRequestTypeDef = TypedDict(
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
@@ -2004,226 +2266,53 @@
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
     total=False,
 )
 
-_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "Username": str,
-        "UserPoolId": str,
-    },
-)
-_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
-    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-):
-    pass
-
-_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-    },
-)
-_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
-    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
-    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-):
-    pass
-
-_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResourceServersRequestListResourceServersPaginateTypeDef(
-    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
-    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
-):
-    pass
-
-_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
-    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-):
-    pass
-
-ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "GroupName": str,
-    },
-)
-_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
-    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-):
-    pass
-
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "Filter": str,
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
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "Username": str,
@@ -2235,20 +2324,22 @@
     {
         "SMSMfaSettings": SMSMfaSettingsTypeTypeDef,
         "SoftwareTokenMfaSettings": SoftwareTokenMfaSettingsTypeTypeDef,
     },
     total=False,
 )
 
+
 class AdminSetUserMFAPreferenceRequestRequestTypeDef(
     _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef,
     _OptionalAdminSetUserMFAPreferenceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "AccessToken": str,
     },
 )
 _OptionalSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
@@ -2256,20 +2347,22 @@
     {
         "SMSMfaSettings": SMSMfaSettingsTypeTypeDef,
         "SoftwareTokenMfaSettings": SoftwareTokenMfaSettingsTypeTypeDef,
     },
     total=False,
 )
 
+
 class SetUserMFAPreferenceRequestRequestTypeDef(
     _RequiredSetUserMFAPreferenceRequestRequestTypeDef,
     _OptionalSetUserMFAPreferenceRequestRequestTypeDef,
 ):
     pass
 
+
 AuthEventTypeTypeDef = TypedDict(
     "AuthEventTypeTypeDef",
     {
         "EventId": str,
         "EventType": EventTypeType,
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
@@ -2294,49 +2387,49 @@
     total=False,
 )
 
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
     "GetUserAttributeVerificationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResendConfirmationCodeResponseTypeDef = TypedDict(
     "ResendConfirmationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SignUpResponseTypeDef = TypedDict(
     "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
@@ -2346,20 +2439,22 @@
     "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "EventFilter": List[EventFilterTypeType],
     },
     total=False,
 )
 
+
 class CompromisedCredentialsRiskConfigurationTypeTypeDef(
     _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
     _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
 ):
     pass
 
+
 _RequiredConfirmDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmDeviceRequestRequestTypeDef",
     {
         "AccessToken": str,
         "DeviceKey": str,
     },
 )
@@ -2368,19 +2463,21 @@
     {
         "DeviceSecretVerifierConfig": DeviceSecretVerifierConfigTypeTypeDef,
         "DeviceName": str,
     },
     total=False,
 )
 
+
 class ConfirmDeviceRequestRequestTypeDef(
     _RequiredConfirmDeviceRequestRequestTypeDef, _OptionalConfirmDeviceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredConfirmForgotPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmForgotPasswordRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
         "ConfirmationCode": str,
         "Password": str,
@@ -2393,20 +2490,22 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ConfirmForgotPasswordRequestRequestTypeDef(
     _RequiredConfirmForgotPasswordRequestRequestTypeDef,
     _OptionalConfirmForgotPasswordRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredConfirmSignUpRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmSignUpRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
         "ConfirmationCode": str,
     },
@@ -2419,19 +2518,21 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ConfirmSignUpRequestRequestTypeDef(
     _RequiredConfirmSignUpRequestRequestTypeDef, _OptionalConfirmSignUpRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredForgotPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredForgotPasswordRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
     },
 )
@@ -2442,19 +2543,21 @@
         "UserContextData": UserContextDataTypeTypeDef,
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ForgotPasswordRequestRequestTypeDef(
     _RequiredForgotPasswordRequestRequestTypeDef, _OptionalForgotPasswordRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredInitiateAuthRequestRequestTypeDef",
     {
         "AuthFlow": AuthFlowTypeType,
         "ClientId": str,
     },
 )
@@ -2465,19 +2568,21 @@
         "ClientMetadata": Mapping[str, str],
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
     },
     total=False,
 )
 
+
 class InitiateAuthRequestRequestTypeDef(
     _RequiredInitiateAuthRequestRequestTypeDef, _OptionalInitiateAuthRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredResendConfirmationCodeRequestRequestTypeDef = TypedDict(
     "_RequiredResendConfirmationCodeRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
     },
 )
@@ -2488,20 +2593,22 @@
         "UserContextData": UserContextDataTypeTypeDef,
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ResendConfirmationCodeRequestRequestTypeDef(
     _RequiredResendConfirmationCodeRequestRequestTypeDef,
     _OptionalResendConfirmationCodeRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRespondToAuthChallengeRequestRequestTypeDef = TypedDict(
     "_RequiredRespondToAuthChallengeRequestRequestTypeDef",
     {
         "ClientId": str,
         "ChallengeName": ChallengeNameTypeType,
     },
 )
@@ -2513,20 +2620,22 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RespondToAuthChallengeRequestRequestTypeDef(
     _RequiredRespondToAuthChallengeRequestRequestTypeDef,
     _OptionalRespondToAuthChallengeRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSignUpRequestRequestTypeDef = TypedDict(
     "_RequiredSignUpRequestRequestTypeDef",
     {
         "ClientId": str,
         "Username": str,
         "Password": str,
     },
@@ -2540,19 +2649,21 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "UserContextData": UserContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class SignUpRequestRequestTypeDef(
     _RequiredSignUpRequestRequestTypeDef, _OptionalSignUpRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredContextDataTypeTypeDef = TypedDict(
     "_RequiredContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "ServerName": str,
         "ServerPath": str,
         "HttpHeaders": Sequence[HttpHeaderTypeDef],
@@ -2562,46 +2673,48 @@
     "_OptionalContextDataTypeTypeDef",
     {
         "EncodedData": str,
     },
     total=False,
 )
 
+
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
+
 CreateIdentityProviderResponseTypeDef = TypedDict(
     "CreateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeIdentityProviderResponseTypeDef = TypedDict(
     "DescribeIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
     "GetIdentityProviderByIdentifierResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2613,20 +2726,22 @@
     "_OptionalCreateResourceServerRequestRequestTypeDef",
     {
         "Scopes": Sequence[ResourceServerScopeTypeTypeDef],
     },
     total=False,
 )
 
+
 class CreateResourceServerRequestRequestTypeDef(
     _RequiredCreateResourceServerRequestRequestTypeDef,
     _OptionalCreateResourceServerRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceServerTypeTypeDef = TypedDict(
     "ResourceServerTypeTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
         "Scopes": List[ResourceServerScopeTypeTypeDef],
@@ -2646,58 +2761,60 @@
     "_OptionalUpdateResourceServerRequestRequestTypeDef",
     {
         "Scopes": Sequence[ResourceServerScopeTypeTypeDef],
     },
     total=False,
 )
 
+
 class UpdateResourceServerRequestRequestTypeDef(
     _RequiredUpdateResourceServerRequestRequestTypeDef,
     _OptionalUpdateResourceServerRequestRequestTypeDef,
 ):
     pass
 
+
 CreateUserImportJobResponseTypeDef = TypedDict(
     "CreateUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserImportJobResponseTypeDef = TypedDict(
     "DescribeUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserImportJobsResponseTypeDef = TypedDict(
     "ListUserImportJobsResponseTypeDef",
     {
         "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartUserImportJobResponseTypeDef = TypedDict(
     "StartUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopUserImportJobResponseTypeDef = TypedDict(
     "StopUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2727,20 +2844,22 @@
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
     total=False,
 )
 
+
 class CreateUserPoolClientRequestRequestTypeDef(
     _RequiredCreateUserPoolClientRequestRequestTypeDef,
     _OptionalCreateUserPoolClientRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
     },
 )
@@ -2767,20 +2886,22 @@
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
     total=False,
 )
 
+
 class UpdateUserPoolClientRequestRequestTypeDef(
     _RequiredUpdateUserPoolClientRequestRequestTypeDef,
     _OptionalUpdateUserPoolClientRequestRequestTypeDef,
 ):
     pass
 
+
 UserPoolClientTypeTypeDef = TypedDict(
     "UserPoolClientTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientName": str,
         "ClientId": str,
         "ClientSecret": str,
@@ -2820,20 +2941,22 @@
     "_OptionalCreateUserPoolDomainRequestRequestTypeDef",
     {
         "CustomDomainConfig": CustomDomainConfigTypeTypeDef,
     },
     total=False,
 )
 
+
 class CreateUserPoolDomainRequestRequestTypeDef(
     _RequiredCreateUserPoolDomainRequestRequestTypeDef,
     _OptionalCreateUserPoolDomainRequestRequestTypeDef,
 ):
     pass
 
+
 DomainDescriptionTypeTypeDef = TypedDict(
     "DomainDescriptionTypeTypeDef",
     {
         "UserPoolId": str,
         "AWSAccountId": str,
         "Domain": str,
         "S3Bucket": str,
@@ -2883,41 +3006,41 @@
     total=False,
 )
 
 GetUICustomizationResponseTypeDef = TypedDict(
     "GetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetUICustomizationResponseTypeDef = TypedDict(
     "SetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNotifyConfigurationTypeTypeDef = TypedDict(
     "_RequiredNotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
@@ -2931,19 +3054,21 @@
         "BlockEmail": NotifyEmailTypeTypeDef,
         "NoActionEmail": NotifyEmailTypeTypeDef,
         "MfaEmail": NotifyEmailTypeTypeDef,
     },
     total=False,
 )
 
+
 class NotifyConfigurationTypeTypeDef(
     _RequiredNotifyConfigurationTypeTypeDef, _OptionalNotifyConfigurationTypeTypeDef
 ):
     pass
 
+
 UserPoolPolicyTypeTypeDef = TypedDict(
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
@@ -2962,120 +3087,120 @@
     total=False,
 )
 
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminListDevicesResponseTypeDef = TypedDict(
     "AdminListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDeviceResponseTypeDef = TypedDict(
     "GetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminCreateUserResponseTypeDef = TypedDict(
     "AdminCreateUserResponseTypeDef",
     {
         "User": UserTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
     "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InitiateAuthResponseTypeDef = TypedDict(
     "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RespondToAuthChallengeResponseTypeDef = TypedDict(
     "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3090,19 +3215,21 @@
         "ClientMetadata": Mapping[str, str],
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ContextData": ContextDataTypeTypeDef,
     },
     total=False,
 )
 
+
 class AdminInitiateAuthRequestRequestTypeDef(
     _RequiredAdminInitiateAuthRequestRequestTypeDef, _OptionalAdminInitiateAuthRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAdminRespondToAuthChallengeRequestRequestTypeDef = TypedDict(
     "_RequiredAdminRespondToAuthChallengeRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ChallengeName": ChallengeNameTypeType,
     },
@@ -3115,92 +3242,94 @@
         "AnalyticsMetadata": AnalyticsMetadataTypeTypeDef,
         "ContextData": ContextDataTypeTypeDef,
         "ClientMetadata": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AdminRespondToAuthChallengeRequestRequestTypeDef(
     _RequiredAdminRespondToAuthChallengeRequestRequestTypeDef,
     _OptionalAdminRespondToAuthChallengeRequestRequestTypeDef,
 ):
     pass
 
+
 CreateResourceServerResponseTypeDef = TypedDict(
     "CreateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourceServerResponseTypeDef = TypedDict(
     "DescribeResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateUserPoolClientResponseTypeDef = TypedDict(
     "CreateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserPoolClientResponseTypeDef = TypedDict(
     "DescribeUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserPoolClientResponseTypeDef = TypedDict(
     "UpdateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserPoolDomainResponseTypeDef = TypedDict(
     "DescribeUserPoolDomainResponseTypeDef",
     {
         "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3212,27 +3341,29 @@
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
     },
     total=False,
 )
 
+
 class SetUserPoolMfaConfigRequestRequestTypeDef(
     _RequiredSetUserPoolMfaConfigRequestRequestTypeDef,
     _OptionalSetUserPoolMfaConfigRequestRequestTypeDef,
 ):
     pass
 
+
 SetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UserPoolDescriptionTypeTypeDef = TypedDict(
     "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
@@ -3255,20 +3386,22 @@
     "_OptionalAccountTakeoverRiskConfigurationTypeTypeDef",
     {
         "NotifyConfiguration": NotifyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class AccountTakeoverRiskConfigurationTypeTypeDef(
     _RequiredAccountTakeoverRiskConfigurationTypeTypeDef,
     _OptionalAccountTakeoverRiskConfigurationTypeTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserPoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalUpdateUserPoolRequestRequestTypeDef = TypedDict(
@@ -3292,19 +3425,21 @@
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
     total=False,
 )
 
+
 class UpdateUserPoolRequestRequestTypeDef(
     _RequiredUpdateUserPoolRequestRequestTypeDef, _OptionalUpdateUserPoolRequestRequestTypeDef
 ):
     pass
 
+
 AddCustomAttributesRequestRequestTypeDef = TypedDict(
     "AddCustomAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "CustomAttributes": Sequence[SchemaAttributeTypeTypeDef],
     },
 )
@@ -3340,19 +3475,21 @@
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
     total=False,
 )
 
+
 class CreateUserPoolRequestRequestTypeDef(
     _RequiredCreateUserPoolRequestRequestTypeDef, _OptionalCreateUserPoolRequestRequestTypeDef
 ):
     pass
 
+
 UserPoolTypeTypeDef = TypedDict(
     "UserPoolTypeTypeDef",
     {
         "Id": str,
         "Name": str,
         "Policies": UserPoolPolicyTypeTypeDef,
         "DeletionProtection": DeletionProtectionTypeType,
@@ -3390,24 +3527,26 @@
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
-        "CompromisedCredentialsRiskConfiguration": CompromisedCredentialsRiskConfigurationTypeTypeDef,
+        "CompromisedCredentialsRiskConfiguration": (
+            CompromisedCredentialsRiskConfigurationTypeTypeDef
+        ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
         "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
         "LastModifiedDate": datetime,
     },
     total=False,
 )
 
@@ -3417,51 +3556,55 @@
         "UserPoolId": str,
     },
 )
 _OptionalSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalSetRiskConfigurationRequestRequestTypeDef",
     {
         "ClientId": str,
-        "CompromisedCredentialsRiskConfiguration": CompromisedCredentialsRiskConfigurationTypeTypeDef,
+        "CompromisedCredentialsRiskConfiguration": (
+            CompromisedCredentialsRiskConfigurationTypeTypeDef
+        ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
         "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class SetRiskConfigurationRequestRequestTypeDef(
     _RequiredSetRiskConfigurationRequestRequestTypeDef,
     _OptionalSetRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 CreateUserPoolResponseTypeDef = TypedDict(
     "CreateUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserPoolResponseTypeDef = TypedDict(
     "DescribeUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRiskConfigurationResponseTypeDef = TypedDict(
     "DescribeRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetRiskConfigurationResponseTypeDef = TypedDict(
     "SetRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
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
 
 <a id="mypy-boto3-cognito-idp"></a>
 
 # mypy-boto3-cognito-idp
 
 [![PyPI - mypy-boto3-cognito-idp](https://img.shields.io/pypi/v/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,59 +400,62 @@
 from mypy_boto3_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
-    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
+    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -468,88 +472,85 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
+    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
+    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
+    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
+    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
-    ConfirmDeviceResponseTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseTypeDef,
-    GetSigningCertificateResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
@@ -645,42 +646,42 @@
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

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy-boto3-cognito-idp-1.27.0/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.26.0.post1/setup.py` & `mypy-boto3-cognito-idp-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cognito-idp.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentityProvider 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CognitoIdentityProvider 1.27.0 service generated with"
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
     keywords="boto3 cognito-idp type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cognito_idp": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cognito_idp": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/",
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


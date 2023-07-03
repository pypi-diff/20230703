# Comparing `tmp/mypy-boto3-chime-sdk-identity-1.26.98.tar.gz` & `tmp/mypy-boto3-chime-sdk-identity-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-identity-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-identity-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-identity-1.26.98.tar` & `mypy-boto3-chime-sdk-identity-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.403627 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22758 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22722 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.178904 mypy-boto3-chime-sdk-identity-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-03 19:50:27.178904 mypy-boto3-chime-sdk-identity-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.162904 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22805 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-03 19:33:24.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25376 2023-07-03 19:33:24.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-07-03 19:33:24.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.162904 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.178904 mypy-boto3-chime-sdk-identity-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-03 19:33:23.000000 mypy-boto3-chime-sdk-identity-1.27.0/setup.py
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/LICENSE` & `mypy-boto3-chime-sdk-identity-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/PKG-INFO` & `mypy-boto3-chime-sdk-identity-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-identity
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKIdentity 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKIdentity 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-identity"></a>
 
 # mypy-boto3-chime-sdk-identity
 
 [![PyPI - mypy-boto3-chime-sdk-identity](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKIdentity 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[boto3.ChimeSDKIdentity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [mypy-boto3-chime-sdk-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,16 @@
 from mypy_boto3_chime_sdk_identity.literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
     ExpirationCriterionType,
     RespondsToType,
+    StandardMessagesType,
+    TargetedMessagesType,
     ChimeSDKIdentityServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -312,78 +314,79 @@
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
-    LexConfigurationTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
+    CreateAppInstanceBotResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
+    InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    RegisterAppInstanceUserEndpointResponseTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
+    UpdateAppInstanceBotResponseTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
+    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
+    UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    ListAppInstanceBotsResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
+    ListAppInstancesResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
-    ConfigurationTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
     PutAppInstanceUserExpirationSettingsResponseTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     ListAppInstanceUserEndpointsResponseTypeDef,
     DescribeAppInstanceUserEndpointResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
+    ConfigurationTypeDef,
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
+    UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
 def get_structure() -> IdentityTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/README.md` & `mypy-boto3-chime-sdk-identity-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-identity"></a>
 
 # mypy-boto3-chime-sdk-identity
 
 [![PyPI - mypy-boto3-chime-sdk-identity](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKIdentity 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[boto3.ChimeSDKIdentity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [mypy-boto3-chime-sdk-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -251,14 +251,16 @@
 from mypy_boto3_chime_sdk_identity.literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
     ExpirationCriterionType,
     RespondsToType,
+    StandardMessagesType,
+    TargetedMessagesType,
     ChimeSDKIdentityServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -280,78 +282,79 @@
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
-    LexConfigurationTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
+    CreateAppInstanceBotResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
+    InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    RegisterAppInstanceUserEndpointResponseTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
+    UpdateAppInstanceBotResponseTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
+    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
+    UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    ListAppInstanceBotsResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
+    ListAppInstancesResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
-    ConfigurationTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
     PutAppInstanceUserExpirationSettingsResponseTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     ListAppInstanceUserEndpointsResponseTypeDef,
     DescribeAppInstanceUserEndpointResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
+    ConfigurationTypeDef,
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
+    UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
 def get_structure() -> IdentityTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__main__.py` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKIdentity 1.26.98\nVersion:         1.26.98\nBuilder"
-        " version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKIdentity 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity\nOther"
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

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.py` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,15 +411,20 @@
         Updates `AppInstance` metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance)
         """
 
     def update_app_instance_bot(
-        self, *, AppInstanceBotArn: str, Name: str, Metadata: str
+        self,
+        *,
+        AppInstanceBotArn: str,
+        Name: str,
+        Metadata: str,
+        Configuration: ConfigurationTypeDef = ...
     ) -> UpdateAppInstanceBotResponseTypeDef:
         """
         Updates the name and metadata of an `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance_bot)
         """
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.pyi` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,20 @@
         """
         Updates `AppInstance` metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance)
         """
     def update_app_instance_bot(
-        self, *, AppInstanceBotArn: str, Name: str, Metadata: str
+        self,
+        *,
+        AppInstanceBotArn: str,
+        Name: str,
+        Metadata: str,
+        Configuration: ConfigurationTypeDef = ...
     ) -> UpdateAppInstanceBotResponseTypeDef:
         """
         Updates the name and metadata of an `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance_bot)
         """
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.py` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,27 +22,31 @@
 __all__ = (
     "AllowMessagesType",
     "AppInstanceUserEndpointTypeType",
     "EndpointStatusReasonType",
     "EndpointStatusType",
     "ExpirationCriterionType",
     "RespondsToType",
+    "StandardMessagesType",
+    "TargetedMessagesType",
     "ChimeSDKIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 AllowMessagesType = Literal["ALL", "NONE"]
 AppInstanceUserEndpointTypeType = Literal["APNS", "APNS_SANDBOX", "GCM"]
 EndpointStatusReasonType = Literal["INVALID_DEVICE_TOKEN", "INVALID_PINPOINT_ARN"]
 EndpointStatusType = Literal["ACTIVE", "INACTIVE"]
 ExpirationCriterionType = Literal["CREATED_TIMESTAMP"]
 RespondsToType = Literal["STANDARD_MESSAGES"]
+StandardMessagesType = Literal["ALL", "AUTO", "MENTIONS", "NONE"]
+TargetedMessagesType = Literal["ALL", "NONE"]
 ChimeSDKIdentityServiceName = Literal["chime-sdk-identity"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -51,14 +55,15 @@
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
@@ -98,14 +103,15 @@
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
@@ -247,14 +253,15 @@
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
@@ -273,16 +280,19 @@
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
@@ -366,15 +376,17 @@
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

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.pyi` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,30 @@
 __all__ = (
     "AllowMessagesType",
     "AppInstanceUserEndpointTypeType",
     "EndpointStatusReasonType",
     "EndpointStatusType",
     "ExpirationCriterionType",
     "RespondsToType",
+    "StandardMessagesType",
+    "TargetedMessagesType",
     "ChimeSDKIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 AllowMessagesType = Literal["ALL", "NONE"]
 AppInstanceUserEndpointTypeType = Literal["APNS", "APNS_SANDBOX", "GCM"]
 EndpointStatusReasonType = Literal["INVALID_DEVICE_TOKEN", "INVALID_PINPOINT_ARN"]
 EndpointStatusType = Literal["ACTIVE", "INACTIVE"]
 ExpirationCriterionType = Literal["CREATED_TIMESTAMP"]
 RespondsToType = Literal["STANDARD_MESSAGES"]
+StandardMessagesType = Literal["ALL", "AUTO", "MENTIONS", "NONE"]
+TargetedMessagesType = Literal["ALL", "NONE"]
 ChimeSDKIdentityServiceName = Literal["chime-sdk-identity"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -49,14 +53,15 @@
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
@@ -96,14 +101,15 @@
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
@@ -245,14 +251,15 @@
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
@@ -271,16 +278,19 @@
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
@@ -364,15 +374,17 @@
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

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.py` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from typing import Dict, List, Sequence
 
 from .literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
+    StandardMessagesType,
+    TargetedMessagesType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -38,78 +40,79 @@
     "ChannelRetentionSettingsTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
     "EndpointAttributesTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "ExpirationSettingsTypeDef",
-    "LexConfigurationTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
+    "CreateAppInstanceBotResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceBotRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeregisterAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceAdminRequestRequestTypeDef",
     "DescribeAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceRequestRequestTypeDef",
     "DescribeAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceUserRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
+    "InvokedByTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceBotsRequestRequestTypeDef",
     "ListAppInstanceUserEndpointsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppInstanceBotRequestRequestTypeDef",
+    "UpdateAppInstanceBotResponseTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserEndpointRequestRequestTypeDef",
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "ListAppInstanceBotsResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
     "AppInstanceUserEndpointSummaryTypeDef",
     "AppInstanceUserEndpointTypeDef",
     "RegisterAppInstanceUserEndpointRequestRequestTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
     "AppInstanceUserTypeDef",
     "PutAppInstanceUserExpirationSettingsRequestRequestTypeDef",
-    "ConfigurationTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateAppInstanceBotResponseTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAppInstanceBotsResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "ListAppInstancesResponseTypeDef",
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    "UpdateAppInstanceBotResponseTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "LexConfigurationTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     "ListAppInstanceUserEndpointsResponseTypeDef",
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     "DescribeAppInstanceUserResponseTypeDef",
+    "ConfigurationTypeDef",
     "AppInstanceBotTypeDef",
     "CreateAppInstanceBotRequestRequestTypeDef",
+    "UpdateAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceBotResponseTypeDef",
 )
 
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "Arn": str,
@@ -212,59 +215,51 @@
     "ExpirationSettingsTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": Literal["CREATED_TIMESTAMP"],
     },
 )
 
-_RequiredLexConfigurationTypeDef = TypedDict(
-    "_RequiredLexConfigurationTypeDef",
+CreateAppInstanceAdminRequestRequestTypeDef = TypedDict(
+    "CreateAppInstanceAdminRequestRequestTypeDef",
     {
-        "RespondsTo": Literal["STANDARD_MESSAGES"],
-        "LexBotAliasArn": str,
-        "LocaleId": str,
+        "AppInstanceAdminArn": str,
+        "AppInstanceArn": str,
     },
 )
-_OptionalLexConfigurationTypeDef = TypedDict(
-    "_OptionalLexConfigurationTypeDef",
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "WelcomeIntent": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-
-class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
-    pass
-
-
-CreateAppInstanceAdminRequestRequestTypeDef = TypedDict(
-    "CreateAppInstanceAdminRequestRequestTypeDef",
+CreateAppInstanceBotResponseTypeDef = TypedDict(
+    "CreateAppInstanceBotResponseTypeDef",
     {
-        "AppInstanceAdminArn": str,
-        "AppInstanceArn": str,
+        "AppInstanceBotArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppInstanceAdminRequestRequestTypeDef = TypedDict(
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
@@ -334,21 +329,36 @@
 DescribeAppInstanceUserRequestRequestTypeDef = TypedDict(
     "DescribeAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
+InvokedByTypeDef = TypedDict(
+    "InvokedByTypeDef",
+    {
+        "StandardMessages": StandardMessagesType,
+        "TargetedMessages": TargetedMessagesType,
+    },
+)
+
 _RequiredListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppInstanceAdminsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 _OptionalListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
@@ -449,40 +459,67 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
-    "UpdateAppInstanceBotRequestRequestTypeDef",
+UpdateAppInstanceBotResponseTypeDef = TypedDict(
+    "UpdateAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBotArn": str,
-        "Name": str,
-        "Metadata": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppInstanceRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
     },
 )
@@ -499,23 +536,40 @@
 class UpdateAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -526,22 +580,58 @@
         "Admin": IdentityTypeDef,
         "AppInstanceArn": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+CreateAppInstanceAdminResponseTypeDef = TypedDict(
+    "CreateAppInstanceAdminResponseTypeDef",
+    {
+        "AppInstanceAdmin": IdentityTypeDef,
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAppInstanceBotsResponseTypeDef = TypedDict(
+    "ListAppInstanceBotsResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceRetentionSettingsTypeDef = TypedDict(
     "AppInstanceRetentionSettingsTypeDef",
     {
         "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
     total=False,
 )
 
+ListAppInstancesResponseTypeDef = TypedDict(
+    "ListAppInstancesResponseTypeDef",
+    {
+        "AppInstances": List[AppInstanceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
+    {
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceUserEndpointSummaryTypeDef = TypedDict(
     "AppInstanceUserEndpointSummaryTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
         "Name": str,
         "Type": AppInstanceUserEndpointTypeType,
@@ -591,14 +681,24 @@
 class RegisterAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredRegisterAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalRegisterAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
 
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceUserTypeDef = TypedDict(
     "AppInstanceUserTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
         "CreatedTimestamp": datetime,
@@ -626,146 +726,20 @@
 class PutAppInstanceUserExpirationSettingsRequestRequestTypeDef(
     _RequiredPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
     _OptionalPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
 ):
     pass
 
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Lex": LexConfigurationTypeDef,
-    },
-)
-
-CreateAppInstanceAdminResponseTypeDef = TypedDict(
-    "CreateAppInstanceAdminResponseTypeDef",
-    {
-        "AppInstanceAdmin": IdentityTypeDef,
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppInstanceBotResponseTypeDef = TypedDict(
-    "CreateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
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
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppInstanceBotsResponseTypeDef = TypedDict(
-    "ListAppInstanceBotsResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppInstancesResponseTypeDef = TypedDict(
-    "ListAppInstancesResponseTypeDef",
-    {
-        "AppInstances": List[AppInstanceSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutAppInstanceUserExpirationSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
     {
         "AppInstanceUserArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceBotResponseTypeDef = TypedDict(
-    "UpdateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -815,50 +789,72 @@
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
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredLexConfigurationTypeDef = TypedDict(
+    "_RequiredLexConfigurationTypeDef",
+    {
+        "LexBotAliasArn": str,
+        "LocaleId": str,
+    },
+)
+_OptionalLexConfigurationTypeDef = TypedDict(
+    "_OptionalLexConfigurationTypeDef",
+    {
+        "RespondsTo": Literal["STANDARD_MESSAGES"],
+        "InvokedBy": InvokedByTypeDef,
+        "WelcomeIntent": str,
+    },
+    total=False,
+)
+
+
+class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
+    pass
+
+
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
@@ -867,40 +863,47 @@
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
 
 ListAppInstanceUserEndpointsResponseTypeDef = TypedDict(
     "ListAppInstanceUserEndpointsResponseTypeDef",
     {
         "AppInstanceUserEndpoints": List[AppInstanceUserEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppInstanceUserEndpointResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     {
         "AppInstanceUserEndpoint": AppInstanceUserEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Lex": LexConfigurationTypeDef,
     },
 )
 
 AppInstanceBotTypeDef = TypedDict(
     "AppInstanceBotTypeDef",
     {
         "AppInstanceBotArn": str,
@@ -935,14 +938,38 @@
 class CreateAppInstanceBotRequestRequestTypeDef(
     _RequiredCreateAppInstanceBotRequestRequestTypeDef,
     _OptionalCreateAppInstanceBotRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppInstanceBotRequestRequestTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "Name": str,
+        "Metadata": str,
+    },
+)
+_OptionalUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppInstanceBotRequestRequestTypeDef",
+    {
+        "Configuration": ConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateAppInstanceBotRequestRequestTypeDef(
+    _RequiredUpdateAppInstanceBotRequestRequestTypeDef,
+    _OptionalUpdateAppInstanceBotRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeAppInstanceBotResponseTypeDef = TypedDict(
     "DescribeAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBot": AppInstanceBotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.pyi` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from typing import Dict, List, Sequence
 
 from .literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
+    StandardMessagesType,
+    TargetedMessagesType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -37,78 +39,79 @@
     "ChannelRetentionSettingsTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
     "EndpointAttributesTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "ExpirationSettingsTypeDef",
-    "LexConfigurationTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
+    "CreateAppInstanceBotResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceBotRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeregisterAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceAdminRequestRequestTypeDef",
     "DescribeAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceRequestRequestTypeDef",
     "DescribeAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceUserRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
+    "InvokedByTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceBotsRequestRequestTypeDef",
     "ListAppInstanceUserEndpointsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppInstanceBotRequestRequestTypeDef",
+    "UpdateAppInstanceBotResponseTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserEndpointRequestRequestTypeDef",
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "ListAppInstanceBotsResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
     "AppInstanceUserEndpointSummaryTypeDef",
     "AppInstanceUserEndpointTypeDef",
     "RegisterAppInstanceUserEndpointRequestRequestTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
     "AppInstanceUserTypeDef",
     "PutAppInstanceUserExpirationSettingsRequestRequestTypeDef",
-    "ConfigurationTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateAppInstanceBotResponseTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAppInstanceBotsResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "ListAppInstancesResponseTypeDef",
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    "UpdateAppInstanceBotResponseTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "LexConfigurationTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     "ListAppInstanceUserEndpointsResponseTypeDef",
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     "DescribeAppInstanceUserResponseTypeDef",
+    "ConfigurationTypeDef",
     "AppInstanceBotTypeDef",
     "CreateAppInstanceBotRequestRequestTypeDef",
+    "UpdateAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceBotResponseTypeDef",
 )
 
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "Arn": str,
@@ -207,57 +210,51 @@
     "ExpirationSettingsTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": Literal["CREATED_TIMESTAMP"],
     },
 )
 
-_RequiredLexConfigurationTypeDef = TypedDict(
-    "_RequiredLexConfigurationTypeDef",
+CreateAppInstanceAdminRequestRequestTypeDef = TypedDict(
+    "CreateAppInstanceAdminRequestRequestTypeDef",
     {
-        "RespondsTo": Literal["STANDARD_MESSAGES"],
-        "LexBotAliasArn": str,
-        "LocaleId": str,
+        "AppInstanceAdminArn": str,
+        "AppInstanceArn": str,
     },
 )
-_OptionalLexConfigurationTypeDef = TypedDict(
-    "_OptionalLexConfigurationTypeDef",
+
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "WelcomeIntent": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
-    pass
-
-CreateAppInstanceAdminRequestRequestTypeDef = TypedDict(
-    "CreateAppInstanceAdminRequestRequestTypeDef",
+CreateAppInstanceBotResponseTypeDef = TypedDict(
+    "CreateAppInstanceBotResponseTypeDef",
     {
-        "AppInstanceAdminArn": str,
-        "AppInstanceArn": str,
+        "AppInstanceBotArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppInstanceAdminRequestRequestTypeDef = TypedDict(
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
@@ -327,21 +324,36 @@
 DescribeAppInstanceUserRequestRequestTypeDef = TypedDict(
     "DescribeAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
+InvokedByTypeDef = TypedDict(
+    "InvokedByTypeDef",
+    {
+        "StandardMessages": StandardMessagesType,
+        "TargetedMessages": TargetedMessagesType,
+    },
+)
+
 _RequiredListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppInstanceAdminsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 _OptionalListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
@@ -434,40 +446,67 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "RegisterAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
-    "UpdateAppInstanceBotRequestRequestTypeDef",
+UpdateAppInstanceBotResponseTypeDef = TypedDict(
+    "UpdateAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBotArn": str,
-        "Name": str,
-        "Metadata": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppInstanceRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
     },
 )
@@ -482,23 +521,40 @@
 
 class UpdateAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
+UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserEndpointResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "EndpointId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
     },
 )
 
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceAdminSummaryTypeDef = TypedDict(
     "AppInstanceAdminSummaryTypeDef",
     {
         "Admin": IdentityTypeDef,
     },
     total=False,
 )
@@ -509,22 +565,58 @@
         "Admin": IdentityTypeDef,
         "AppInstanceArn": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+CreateAppInstanceAdminResponseTypeDef = TypedDict(
+    "CreateAppInstanceAdminResponseTypeDef",
+    {
+        "AppInstanceAdmin": IdentityTypeDef,
+        "AppInstanceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAppInstanceBotsResponseTypeDef = TypedDict(
+    "ListAppInstanceBotsResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceRetentionSettingsTypeDef = TypedDict(
     "AppInstanceRetentionSettingsTypeDef",
     {
         "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
     },
     total=False,
 )
 
+ListAppInstancesResponseTypeDef = TypedDict(
+    "ListAppInstancesResponseTypeDef",
+    {
+        "AppInstances": List[AppInstanceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
+    {
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceUserEndpointSummaryTypeDef = TypedDict(
     "AppInstanceUserEndpointSummaryTypeDef",
     {
         "AppInstanceUserArn": str,
         "EndpointId": str,
         "Name": str,
         "Type": AppInstanceUserEndpointTypeType,
@@ -572,14 +664,24 @@
 
 class RegisterAppInstanceUserEndpointRequestRequestTypeDef(
     _RequiredRegisterAppInstanceUserEndpointRequestRequestTypeDef,
     _OptionalRegisterAppInstanceUserEndpointRequestRequestTypeDef,
 ):
     pass
 
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AppInstanceUserTypeDef = TypedDict(
     "AppInstanceUserTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
         "Metadata": str,
         "CreatedTimestamp": datetime,
@@ -605,146 +707,20 @@
 
 class PutAppInstanceUserExpirationSettingsRequestRequestTypeDef(
     _RequiredPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
     _OptionalPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
 ):
     pass
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Lex": LexConfigurationTypeDef,
-    },
-)
-
-CreateAppInstanceAdminResponseTypeDef = TypedDict(
-    "CreateAppInstanceAdminResponseTypeDef",
-    {
-        "AppInstanceAdmin": IdentityTypeDef,
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppInstanceBotResponseTypeDef = TypedDict(
-    "CreateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
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
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppInstanceBotsResponseTypeDef = TypedDict(
-    "ListAppInstanceBotsResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceBots": List[AppInstanceBotSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppInstancesResponseTypeDef = TypedDict(
-    "ListAppInstancesResponseTypeDef",
-    {
-        "AppInstances": List[AppInstanceSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutAppInstanceUserExpirationSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceUserExpirationSettingsResponseTypeDef",
     {
         "AppInstanceUserArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "RegisterAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceBotResponseTypeDef = TypedDict(
-    "UpdateAppInstanceBotResponseTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceUserEndpointResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserEndpointResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "EndpointId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -790,50 +766,70 @@
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
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredLexConfigurationTypeDef = TypedDict(
+    "_RequiredLexConfigurationTypeDef",
+    {
+        "LexBotAliasArn": str,
+        "LocaleId": str,
+    },
+)
+_OptionalLexConfigurationTypeDef = TypedDict(
+    "_OptionalLexConfigurationTypeDef",
+    {
+        "RespondsTo": Literal["STANDARD_MESSAGES"],
+        "InvokedBy": InvokedByTypeDef,
+        "WelcomeIntent": str,
+    },
+    total=False,
+)
+
+class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
+    pass
+
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
@@ -842,40 +838,47 @@
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
 
 ListAppInstanceUserEndpointsResponseTypeDef = TypedDict(
     "ListAppInstanceUserEndpointsResponseTypeDef",
     {
         "AppInstanceUserEndpoints": List[AppInstanceUserEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppInstanceUserEndpointResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     {
         "AppInstanceUserEndpoint": AppInstanceUserEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Lex": LexConfigurationTypeDef,
     },
 )
 
 AppInstanceBotTypeDef = TypedDict(
     "AppInstanceBotTypeDef",
     {
         "AppInstanceBotArn": str,
@@ -908,14 +911,36 @@
 
 class CreateAppInstanceBotRequestRequestTypeDef(
     _RequiredCreateAppInstanceBotRequestRequestTypeDef,
     _OptionalCreateAppInstanceBotRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppInstanceBotRequestRequestTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "Name": str,
+        "Metadata": str,
+    },
+)
+_OptionalUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppInstanceBotRequestRequestTypeDef",
+    {
+        "Configuration": ConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateAppInstanceBotRequestRequestTypeDef(
+    _RequiredUpdateAppInstanceBotRequestRequestTypeDef,
+    _OptionalUpdateAppInstanceBotRequestRequestTypeDef,
+):
+    pass
+
 DescribeAppInstanceBotResponseTypeDef = TypedDict(
     "DescribeAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBot": AppInstanceBotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-identity
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKIdentity 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKIdentity 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-identity"></a>
 
 # mypy-boto3-chime-sdk-identity
 
 [![PyPI - mypy-boto3-chime-sdk-identity](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKIdentity 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[boto3.ChimeSDKIdentity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
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
 [mypy-boto3-chime-sdk-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,16 @@
 from mypy_boto3_chime_sdk_identity.literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
     ExpirationCriterionType,
     RespondsToType,
+    StandardMessagesType,
+    TargetedMessagesType,
     ChimeSDKIdentityServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -312,78 +314,79 @@
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
-    LexConfigurationTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
+    CreateAppInstanceBotResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
+    InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    RegisterAppInstanceUserEndpointResponseTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
+    UpdateAppInstanceBotResponseTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
+    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
+    UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    ListAppInstanceBotsResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
+    ListAppInstancesResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
-    ConfigurationTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
     PutAppInstanceUserExpirationSettingsResponseTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     ListAppInstanceUserEndpointsResponseTypeDef,
     DescribeAppInstanceUserEndpointResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
+    ConfigurationTypeDef,
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
+    UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
 def get_structure() -> IdentityTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-identity-1.27.0/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-identity-1.26.98/setup.py` & `mypy-boto3-chime-sdk-identity-1.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-identity",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_chime_sdk_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKIdentity 1.26.98 service generated with"
-        " mypy-boto3-builder 7.14.2"
+        "Type annotations for boto3.ChimeSDKIdentity 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


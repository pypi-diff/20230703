# Comparing `tmp/mypy-boto3-ssm-contacts-1.26.101.tar.gz` & `tmp/mypy-boto3-ssm-contacts-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-contacts-1.26.101.tar", last modified: Tue Mar 28 20:46:58 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-contacts-1.27.0.tar", last modified: Mon Jul  3 19:51:30 2023, max compression
```

## Comparing `mypy-boto3-ssm-contacts-1.26.101.tar` & `mypy-boto3-ssm-contacts-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:46:58.808918 mypy-boto3-ssm-contacts-1.26.101/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-03-28 20:46:58.808918 mypy-boto3-ssm-contacts-1.26.101/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17150 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:46:58.808918 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-03-28 20:46:48.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-03-28 20:46:48.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39435 2023-03-28 20:46:49.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39360 2023-03-28 20:46:48.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:46:58.808918 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-03-28 20:46:58.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-28 20:46:58.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:46:58.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:46:58.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-28 20:46:58.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-28 20:46:58.000000 mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 20:46:58.808918 mypy-boto3-ssm-contacts-1.26.101/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-28 20:46:47.000000 mypy-boto3-ssm-contacts-1.26.101/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.232044 mypy-boto3-ssm-contacts-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-03 19:51:30.232044 mypy-boto3-ssm-contacts-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.232044 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-03 19:48:39.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-03 19:48:37.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39505 2023-07-03 19:48:40.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39430 2023-07-03 19:48:40.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.232044 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-03 19:51:30.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:51:30.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:30.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:30.000000 mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:30.232044 mypy-boto3-ssm-contacts-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:48:36.000000 mypy-boto3-ssm-contacts-1.27.0/setup.py
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/LICENSE` & `mypy-boto3-ssm-contacts-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.26.101/PKG-INFO` & `mypy-boto3-ssm-contacts-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.26.101
-Summary: Type annotations for boto3.SSMContacts 1.26.101 service generated with mypy-boto3-builder 7.14.4
+Version: 1.27.0
+Summary: Type annotations for boto3.SSMContacts 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-contacts?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.26.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,14 +356,15 @@
     ListRotationsPaginatorName,
     ReceiptTypeType,
     ShiftTypeType,
     SSMContactsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
@@ -379,83 +380,83 @@
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateContactChannelResultTypeDef,
     TagTypeDef,
+    CreateContactResultTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
+    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
+    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
+    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
+    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactChannelsRequestRequestTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     TimeRangeTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutContactPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
+    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
+    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
     TargetTypeDef,
+    ListContactsResultTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
-    CreateContactChannelResultTypeDef,
-    CreateContactResultTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
-    DescribeEngagementResultTypeDef,
-    DescribePageResultTypeDef,
-    GetContactChannelResultTypeDef,
-    GetContactPolicyResultTypeDef,
-    GetRotationOverrideResultTypeDef,
-    ListContactsResultTypeDef,
-    StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/README.md` & `mypy-boto3-ssm-contacts-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-contacts?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.26.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,14 +324,15 @@
     ListRotationsPaginatorName,
     ReceiptTypeType,
     ShiftTypeType,
     SSMContactsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
@@ -347,83 +348,83 @@
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateContactChannelResultTypeDef,
     TagTypeDef,
+    CreateContactResultTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
+    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
+    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
+    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
+    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactChannelsRequestRequestTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     TimeRangeTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutContactPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
+    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
+    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
     TargetTypeDef,
+    ListContactsResultTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
-    CreateContactChannelResultTypeDef,
-    CreateContactResultTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
-    DescribeEngagementResultTypeDef,
-    DescribePageResultTypeDef,
-    GetContactChannelResultTypeDef,
-    GetContactPolicyResultTypeDef,
-    GetRotationOverrideResultTypeDef,
-    ListContactsResultTypeDef,
-    StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/__init__.py` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/__init__.pyi` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/__main__.py` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMContacts 1.26.101\nVersion:         1.26.101\nBuilder"
-        " version: 7.14.4\nDocs:           "
+        "Type annotations for boto3.SSMContacts 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.101")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/client.py` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/client.pyi` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/literals.py` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "ListRotationsPaginatorName",
     "ReceiptTypeType",
     "ShiftTypeType",
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
@@ -77,14 +78,15 @@
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
@@ -124,14 +126,15 @@
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
@@ -273,14 +276,15 @@
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
@@ -299,16 +303,19 @@
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
@@ -392,15 +399,17 @@
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
@@ -431,7 +440,25 @@
     "list_pages_by_contact",
     "list_pages_by_engagement",
     "list_preview_rotation_shifts",
     "list_rotation_overrides",
     "list_rotation_shifts",
     "list_rotations",
 ]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
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

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/literals.pyi` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "ListRotationsPaginatorName",
     "ReceiptTypeType",
     "ShiftTypeType",
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
 ContactTypeType = Literal["ESCALATION", "ONCALL_SCHEDULE", "PERSONAL"]
@@ -75,14 +76,15 @@
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
@@ -122,14 +124,15 @@
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
@@ -271,14 +274,15 @@
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
@@ -297,16 +301,19 @@
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
@@ -390,15 +397,17 @@
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
@@ -429,7 +438,25 @@
     "list_pages_by_contact",
     "list_pages_by_engagement",
     "list_preview_rotation_shifts",
     "list_rotation_overrides",
     "list_rotation_shifts",
     "list_rotations",
 ]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
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

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/paginator.py` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -73,138 +73,128 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
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
 class ListContactChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContactChannelsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
         """
 
-
 class ListContactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
         """
 
-
 class ListEngagementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
         """
 
-
 class ListPageReceiptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPageReceiptsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
         """
 
-
 class ListPageResolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPageResolutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
         """
 
-
 class ListPagesByContactPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPagesByContactResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
         """
 
-
 class ListPagesByEngagementPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
     """
 
     def paginate(
-        self, *, EngagementId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EngagementId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPagesByEngagementResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
         """
 
-
 class ListPreviewRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
@@ -213,68 +203,65 @@
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
-
 class ListRotationOverridesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
-
 class ListRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         EndTime: Union[datetime, str],
         StartTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
-
 class ListRotationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
     """
 
     def paginate(
-        self, *, RotationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RotationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRotationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/paginator.pyi` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,128 +73,138 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
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
 class ListContactChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContactChannelsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactchannelspaginator)
         """
 
+
 class ListContactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listcontactspaginator)
         """
 
+
 class ListEngagementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listengagementspaginator)
         """
 
+
 class ListPageReceiptsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPageReceiptsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagereceiptspaginator)
         """
 
+
 class ListPageResolutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPageResolutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpageresolutionspaginator)
         """
 
+
 class ListPagesByContactPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPagesByContactResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbycontactpaginator)
         """
 
+
 class ListPagesByEngagementPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
     """
 
     def paginate(
-        self, *, EngagementId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EngagementId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPagesByEngagementResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpagesbyengagementpaginator)
         """
 
+
 class ListPreviewRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
@@ -203,65 +213,68 @@
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
         Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
+
 class ListRotationOverridesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
+
 class ListRotationShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
         EndTime: Union[datetime, str],
         StartTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
+
 class ListRotationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
     """
 
     def paginate(
-        self, *, RotationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RotationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRotationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/paginators/#listrotationspaginator)
         """
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/type_defs.py` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,83 +36,83 @@
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
     "HandOffTimeTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateContactChannelResultTypeDef",
     "TagTypeDef",
+    "CreateContactResultTypeDef",
     "CreateRotationOverrideRequestRequestTypeDef",
+    "CreateRotationOverrideResultTypeDef",
+    "CreateRotationResultTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
+    "DescribeEngagementResultTypeDef",
     "DescribePageRequestRequestTypeDef",
+    "DescribePageResultTypeDef",
     "EngagementTypeDef",
     "GetContactChannelRequestRequestTypeDef",
     "GetContactPolicyRequestRequestTypeDef",
+    "GetContactPolicyResultTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
+    "GetRotationOverrideResultTypeDef",
     "GetRotationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
     "TimeRangeTypeDef",
+    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
+    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
+    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
+    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
     "PreviewOverrideTypeDef",
+    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
+    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     "ListRotationShiftsRequestRequestTypeDef",
+    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
+    "StartEngagementResultTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
+    "GetContactChannelResultTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
     "TargetTypeDef",
+    "ListContactsResultTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
-    "CreateContactChannelResultTypeDef",
-    "CreateContactResultTypeDef",
-    "CreateRotationOverrideResultTypeDef",
-    "CreateRotationResultTypeDef",
-    "DescribeEngagementResultTypeDef",
-    "DescribePageResultTypeDef",
-    "GetContactChannelResultTypeDef",
-    "GetContactPolicyResultTypeDef",
-    "GetRotationOverrideResultTypeDef",
-    "ListContactsResultTypeDef",
-    "StartEngagementResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEngagementsResultTypeDef",
-    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
-    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
@@ -243,34 +243,39 @@
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateContactChannelResultTypeDef = TypedDict(
+    "CreateContactChannelResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ContactChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+CreateContactResultTypeDef = TypedDict(
+    "CreateContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "NewContactIds": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -288,14 +293,30 @@
 class CreateRotationOverrideRequestRequestTypeDef(
     _RequiredCreateRotationOverrideRequestRequestTypeDef,
     _OptionalCreateRotationOverrideRequestRequestTypeDef,
 ):
     pass
 
 
+CreateRotationOverrideResultTypeDef = TypedDict(
+    "CreateRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRotationResultTypeDef = TypedDict(
+    "CreateRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -331,21 +352,57 @@
 DescribeEngagementRequestRequestTypeDef = TypedDict(
     "DescribeEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 
+DescribeEngagementResultTypeDef = TypedDict(
+    "DescribeEngagementResultTypeDef",
+    {
+        "ContactArn": str,
+        "EngagementArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "StartTime": datetime,
+        "StopTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePageRequestRequestTypeDef = TypedDict(
     "DescribePageRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 
+DescribePageResultTypeDef = TypedDict(
+    "DescribePageResultTypeDef",
+    {
+        "PageArn": str,
+        "EngagementArn": str,
+        "ContactArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "SentTime": datetime,
+        "ReadTime": datetime,
+        "DeliveryTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEngagementTypeDef = TypedDict(
     "_RequiredEngagementTypeDef",
     {
         "EngagementArn": str,
         "ContactArn": str,
         "Sender": str,
     },
@@ -375,14 +432,23 @@
 GetContactPolicyRequestRequestTypeDef = TypedDict(
     "GetContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
     },
 )
 
+GetContactPolicyResultTypeDef = TypedDict(
+    "GetContactPolicyResultTypeDef",
+    {
+        "ContactArn": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 
@@ -390,31 +456,56 @@
     "GetRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "RotationOverrideId": str,
     },
 )
 
+GetRotationOverrideResultTypeDef = TypedDict(
+    "GetRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "RotationArn": str,
+        "NewContactIds": List[str],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "CreateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRotationRequestRequestTypeDef = TypedDict(
     "GetRotationRequestRequestTypeDef",
     {
         "RotationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ContactId": str,
+    },
+)
+_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
+    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListContactChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactChannelsRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListContactChannelsRequestRequestTypeDef = TypedDict(
@@ -430,14 +521,24 @@
 class ListContactChannelsRequestRequestTypeDef(
     _RequiredListContactChannelsRequestRequestTypeDef,
     _OptionalListContactChannelsRequestRequestTypeDef,
 ):
     pass
 
 
+ListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "ListContactsRequestListContactsPaginateTypeDef",
+    {
+        "AliasPrefix": str,
+        "Type": ContactTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListContactsRequestRequestTypeDef = TypedDict(
     "ListContactsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
@@ -450,14 +551,36 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
+    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -493,14 +616,36 @@
 )
 
 
 class ReceiptTypeDef(_RequiredReceiptTypeDef, _OptionalReceiptTypeDef):
     pass
 
 
+_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
+    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPageResolutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageResolutionsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageResolutionsRequestRequestTypeDef = TypedDict(
@@ -537,14 +682,36 @@
 
 class ResolutionContactTypeDef(
     _RequiredResolutionContactTypeDef, _OptionalResolutionContactTypeDef
 ):
     pass
 
 
+_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
+    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPagesByContactRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListPagesByContactRequestRequestTypeDef = TypedDict(
@@ -585,14 +752,36 @@
 )
 
 
 class PageTypeDef(_RequiredPageTypeDef, _OptionalPageTypeDef):
     pass
 
 
+_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "EngagementId": str,
+    },
+)
+_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
+    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPagesByEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalListPagesByEngagementRequestRequestTypeDef = TypedDict(
@@ -618,14 +807,38 @@
         "NewMembers": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
+    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationOverridesRequestRequestTypeDef",
     {
         "RotationId": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
@@ -654,14 +867,38 @@
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
+_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
+    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationShiftsRequestRequestTypeDef",
     {
         "RotationId": str,
         "EndTime": Union[datetime, str],
     },
 )
@@ -679,14 +916,23 @@
 class ListRotationShiftsRequestRequestTypeDef(
     _RequiredListRotationShiftsRequestRequestTypeDef,
     _OptionalListRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
 
+ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
+    "ListRotationsRequestListRotationsPaginateTypeDef",
+    {
+        "RotationNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -696,22 +942,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
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
 ShiftDetailsTypeDef = TypedDict(
     "ShiftDetailsTypeDef",
     {
         "OverriddenContactIds": List[str],
     },
 )
 
@@ -745,14 +1012,22 @@
 
 class StartEngagementRequestRequestTypeDef(
     _RequiredStartEngagementRequestRequestTypeDef, _OptionalStartEngagementRequestRequestTypeDef
 ):
     pass
 
 
+StartEngagementResultTypeDef = TypedDict(
+    "StartEngagementResultTypeDef",
+    {
+        "EngagementArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredStopEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalStopEngagementRequestRequestTypeDef = TypedDict(
@@ -823,14 +1098,27 @@
 class CreateContactChannelRequestRequestTypeDef(
     _RequiredCreateContactChannelRequestRequestTypeDef,
     _OptionalCreateContactChannelRequestRequestTypeDef,
 ):
     pass
 
 
+GetContactChannelResultTypeDef = TypedDict(
+    "GetContactChannelResultTypeDef",
+    {
+        "ContactArn": str,
+        "ContactChannelArn": str,
+        "Name": str,
+        "Type": ChannelTypeType,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
+        "ActivationStatus": ActivationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateContactChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalUpdateContactChannelRequestRequestTypeDef = TypedDict(
@@ -855,14 +1143,23 @@
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
+ListContactsResultTypeDef = TypedDict(
+    "ListContactsResultTypeDef",
+    {
+        "NextToken": str,
+        "Contacts": List[ContactTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
         "End": HandOffTimeTypeDef,
     },
     total=False,
@@ -880,139 +1177,19 @@
     "WeeklySettingTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "HandOffTime": HandOffTimeTypeDef,
     },
 )
 
-CreateContactChannelResultTypeDef = TypedDict(
-    "CreateContactChannelResultTypeDef",
-    {
-        "ContactChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateContactResultTypeDef = TypedDict(
-    "CreateContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRotationOverrideResultTypeDef = TypedDict(
-    "CreateRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRotationResultTypeDef = TypedDict(
-    "CreateRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEngagementResultTypeDef = TypedDict(
-    "DescribeEngagementResultTypeDef",
-    {
-        "ContactArn": str,
-        "EngagementArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "StartTime": datetime,
-        "StopTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePageResultTypeDef = TypedDict(
-    "DescribePageResultTypeDef",
-    {
-        "PageArn": str,
-        "EngagementArn": str,
-        "ContactArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "SentTime": datetime,
-        "ReadTime": datetime,
-        "DeliveryTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactChannelResultTypeDef = TypedDict(
-    "GetContactChannelResultTypeDef",
-    {
-        "ContactArn": str,
-        "ContactChannelArn": str,
-        "Name": str,
-        "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
-        "ActivationStatus": ActivationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactPolicyResultTypeDef = TypedDict(
-    "GetContactPolicyResultTypeDef",
-    {
-        "ContactArn": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRotationOverrideResultTypeDef = TypedDict(
-    "GetRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "RotationArn": str,
-        "NewContactIds": List[str],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "CreateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListContactsResultTypeDef = TypedDict(
-    "ListContactsResultTypeDef",
-    {
-        "NextToken": str,
-        "Contacts": List[ContactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartEngagementResultTypeDef = TypedDict(
-    "StartEngagementResultTypeDef",
-    {
-        "EngagementArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
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
@@ -1021,201 +1198,24 @@
 )
 
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
-    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
-):
-    pass
-
-
-ListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "ListContactsRequestListContactsPaginateTypeDef",
-    {
-        "AliasPrefix": str,
-        "Type": ContactTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
-    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
-    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
-    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "EngagementId": str,
-    },
-)
-_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
-    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
-    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
-    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-):
-    pass
-
-
-ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
-    "ListRotationsRequestListRotationsPaginateTypeDef",
-    {
-        "RotationNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     {
         "IncidentId": str,
         "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEngagementsRequestRequestTypeDef = TypedDict(
     "ListEngagementsRequestRequestTypeDef",
     {
@@ -1228,51 +1228,51 @@
 )
 
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPageResolutionsResultTypeDef = TypedDict(
     "ListPageResolutionsResultTypeDef",
     {
         "NextToken": str,
         "PageResolutions": List[ResolutionContactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPagesByContactResultTypeDef = TypedDict(
     "ListPagesByContactResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPagesByEngagementResultTypeDef = TypedDict(
     "ListPagesByEngagementResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRotationOverridesResultTypeDef = TypedDict(
     "ListRotationOverridesResultTypeDef",
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
@@ -1295,15 +1295,15 @@
 
 
 ListContactChannelsResultTypeDef = TypedDict(
     "ListContactChannelsResultTypeDef",
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
@@ -1337,24 +1337,24 @@
 
 
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRotationShiftsResultTypeDef = TypedDict(
     "ListRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
@@ -1394,15 +1394,15 @@
     {
         "RotationArn": str,
         "Name": str,
         "ContactIds": List[str],
         "StartTime": datetime,
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "EndTime": Union[datetime, str],
@@ -1413,15 +1413,15 @@
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "RotationStartTime": Union[datetime, str],
         "StartTime": Union[datetime, str],
         "Overrides": Sequence[PreviewOverrideTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
     _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
@@ -1535,15 +1535,15 @@
     "GetContactResultTypeDef",
     {
         "ContactArn": str,
         "Alias": str,
         "DisplayName": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
@@ -1566,10 +1566,10 @@
 
 
 ListRotationsResultTypeDef = TypedDict(
     "ListRotationsResultTypeDef",
     {
         "NextToken": str,
         "Rotations": List[RotationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts/type_defs.pyi` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -35,83 +35,83 @@
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
     "HandOffTimeTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateContactChannelResultTypeDef",
     "TagTypeDef",
+    "CreateContactResultTypeDef",
     "CreateRotationOverrideRequestRequestTypeDef",
+    "CreateRotationOverrideResultTypeDef",
+    "CreateRotationResultTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
+    "DescribeEngagementResultTypeDef",
     "DescribePageRequestRequestTypeDef",
+    "DescribePageResultTypeDef",
     "EngagementTypeDef",
     "GetContactChannelRequestRequestTypeDef",
     "GetContactPolicyRequestRequestTypeDef",
+    "GetContactPolicyResultTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
+    "GetRotationOverrideResultTypeDef",
     "GetRotationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
     "TimeRangeTypeDef",
+    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
+    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
+    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
+    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
     "PreviewOverrideTypeDef",
+    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
     "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
+    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
     "ListRotationShiftsRequestRequestTypeDef",
+    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
+    "StartEngagementResultTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
+    "GetContactChannelResultTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
     "TargetTypeDef",
+    "ListContactsResultTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
-    "CreateContactChannelResultTypeDef",
-    "CreateContactResultTypeDef",
-    "CreateRotationOverrideResultTypeDef",
-    "CreateRotationResultTypeDef",
-    "DescribeEngagementResultTypeDef",
-    "DescribePageResultTypeDef",
-    "GetContactChannelResultTypeDef",
-    "GetContactPolicyResultTypeDef",
-    "GetRotationOverrideResultTypeDef",
-    "ListContactsResultTypeDef",
-    "StartEngagementResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEngagementsResultTypeDef",
-    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
-    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
@@ -234,34 +234,39 @@
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateContactChannelResultTypeDef = TypedDict(
+    "CreateContactChannelResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ContactChannelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+CreateContactResultTypeDef = TypedDict(
+    "CreateContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "NewContactIds": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -277,14 +282,30 @@
 
 class CreateRotationOverrideRequestRequestTypeDef(
     _RequiredCreateRotationOverrideRequestRequestTypeDef,
     _OptionalCreateRotationOverrideRequestRequestTypeDef,
 ):
     pass
 
+CreateRotationOverrideResultTypeDef = TypedDict(
+    "CreateRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRotationResultTypeDef = TypedDict(
+    "CreateRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -320,21 +341,57 @@
 DescribeEngagementRequestRequestTypeDef = TypedDict(
     "DescribeEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 
+DescribeEngagementResultTypeDef = TypedDict(
+    "DescribeEngagementResultTypeDef",
+    {
+        "ContactArn": str,
+        "EngagementArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "StartTime": datetime,
+        "StopTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePageRequestRequestTypeDef = TypedDict(
     "DescribePageRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 
+DescribePageResultTypeDef = TypedDict(
+    "DescribePageResultTypeDef",
+    {
+        "PageArn": str,
+        "EngagementArn": str,
+        "ContactArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "SentTime": datetime,
+        "ReadTime": datetime,
+        "DeliveryTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEngagementTypeDef = TypedDict(
     "_RequiredEngagementTypeDef",
     {
         "EngagementArn": str,
         "ContactArn": str,
         "Sender": str,
     },
@@ -362,14 +419,23 @@
 GetContactPolicyRequestRequestTypeDef = TypedDict(
     "GetContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
     },
 )
 
+GetContactPolicyResultTypeDef = TypedDict(
+    "GetContactPolicyResultTypeDef",
+    {
+        "ContactArn": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 
@@ -377,31 +443,54 @@
     "GetRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "RotationOverrideId": str,
     },
 )
 
+GetRotationOverrideResultTypeDef = TypedDict(
+    "GetRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "RotationArn": str,
+        "NewContactIds": List[str],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "CreateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRotationRequestRequestTypeDef = TypedDict(
     "GetRotationRequestRequestTypeDef",
     {
         "RotationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ContactId": str,
+    },
+)
+_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
+    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
+):
+    pass
+
 _RequiredListContactChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactChannelsRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListContactChannelsRequestRequestTypeDef = TypedDict(
@@ -415,14 +504,24 @@
 
 class ListContactChannelsRequestRequestTypeDef(
     _RequiredListContactChannelsRequestRequestTypeDef,
     _OptionalListContactChannelsRequestRequestTypeDef,
 ):
     pass
 
+ListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "ListContactsRequestListContactsPaginateTypeDef",
+    {
+        "AliasPrefix": str,
+        "Type": ContactTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListContactsRequestRequestTypeDef = TypedDict(
     "ListContactsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
@@ -435,14 +534,34 @@
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
+    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -474,14 +593,34 @@
     },
     total=False,
 )
 
 class ReceiptTypeDef(_RequiredReceiptTypeDef, _OptionalReceiptTypeDef):
     pass
 
+_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
+    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPageResolutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageResolutionsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageResolutionsRequestRequestTypeDef = TypedDict(
@@ -514,14 +653,34 @@
 )
 
 class ResolutionContactTypeDef(
     _RequiredResolutionContactTypeDef, _OptionalResolutionContactTypeDef
 ):
     pass
 
+_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
+    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
+):
+    pass
+
 _RequiredListPagesByContactRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListPagesByContactRequestRequestTypeDef = TypedDict(
@@ -558,14 +717,34 @@
     },
     total=False,
 )
 
 class PageTypeDef(_RequiredPageTypeDef, _OptionalPageTypeDef):
     pass
 
+_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "EngagementId": str,
+    },
+)
+_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
+    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+):
+    pass
+
 _RequiredListPagesByEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalListPagesByEngagementRequestRequestTypeDef = TypedDict(
@@ -589,14 +768,36 @@
         "NewMembers": Sequence[str],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
+    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+):
+    pass
+
 _RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationOverridesRequestRequestTypeDef",
     {
         "RotationId": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
@@ -623,14 +824,36 @@
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
+_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": Union[datetime, str],
+    },
+)
+_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
+    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListRotationShiftsRequestRequestTypeDef",
     {
         "RotationId": str,
         "EndTime": Union[datetime, str],
     },
 )
@@ -646,14 +869,23 @@
 
 class ListRotationShiftsRequestRequestTypeDef(
     _RequiredListRotationShiftsRequestRequestTypeDef,
     _OptionalListRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
+ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
+    "ListRotationsRequestListRotationsPaginateTypeDef",
+    {
+        "RotationNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -663,22 +895,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
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
 ShiftDetailsTypeDef = TypedDict(
     "ShiftDetailsTypeDef",
     {
         "OverriddenContactIds": List[str],
     },
 )
 
@@ -710,14 +963,22 @@
 )
 
 class StartEngagementRequestRequestTypeDef(
     _RequiredStartEngagementRequestRequestTypeDef, _OptionalStartEngagementRequestRequestTypeDef
 ):
     pass
 
+StartEngagementResultTypeDef = TypedDict(
+    "StartEngagementResultTypeDef",
+    {
+        "EngagementArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredStopEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalStopEngagementRequestRequestTypeDef = TypedDict(
@@ -782,14 +1043,27 @@
 
 class CreateContactChannelRequestRequestTypeDef(
     _RequiredCreateContactChannelRequestRequestTypeDef,
     _OptionalCreateContactChannelRequestRequestTypeDef,
 ):
     pass
 
+GetContactChannelResultTypeDef = TypedDict(
+    "GetContactChannelResultTypeDef",
+    {
+        "ContactArn": str,
+        "ContactChannelArn": str,
+        "Name": str,
+        "Type": ChannelTypeType,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
+        "ActivationStatus": ActivationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateContactChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalUpdateContactChannelRequestRequestTypeDef = TypedDict(
@@ -812,14 +1086,23 @@
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
+ListContactsResultTypeDef = TypedDict(
+    "ListContactsResultTypeDef",
+    {
+        "NextToken": str,
+        "Contacts": List[ContactTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
         "End": HandOffTimeTypeDef,
     },
     total=False,
@@ -837,139 +1120,19 @@
     "WeeklySettingTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "HandOffTime": HandOffTimeTypeDef,
     },
 )
 
-CreateContactChannelResultTypeDef = TypedDict(
-    "CreateContactChannelResultTypeDef",
-    {
-        "ContactChannelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateContactResultTypeDef = TypedDict(
-    "CreateContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRotationOverrideResultTypeDef = TypedDict(
-    "CreateRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRotationResultTypeDef = TypedDict(
-    "CreateRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEngagementResultTypeDef = TypedDict(
-    "DescribeEngagementResultTypeDef",
-    {
-        "ContactArn": str,
-        "EngagementArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "StartTime": datetime,
-        "StopTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePageResultTypeDef = TypedDict(
-    "DescribePageResultTypeDef",
-    {
-        "PageArn": str,
-        "EngagementArn": str,
-        "ContactArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "SentTime": datetime,
-        "ReadTime": datetime,
-        "DeliveryTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactChannelResultTypeDef = TypedDict(
-    "GetContactChannelResultTypeDef",
-    {
-        "ContactArn": str,
-        "ContactChannelArn": str,
-        "Name": str,
-        "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
-        "ActivationStatus": ActivationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetContactPolicyResultTypeDef = TypedDict(
-    "GetContactPolicyResultTypeDef",
-    {
-        "ContactArn": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRotationOverrideResultTypeDef = TypedDict(
-    "GetRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "RotationArn": str,
-        "NewContactIds": List[str],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "CreateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListContactsResultTypeDef = TypedDict(
-    "ListContactsResultTypeDef",
-    {
-        "NextToken": str,
-        "Contacts": List[ContactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartEngagementResultTypeDef = TypedDict(
-    "StartEngagementResultTypeDef",
-    {
-        "EngagementArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
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
@@ -978,187 +1141,24 @@
 )
 
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
-    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
-):
-    pass
-
-ListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "ListContactsRequestListContactsPaginateTypeDef",
-    {
-        "AliasPrefix": str,
-        "Type": ContactTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
-    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-):
-    pass
-
-_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
-    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
-    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
-):
-    pass
-
-_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "EngagementId": str,
-    },
-)
-_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
-    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-):
-    pass
-
-_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
-    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-):
-    pass
-
-_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
-    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-):
-    pass
-
-ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
-    "ListRotationsRequestListRotationsPaginateTypeDef",
-    {
-        "RotationNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     {
         "IncidentId": str,
         "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEngagementsRequestRequestTypeDef = TypedDict(
     "ListEngagementsRequestRequestTypeDef",
     {
@@ -1171,51 +1171,51 @@
 )
 
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPageResolutionsResultTypeDef = TypedDict(
     "ListPageResolutionsResultTypeDef",
     {
         "NextToken": str,
         "PageResolutions": List[ResolutionContactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPagesByContactResultTypeDef = TypedDict(
     "ListPagesByContactResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPagesByEngagementResultTypeDef = TypedDict(
     "ListPagesByEngagementResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRotationOverridesResultTypeDef = TypedDict(
     "ListRotationOverridesResultTypeDef",
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
@@ -1236,15 +1236,15 @@
     pass
 
 ListContactChannelsResultTypeDef = TypedDict(
     "ListContactChannelsResultTypeDef",
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
@@ -1276,24 +1276,24 @@
     pass
 
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRotationShiftsResultTypeDef = TypedDict(
     "ListRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
@@ -1331,15 +1331,15 @@
     {
         "RotationArn": str,
         "Name": str,
         "ContactIds": List[str],
         "StartTime": datetime,
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "EndTime": Union[datetime, str],
@@ -1350,15 +1350,15 @@
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "RotationStartTime": Union[datetime, str],
         "StartTime": Union[datetime, str],
         "Overrides": Sequence[PreviewOverrideTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
     _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
@@ -1462,15 +1462,15 @@
     "GetContactResultTypeDef",
     {
         "ContactArn": str,
         "Alias": str,
         "DisplayName": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
@@ -1491,10 +1491,10 @@
     pass
 
 ListRotationsResultTypeDef = TypedDict(
     "ListRotationsResultTypeDef",
     {
         "NextToken": str,
         "Rotations": List[RotationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/PKG-INFO` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.26.101
-Summary: Type annotations for boto3.SSMContacts 1.26.101 service generated with mypy-boto3-builder 7.14.4
+Version: 1.27.0
+Summary: Type annotations for boto3.SSMContacts 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-contacts?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.26.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,14 +356,15 @@
     ListRotationsPaginatorName,
     ReceiptTypeType,
     ShiftTypeType,
     SSMContactsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
+    RegionName,
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
@@ -379,83 +380,83 @@
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateContactChannelResultTypeDef,
     TagTypeDef,
+    CreateContactResultTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
+    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
+    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
+    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
+    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactChannelsRequestRequestTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
     TimeRangeTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutContactPolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
+    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
+    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
     TargetTypeDef,
+    ListContactsResultTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
-    CreateContactChannelResultTypeDef,
-    CreateContactResultTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
-    DescribeEngagementResultTypeDef,
-    DescribePageResultTypeDef,
-    GetContactChannelResultTypeDef,
-    GetContactPolicyResultTypeDef,
-    GetRotationOverrideResultTypeDef,
-    ListContactsResultTypeDef,
-    StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
```

### Comparing `mypy-boto3-ssm-contacts-1.26.101/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt` & `mypy-boto3-ssm-contacts-1.27.0/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.26.101/setup.py` & `mypy-boto3-ssm-contacts-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-contacts",
-    version="1.26.101",
+    version="1.27.0",
     packages=["mypy_boto3_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMContacts 1.26.101 service generated with mypy-boto3-builder"
-        " 7.14.4"
+        "Type annotations for boto3.SSMContacts 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


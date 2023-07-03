# Comparing `tmp/mypy-boto3-identitystore-1.26.107.tar.gz` & `tmp/mypy-boto3-identitystore-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-identitystore-1.26.107.tar", last modified: Wed Apr  5 20:26:18 2023, max compression
+gzip compressed data, was "mypy-boto3-identitystore-1.27.0.tar", last modified: Mon Jul  3 19:50:51 2023, max compression
```

## Comparing `mypy-boto3-identitystore-1.26.107.tar` & `mypy-boto3-identitystore-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:18.838361 mypy-boto3-identitystore-1.26.107/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-04-05 20:26:18.838361 mypy-boto3-identitystore-1.26.107/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:18.838361 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19209 2023-04-05 20:25:57.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 20:26:18.838361 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-04-05 20:26:18.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-05 20:26:18.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:26:18.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 20:26:18.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-05 20:26:18.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-05 20:26:18.000000 mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 20:26:18.838361 mypy-boto3-identitystore-1.26.107/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-05 20:25:56.000000 mypy-boto3-identitystore-1.26.107/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:51.803384 mypy-boto3-identitystore-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-03 19:50:51.803384 mypy-boto3-identitystore-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:51.803384 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-03 19:39:03.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-07-03 19:39:03.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-07-03 19:39:03.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:51.803384 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-03 19:50:51.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:50:51.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:51.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:51.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:51.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:50:51.000000 mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:51.803384 mypy-boto3-identitystore-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:39:02.000000 mypy-boto3-identitystore-1.27.0/setup.py
```

### Comparing `mypy-boto3-identitystore-1.26.107/LICENSE` & `mypy-boto3-identitystore-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.26.107/PKG-INFO` & `mypy-boto3-identitystore-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-identitystore
-Version: 1.26.107
-Summary: Type annotations for boto3.IdentityStore 1.26.107 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.IdentityStore 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-identitystore?color=blue)](https://pypistats.org/packages/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.26.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,55 +339,55 @@
 ```python
 from mypy_boto3_identitystore.type_defs import (
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    ResponseMetadataTypeDef,
+    CreateGroupMembershipResponseTypeDef,
     CreateGroupRequestRequestTypeDef,
+    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
+    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
     DescribeGroupRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupMembershipsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeGroupResponseTypeDef,
     GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
     GroupMembershipExistenceResultTypeDef,
     GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
-    CreateGroupMembershipResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateUserResponseTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
-    DescribeGroupResponseTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestRequestTypeDef,
-    ListUsersRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
+    ListGroupsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
+    ListUsersRequestRequestTypeDef,
     ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListUsersResponseTypeDef,
```

### Comparing `mypy-boto3-identitystore-1.26.107/README.md` & `mypy-boto3-identitystore-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-identitystore?color=blue)](https://pypistats.org/packages/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.26.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -307,55 +307,55 @@
 ```python
 from mypy_boto3_identitystore.type_defs import (
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    ResponseMetadataTypeDef,
+    CreateGroupMembershipResponseTypeDef,
     CreateGroupRequestRequestTypeDef,
+    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
+    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
     DescribeGroupRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupMembershipsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeGroupResponseTypeDef,
     GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
     GroupMembershipExistenceResultTypeDef,
     GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
-    CreateGroupMembershipResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateUserResponseTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
-    DescribeGroupResponseTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestRequestTypeDef,
-    ListUsersRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
+    ListGroupsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
+    ListUsersRequestRequestTypeDef,
     ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListUsersResponseTypeDef,
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/__init__.py` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/__init__.pyi` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/__main__.py` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IdentityStore 1.26.107\nVersion:         1.26.107\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IdentityStore 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.107")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/client.py` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/client.pyi` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/literals.py` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListGroupMembershipsForMemberPaginatorName",
     "ListGroupMembershipsPaginatorName",
     "ListGroupsPaginatorName",
     "ListUsersPaginatorName",
     "IdentityStoreServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListGroupMembershipsForMemberPaginatorName = Literal["list_group_memberships_for_member"]
 ListGroupMembershipsPaginatorName = Literal["list_group_memberships"]
 ListGroupsPaginatorName = Literal["list_groups"]
 ListUsersPaginatorName = Literal["list_users"]
 IdentityStoreServiceName = Literal["identitystore"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -48,14 +46,15 @@
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
@@ -95,14 +94,15 @@
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
@@ -244,14 +244,15 @@
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
@@ -270,16 +271,19 @@
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
@@ -363,14 +367,15 @@
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
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/literals.pyi` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListGroupMembershipsForMemberPaginatorName",
     "ListGroupMembershipsPaginatorName",
     "ListGroupsPaginatorName",
     "ListUsersPaginatorName",
     "IdentityStoreServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListGroupMembershipsForMemberPaginatorName = Literal["list_group_memberships_for_member"]
 ListGroupMembershipsPaginatorName = Literal["list_group_memberships"]
 ListGroupsPaginatorName = Literal["list_groups"]
 ListUsersPaginatorName = Literal["list_users"]
 IdentityStoreServiceName = Literal["identitystore"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -46,14 +48,15 @@
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
@@ -93,14 +96,15 @@
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
@@ -242,14 +246,15 @@
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
@@ -268,16 +273,19 @@
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
@@ -361,14 +369,15 @@
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
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/paginator.py` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,19 @@
 class ListGroupMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
     """
 
     def paginate(
-        self, *, IdentityStoreId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        IdentityStoreId: str,
+        GroupId: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
         """
 
 
@@ -79,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         MemberId: MemberIdTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupMembershipsForMemberResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipsformemberpaginator)
         """
 
 
@@ -98,15 +102,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupspaginator)
         """
 
 
@@ -117,13 +121,13 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/paginator.pyi` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,19 @@
 class ListGroupMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
     """
 
     def paginate(
-        self, *, IdentityStoreId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        IdentityStoreId: str,
+        GroupId: str,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
         """
 
 class ListGroupMembershipsForMemberPaginator(Paginator):
@@ -75,15 +79,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         MemberId: MemberIdTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupMembershipsForMemberResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipsformemberpaginator)
         """
 
 class ListGroupsPaginator(Paginator):
@@ -93,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupspaginator)
         """
 
 class ListUsersPaginator(Paginator):
@@ -111,13 +115,13 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/type_defs.py` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,55 +22,55 @@
 
 __all__ = (
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateGroupMembershipResponseTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "CreateGroupResponseTypeDef",
     "EmailTypeDef",
     "NameTypeDef",
     "PhoneNumberTypeDef",
+    "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
     "DescribeGroupRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetGroupIdResponseTypeDef",
+    "GetGroupMembershipIdResponseTypeDef",
+    "GetUserIdResponseTypeDef",
+    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     "ListGroupMembershipsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "DescribeGroupResponseTypeDef",
     "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
+    "DescribeGroupMembershipResponseTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
     "GroupMembershipExistenceResultTypeDef",
     "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
+    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
-    "CreateGroupMembershipResponseTypeDef",
-    "CreateGroupResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "DescribeGroupMembershipResponseTypeDef",
-    "DescribeGroupResponseTypeDef",
-    "GetGroupIdResponseTypeDef",
-    "GetGroupMembershipIdResponseTypeDef",
-    "GetUserIdResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
-    "ListGroupsRequestRequestTypeDef",
-    "ListUsersRequestRequestTypeDef",
-    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListGroupsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
+    "ListUsersRequestRequestTypeDef",
     "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -132,22 +132,20 @@
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateGroupMembershipResponseTypeDef = TypedDict(
+    "CreateGroupMembershipResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -165,14 +163,23 @@
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
 
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EmailTypeDef = TypedDict(
     "EmailTypeDef",
     {
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
@@ -198,14 +205,23 @@
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
     total=False,
 )
 
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGroupMembershipRequestRequestTypeDef = TypedDict(
     "DeleteGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
@@ -254,24 +270,64 @@
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetGroupIdResponseTypeDef = TypedDict(
+    "GetGroupIdResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetGroupMembershipIdResponseTypeDef = TypedDict(
+    "GetGroupMembershipIdResponseTypeDef",
+    {
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetUserIdResponseTypeDef = TypedDict(
+    "GetUserIdResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "IdentityStoreId": str,
+        "GroupId": str,
+    },
+)
+_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
+    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -288,14 +344,47 @@
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
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
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGroupTypeDef = TypedDict(
     "_RequiredGroupTypeDef",
     {
         "GroupId": str,
         "IdentityStoreId": str,
     },
 )
@@ -346,14 +435,25 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
+DescribeGroupMembershipResponseTypeDef = TypedDict(
+    "DescribeGroupMembershipResponseTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupMembershipIdRequestRequestTypeDef = TypedDict(
     "GetGroupMembershipIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
@@ -395,14 +495,41 @@
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
         "GroupIds": Sequence[str],
     },
 )
 
+_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "IdentityStoreId": str,
+            "MemberId": MemberIdTypeDef,
+        },
+    )
+)
+_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+
+class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
+    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -419,91 +546,14 @@
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
 
-CreateGroupMembershipResponseTypeDef = TypedDict(
-    "CreateGroupMembershipResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGroupMembershipResponseTypeDef = TypedDict(
-    "DescribeGroupMembershipResponseTypeDef",
-    {
-        "IdentityStoreId": str,
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupIdResponseTypeDef = TypedDict(
-    "GetGroupIdResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupMembershipIdResponseTypeDef = TypedDict(
-    "GetGroupMembershipIdResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUserIdResponseTypeDef = TypedDict(
-    "GetUserIdResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -548,15 +598,15 @@
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "UserId": str,
@@ -585,162 +635,112 @@
 )
 
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 
-_RequiredListGroupsRequestRequestTypeDef = TypedDict(
-    "_RequiredListGroupsRequestRequestTypeDef",
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestRequestTypeDef = TypedDict(
-    "_OptionalListGroupsRequestRequestTypeDef",
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListGroupsRequestRequestTypeDef(
-    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListUsersRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsersRequestRequestTypeDef",
+_RequiredListGroupsRequestRequestTypeDef = TypedDict(
+    "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsersRequestRequestTypeDef",
+_OptionalListGroupsRequestRequestTypeDef = TypedDict(
+    "_OptionalListGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 
-class ListUsersRequestRequestTypeDef(
-    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "IdentityStoreId": str,
-            "MemberId": MemberIdTypeDef,
-        },
-    )
-)
-_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-
-class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
-    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "IdentityStoreId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
-    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+class ListGroupsRequestRequestTypeDef(
+    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -756,37 +756,37 @@
     },
 )
 
 IsMemberInGroupsResponseTypeDef = TypedDict(
     "IsMemberInGroupsResponseTypeDef",
     {
         "Results": List[GroupMembershipExistenceResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupMembershipsForMemberResponseTypeDef = TypedDict(
     "ListGroupMembershipsForMemberResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
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
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore/type_defs.pyi` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -21,55 +21,55 @@
 
 __all__ = (
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateGroupMembershipResponseTypeDef",
     "CreateGroupRequestRequestTypeDef",
+    "CreateGroupResponseTypeDef",
     "EmailTypeDef",
     "NameTypeDef",
     "PhoneNumberTypeDef",
+    "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
     "DescribeGroupRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetGroupIdResponseTypeDef",
+    "GetGroupMembershipIdResponseTypeDef",
+    "GetUserIdResponseTypeDef",
+    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     "ListGroupMembershipsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "DescribeGroupResponseTypeDef",
     "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
+    "DescribeGroupMembershipResponseTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
     "GroupMembershipExistenceResultTypeDef",
     "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
+    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
-    "CreateGroupMembershipResponseTypeDef",
-    "CreateGroupResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "DescribeGroupMembershipResponseTypeDef",
-    "DescribeGroupResponseTypeDef",
-    "GetGroupIdResponseTypeDef",
-    "GetGroupMembershipIdResponseTypeDef",
-    "GetUserIdResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
-    "ListGroupsRequestRequestTypeDef",
-    "ListUsersRequestRequestTypeDef",
-    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListGroupsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
+    "ListUsersRequestRequestTypeDef",
     "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -129,22 +129,20 @@
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateGroupMembershipResponseTypeDef = TypedDict(
+    "CreateGroupMembershipResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -160,14 +158,23 @@
 )
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EmailTypeDef = TypedDict(
     "EmailTypeDef",
     {
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
@@ -193,14 +200,23 @@
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
     total=False,
 )
 
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGroupMembershipRequestRequestTypeDef = TypedDict(
     "DeleteGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
@@ -249,24 +265,62 @@
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetGroupIdResponseTypeDef = TypedDict(
+    "GetGroupIdResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetGroupMembershipIdResponseTypeDef = TypedDict(
+    "GetGroupMembershipIdResponseTypeDef",
+    {
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetUserIdResponseTypeDef = TypedDict(
+    "GetUserIdResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "IdentityStoreId": str,
+        "GroupId": str,
+    },
+)
+_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
+    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+):
+    pass
+
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -281,14 +335,47 @@
 
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
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
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGroupTypeDef = TypedDict(
     "_RequiredGroupTypeDef",
     {
         "GroupId": str,
         "IdentityStoreId": str,
     },
 )
@@ -337,14 +424,25 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
+DescribeGroupMembershipResponseTypeDef = TypedDict(
+    "DescribeGroupMembershipResponseTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetGroupMembershipIdRequestRequestTypeDef = TypedDict(
     "GetGroupMembershipIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
@@ -384,14 +482,39 @@
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
         "GroupIds": Sequence[str],
     },
 )
 
+_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "IdentityStoreId": str,
+            "MemberId": MemberIdTypeDef,
+        },
+    )
+)
+_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
+    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+):
+    pass
+
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -406,91 +529,14 @@
 
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
-CreateGroupMembershipResponseTypeDef = TypedDict(
-    "CreateGroupMembershipResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGroupMembershipResponseTypeDef = TypedDict(
-    "DescribeGroupMembershipResponseTypeDef",
-    {
-        "IdentityStoreId": str,
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupIdResponseTypeDef = TypedDict(
-    "GetGroupIdResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupMembershipIdResponseTypeDef = TypedDict(
-    "GetGroupMembershipIdResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUserIdResponseTypeDef = TypedDict(
-    "GetUserIdResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -533,15 +579,15 @@
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "UserId": str,
@@ -568,150 +614,104 @@
     },
     total=False,
 )
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-_RequiredListGroupsRequestRequestTypeDef = TypedDict(
-    "_RequiredListGroupsRequestRequestTypeDef",
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestRequestTypeDef = TypedDict(
-    "_OptionalListGroupsRequestRequestTypeDef",
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListGroupsRequestRequestTypeDef(
-    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
-_RequiredListUsersRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsersRequestRequestTypeDef",
+_RequiredListGroupsRequestRequestTypeDef = TypedDict(
+    "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsersRequestRequestTypeDef",
+_OptionalListGroupsRequestRequestTypeDef = TypedDict(
+    "_OptionalListGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class ListUsersRequestRequestTypeDef(
-    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
-):
-    pass
-
-_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "IdentityStoreId": str,
-            "MemberId": MemberIdTypeDef,
-        },
-    )
-)
-_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
-    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-):
-    pass
-
-_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "IdentityStoreId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
-    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+class ListGroupsRequestRequestTypeDef(
+    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -727,37 +727,37 @@
     },
 )
 
 IsMemberInGroupsResponseTypeDef = TypedDict(
     "IsMemberInGroupsResponseTypeDef",
     {
         "Results": List[GroupMembershipExistenceResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupMembershipsForMemberResponseTypeDef = TypedDict(
     "ListGroupMembershipsForMemberResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
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
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/PKG-INFO` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-identitystore
-Version: 1.26.107
-Summary: Type annotations for boto3.IdentityStore 1.26.107 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.IdentityStore 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-identitystore?color=blue)](https://pypistats.org/packages/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.26.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,55 +339,55 @@
 ```python
 from mypy_boto3_identitystore.type_defs import (
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    ResponseMetadataTypeDef,
+    CreateGroupMembershipResponseTypeDef,
     CreateGroupRequestRequestTypeDef,
+    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
+    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
     DescribeGroupRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupMembershipsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    DescribeGroupResponseTypeDef,
     GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
     GroupMembershipExistenceResultTypeDef,
     GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
-    CreateGroupMembershipResponseTypeDef,
-    CreateGroupResponseTypeDef,
-    CreateUserResponseTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
-    DescribeGroupResponseTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestRequestTypeDef,
-    ListUsersRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
+    ListGroupsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
+    ListUsersRequestRequestTypeDef,
     ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListUsersResponseTypeDef,
```

### Comparing `mypy-boto3-identitystore-1.26.107/mypy_boto3_identitystore.egg-info/SOURCES.txt` & `mypy-boto3-identitystore-1.27.0/mypy_boto3_identitystore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.26.107/setup.py` & `mypy-boto3-identitystore-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-identitystore",
-    version="1.26.107",
+    version="1.27.0",
     packages=["mypy_boto3_identitystore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IdentityStore 1.26.107 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IdentityStore 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


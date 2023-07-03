# Comparing `tmp/mypy-boto3-workspaces-web-1.26.46.tar.gz` & `tmp/mypy-boto3-workspaces-web-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-web-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-web-1.27.0.tar", last modified: Mon Jul  3 19:51:37 2023, max compression
```

## Comparing `mypy-boto3-workspaces-web-1.26.46.tar` & `mypy-boto3-workspaces-web-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.332431 mypy-boto3-workspaces-web-1.26.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-01-09 20:27:39.324432 mypy-boto3-workspaces-web-1.26.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.324432 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33661 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36104 2023-01-09 20:27:31.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.324432 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-01-09 20:27:39.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-09 20:27:39.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-09 20:27:39.000000 mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.332431 mypy-boto3-workspaces-web-1.26.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-09 20:27:30.000000 mypy-boto3-workspaces-web-1.26.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.608168 mypy-boto3-workspaces-web-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-03 19:51:37.608168 mypy-boto3-workspaces-web-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.608168 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37970 2023-07-03 19:49:57.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37906 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-03 19:49:57.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-03 19:49:57.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41390 2023-07-03 19:49:57.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41339 2023-07-03 19:49:57.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:37.608168 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:37.000000 mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:37.608168 mypy-boto3-workspaces-web-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:49:56.000000 mypy-boto3-workspaces-web-1.27.0/setup.py
```

### Comparing `mypy-boto3-workspaces-web-1.26.46/LICENSE` & `mypy-boto3-workspaces-web-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-workspaces-web-1.26.46/PKG-INFO` & `mypy-boto3-workspaces-web-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.26.46
-Summary: Type annotations for boto3.WorkSpacesWeb 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkSpacesWeb 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces-web?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,161 +304,176 @@
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsRequestRequestTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
+    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
+    AssociateUserSettingsResponseTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    IpRuleTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
+    DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
     DeleteUserSettingsRequestRequestTypeDef,
     DisassociateBrowserSettingsRequestRequestTypeDef,
+    DisassociateIpAccessSettingsRequestRequestTypeDef,
     DisassociateNetworkSettingsRequestRequestTypeDef,
     DisassociateTrustStoreRequestRequestTypeDef,
     DisassociateUserAccessLoggingSettingsRequestRequestTypeDef,
     DisassociateUserSettingsRequestRequestTypeDef,
     GetBrowserSettingsRequestRequestTypeDef,
     GetIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeDef,
+    GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
+    IpAccessSettingsSummaryTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
+    ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
     UpdateTrustStoreRequestRequestTypeDef,
+    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
-    AssociateTrustStoreResponseTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
-    AssociateUserSettingsResponseTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateIpAccessSettingsRequestRequestTypeDef,
+    IpAccessSettingsTypeDef,
+    UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
+    ListIpAccessSettingsResponseTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
+    GetIpAccessSettingsResponseTypeDef,
+    UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-workspaces-web-1.26.46/README.md` & `mypy-boto3-workspaces-web-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces-web?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,161 +272,176 @@
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsRequestRequestTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
+    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
+    AssociateUserSettingsResponseTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    IpRuleTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
+    DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
     DeleteUserSettingsRequestRequestTypeDef,
     DisassociateBrowserSettingsRequestRequestTypeDef,
+    DisassociateIpAccessSettingsRequestRequestTypeDef,
     DisassociateNetworkSettingsRequestRequestTypeDef,
     DisassociateTrustStoreRequestRequestTypeDef,
     DisassociateUserAccessLoggingSettingsRequestRequestTypeDef,
     DisassociateUserSettingsRequestRequestTypeDef,
     GetBrowserSettingsRequestRequestTypeDef,
     GetIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeDef,
+    GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
+    IpAccessSettingsSummaryTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
+    ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
     UpdateTrustStoreRequestRequestTypeDef,
+    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
-    AssociateTrustStoreResponseTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
-    AssociateUserSettingsResponseTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateIpAccessSettingsRequestRequestTypeDef,
+    IpAccessSettingsTypeDef,
+    UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
+    ListIpAccessSettingsResponseTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
+    GetIpAccessSettingsResponseTypeDef,
+    UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/__main__.py` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpacesWeb 1.26.46\nVersion:         1.26.46\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.WorkSpacesWeb 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.46")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/client.py` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,46 +17,52 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
     CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
     CreateUserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     GetIdentityProviderResponseTypeDef,
+    GetIpAccessSettingsResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
+    IpRuleTypeDef,
     ListBrowserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
+    ListIpAccessSettingsResponseTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     TagTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
+    UpdateIpAccessSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     UpdatePortalResponseTypeDef,
     UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
 )
 
@@ -106,14 +112,24 @@
         """
         Associates a browser settings resource with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_browser_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#associate_browser_settings)
         """
 
+    def associate_ip_access_settings(
+        self, *, ipAccessSettingsArn: str, portalArn: str
+    ) -> AssociateIpAccessSettingsResponseTypeDef:
+        """
+        Associates an IP access settings resource with a web portal.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#associate_ip_access_settings)
+        """
+
     def associate_network_settings(
         self, *, networkSettingsArn: str, portalArn: str
     ) -> AssociateNetworkSettingsResponseTypeDef:
         """
         Associates a network settings resource with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_network_settings)
@@ -194,14 +210,32 @@
         """
         Creates an identity provider resource that is then associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_identity_provider)
         """
 
+    def create_ip_access_settings(
+        self,
+        *,
+        ipRules: Sequence[IpRuleTypeDef],
+        additionalEncryptionContext: Mapping[str, str] = ...,
+        clientToken: str = ...,
+        customerManagedKey: str = ...,
+        description: str = ...,
+        displayName: str = ...,
+        tags: Sequence[TagTypeDef] = ...
+    ) -> CreateIpAccessSettingsResponseTypeDef:
+        """
+        Creates an IP access settings resource that can be associated with a web portal.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_ip_access_settings)
+        """
+
     def create_network_settings(
         self,
         *,
         securityGroupIds: Sequence[str],
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
@@ -288,14 +322,22 @@
         """
         Deletes the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#delete_identity_provider)
         """
 
+    def delete_ip_access_settings(self, *, ipAccessSettingsArn: str) -> Dict[str, Any]:
+        """
+        Deletes IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#delete_ip_access_settings)
+        """
+
     def delete_network_settings(self, *, networkSettingsArn: str) -> Dict[str, Any]:
         """
         Deletes network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#delete_network_settings)
         """
@@ -338,14 +380,22 @@
         """
         Disassociates browser settings from a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_browser_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#disassociate_browser_settings)
         """
 
+    def disassociate_ip_access_settings(self, *, portalArn: str) -> Dict[str, Any]:
+        """
+        Disassociates IP access settings from a web portal.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#disassociate_ip_access_settings)
+        """
+
     def disassociate_network_settings(self, *, portalArn: str) -> Dict[str, Any]:
         """
         Disassociates network settings from a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#disassociate_network_settings)
         """
@@ -402,14 +452,24 @@
         """
         Gets the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#get_identity_provider)
         """
 
+    def get_ip_access_settings(
+        self, *, ipAccessSettingsArn: str
+    ) -> GetIpAccessSettingsResponseTypeDef:
+        """
+        Gets the IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#get_ip_access_settings)
+        """
+
     def get_network_settings(self, *, networkSettingsArn: str) -> GetNetworkSettingsResponseTypeDef:
         """
         Gets the network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#get_network_settings)
         """
@@ -484,14 +544,24 @@
         """
         Retrieves a list of identity providers for a specific web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_identity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#list_identity_providers)
         """
 
+    def list_ip_access_settings(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListIpAccessSettingsResponseTypeDef:
+        """
+        Retrieves a list of IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#list_ip_access_settings)
+        """
+
     def list_network_settings(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListNetworkSettingsResponseTypeDef:
         """
         Retrieves a list of network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_network_settings)
@@ -596,14 +666,30 @@
         """
         Updates the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_identity_provider)
         """
 
+    def update_ip_access_settings(
+        self,
+        *,
+        ipAccessSettingsArn: str,
+        clientToken: str = ...,
+        description: str = ...,
+        displayName: str = ...,
+        ipRules: Sequence[IpRuleTypeDef] = ...
+    ) -> UpdateIpAccessSettingsResponseTypeDef:
+        """
+        Updates IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_ip_access_settings)
+        """
+
     def update_network_settings(
         self,
         *,
         networkSettingsArn: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
```

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/client.pyi` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -17,46 +17,52 @@
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
     CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
     CreateNetworkSettingsResponseTypeDef,
     CreatePortalResponseTypeDef,
     CreateTrustStoreResponseTypeDef,
     CreateUserAccessLoggingSettingsResponseTypeDef,
     CreateUserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     GetIdentityProviderResponseTypeDef,
+    GetIpAccessSettingsResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
+    IpRuleTypeDef,
     ListBrowserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
+    ListIpAccessSettingsResponseTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     TagTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
+    UpdateIpAccessSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     UpdatePortalResponseTypeDef,
     UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
 )
 
@@ -101,14 +107,23 @@
     ) -> AssociateBrowserSettingsResponseTypeDef:
         """
         Associates a browser settings resource with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_browser_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#associate_browser_settings)
         """
+    def associate_ip_access_settings(
+        self, *, ipAccessSettingsArn: str, portalArn: str
+    ) -> AssociateIpAccessSettingsResponseTypeDef:
+        """
+        Associates an IP access settings resource with a web portal.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#associate_ip_access_settings)
+        """
     def associate_network_settings(
         self, *, networkSettingsArn: str, portalArn: str
     ) -> AssociateNetworkSettingsResponseTypeDef:
         """
         Associates a network settings resource with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.associate_network_settings)
@@ -181,14 +196,31 @@
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an identity provider resource that is then associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_identity_provider)
         """
+    def create_ip_access_settings(
+        self,
+        *,
+        ipRules: Sequence[IpRuleTypeDef],
+        additionalEncryptionContext: Mapping[str, str] = ...,
+        clientToken: str = ...,
+        customerManagedKey: str = ...,
+        description: str = ...,
+        displayName: str = ...,
+        tags: Sequence[TagTypeDef] = ...
+    ) -> CreateIpAccessSettingsResponseTypeDef:
+        """
+        Creates an IP access settings resource that can be associated with a web portal.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_ip_access_settings)
+        """
     def create_network_settings(
         self,
         *,
         securityGroupIds: Sequence[str],
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
@@ -268,14 +300,21 @@
     def delete_identity_provider(self, *, identityProviderArn: str) -> Dict[str, Any]:
         """
         Deletes the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#delete_identity_provider)
         """
+    def delete_ip_access_settings(self, *, ipAccessSettingsArn: str) -> Dict[str, Any]:
+        """
+        Deletes IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#delete_ip_access_settings)
+        """
     def delete_network_settings(self, *, networkSettingsArn: str) -> Dict[str, Any]:
         """
         Deletes network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.delete_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#delete_network_settings)
         """
@@ -312,14 +351,21 @@
     def disassociate_browser_settings(self, *, portalArn: str) -> Dict[str, Any]:
         """
         Disassociates browser settings from a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_browser_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#disassociate_browser_settings)
         """
+    def disassociate_ip_access_settings(self, *, portalArn: str) -> Dict[str, Any]:
+        """
+        Disassociates IP access settings from a web portal.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#disassociate_ip_access_settings)
+        """
     def disassociate_network_settings(self, *, portalArn: str) -> Dict[str, Any]:
         """
         Disassociates network settings from a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.disassociate_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#disassociate_network_settings)
         """
@@ -369,14 +415,23 @@
     ) -> GetIdentityProviderResponseTypeDef:
         """
         Gets the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#get_identity_provider)
         """
+    def get_ip_access_settings(
+        self, *, ipAccessSettingsArn: str
+    ) -> GetIpAccessSettingsResponseTypeDef:
+        """
+        Gets the IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#get_ip_access_settings)
+        """
     def get_network_settings(self, *, networkSettingsArn: str) -> GetNetworkSettingsResponseTypeDef:
         """
         Gets the network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.get_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#get_network_settings)
         """
@@ -442,14 +497,23 @@
     ) -> ListIdentityProvidersResponseTypeDef:
         """
         Retrieves a list of identity providers for a specific web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_identity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#list_identity_providers)
         """
+    def list_ip_access_settings(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListIpAccessSettingsResponseTypeDef:
+        """
+        Retrieves a list of IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#list_ip_access_settings)
+        """
     def list_network_settings(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListNetworkSettingsResponseTypeDef:
         """
         Retrieves a list of network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.list_network_settings)
@@ -543,14 +607,29 @@
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_identity_provider)
         """
+    def update_ip_access_settings(
+        self,
+        *,
+        ipAccessSettingsArn: str,
+        clientToken: str = ...,
+        description: str = ...,
+        displayName: str = ...,
+        ipRules: Sequence[IpRuleTypeDef] = ...
+    ) -> UpdateIpAccessSettingsResponseTypeDef:
+        """
+        Updates IP access settings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_ip_access_settings)
+        """
     def update_network_settings(
         self,
         *,
         networkSettingsArn: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
```

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/literals.py` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
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
@@ -81,31 +82,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -184,14 +188,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -202,14 +207,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
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
@@ -360,18 +370,21 @@
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

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/literals.pyi` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
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
@@ -79,31 +80,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -182,14 +186,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -200,14 +205,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -243,14 +249,15 @@
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
@@ -269,16 +276,19 @@
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
@@ -358,18 +368,21 @@
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

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/type_defs.py` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,172 +32,238 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateBrowserSettingsResponseTypeDef",
+    "AssociateIpAccessSettingsRequestRequestTypeDef",
+    "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
+    "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
+    "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
+    "AssociateUserSettingsResponseTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
+    "CreateBrowserSettingsResponseTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "IpRuleTypeDef",
+    "CreateIpAccessSettingsResponseTypeDef",
+    "CreateNetworkSettingsResponseTypeDef",
+    "CreatePortalResponseTypeDef",
+    "CreateTrustStoreResponseTypeDef",
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    "CreateUserSettingsResponseTypeDef",
     "DeleteBrowserSettingsRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
+    "DeleteIpAccessSettingsRequestRequestTypeDef",
     "DeleteNetworkSettingsRequestRequestTypeDef",
     "DeletePortalRequestRequestTypeDef",
     "DeleteTrustStoreRequestRequestTypeDef",
     "DeleteUserAccessLoggingSettingsRequestRequestTypeDef",
     "DeleteUserSettingsRequestRequestTypeDef",
     "DisassociateBrowserSettingsRequestRequestTypeDef",
+    "DisassociateIpAccessSettingsRequestRequestTypeDef",
     "DisassociateNetworkSettingsRequestRequestTypeDef",
     "DisassociateTrustStoreRequestRequestTypeDef",
     "DisassociateUserAccessLoggingSettingsRequestRequestTypeDef",
     "DisassociateUserSettingsRequestRequestTypeDef",
     "GetBrowserSettingsRequestRequestTypeDef",
     "GetIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeDef",
+    "GetIpAccessSettingsRequestRequestTypeDef",
     "GetNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsTypeDef",
     "GetPortalRequestRequestTypeDef",
     "PortalTypeDef",
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
+    "GetPortalServiceProviderMetadataResponseTypeDef",
     "GetTrustStoreCertificateRequestRequestTypeDef",
     "GetTrustStoreRequestRequestTypeDef",
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
     "IdentityProviderSummaryTypeDef",
+    "IpAccessSettingsSummaryTypeDef",
     "ListBrowserSettingsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
+    "ListIpAccessSettingsRequestRequestTypeDef",
     "ListNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsSummaryTypeDef",
     "ListPortalsRequestRequestTypeDef",
     "PortalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
     "UpdateTrustStoreRequestRequestTypeDef",
+    "UpdateTrustStoreResponseTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "AssociateBrowserSettingsResponseTypeDef",
-    "AssociateNetworkSettingsResponseTypeDef",
-    "AssociateTrustStoreResponseTypeDef",
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    "AssociateUserSettingsResponseTypeDef",
-    "CreateBrowserSettingsResponseTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
-    "CreateNetworkSettingsResponseTypeDef",
-    "CreatePortalResponseTypeDef",
-    "CreateTrustStoreResponseTypeDef",
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    "CreateUserSettingsResponseTypeDef",
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    "UpdateTrustStoreResponseTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "CreateTrustStoreRequestRequestTypeDef",
     "CreateUserAccessLoggingSettingsRequestRequestTypeDef",
     "CreateUserSettingsRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateIpAccessSettingsRequestRequestTypeDef",
+    "IpAccessSettingsTypeDef",
+    "UpdateIpAccessSettingsRequestRequestTypeDef",
     "GetIdentityProviderResponseTypeDef",
     "UpdateIdentityProviderResponseTypeDef",
     "GetNetworkSettingsResponseTypeDef",
     "UpdateNetworkSettingsResponseTypeDef",
     "GetPortalResponseTypeDef",
     "UpdatePortalResponseTypeDef",
     "GetTrustStoreResponseTypeDef",
     "GetUserAccessLoggingSettingsResponseTypeDef",
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
+    "ListIpAccessSettingsResponseTypeDef",
     "ListNetworkSettingsResponseTypeDef",
     "ListPortalsResponseTypeDef",
     "ListTrustStoresResponseTypeDef",
     "ListUserAccessLoggingSettingsResponseTypeDef",
     "ListUserSettingsResponseTypeDef",
+    "GetIpAccessSettingsResponseTypeDef",
+    "UpdateIpAccessSettingsResponseTypeDef",
 )
 
 AssociateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateBrowserSettingsResponseTypeDef = TypedDict(
+    "AssociateBrowserSettingsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "browserSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "AssociateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+    },
+)
+
+AssociateIpAccessSettingsResponseTypeDef = TypedDict(
+    "AssociateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "AssociateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
         "portalArn": str,
     },
 )
 
+AssociateNetworkSettingsResponseTypeDef = TypedDict(
+    "AssociateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateTrustStoreRequestRequestTypeDef = TypedDict(
     "AssociateTrustStoreRequestRequestTypeDef",
     {
         "portalArn": str,
         "trustStoreArn": str,
     },
 )
 
+AssociateTrustStoreResponseTypeDef = TypedDict(
+    "AssociateTrustStoreResponseTypeDef",
+    {
+        "portalArn": str,
+        "trustStoreArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userAccessLoggingSettingsArn": str,
     },
 )
 
+AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateUserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
+AssociateUserSettingsResponseTypeDef = TypedDict(
+    "AssociateUserSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -251,14 +317,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateBrowserSettingsResponseTypeDef = TypedDict(
+    "CreateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
         "portalArn": str,
@@ -276,28 +350,111 @@
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
+    {
+        "identityProviderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredIpRuleTypeDef = TypedDict(
+    "_RequiredIpRuleTypeDef",
+    {
+        "ipRange": str,
+    },
+)
+_OptionalIpRuleTypeDef = TypedDict(
+    "_OptionalIpRuleTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
+    pass
+
+
+CreateIpAccessSettingsResponseTypeDef = TypedDict(
+    "CreateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateNetworkSettingsResponseTypeDef = TypedDict(
+    "CreateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePortalResponseTypeDef = TypedDict(
+    "CreatePortalResponseTypeDef",
+    {
+        "portalArn": str,
+        "portalEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTrustStoreResponseTypeDef = TypedDict(
+    "CreateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateUserSettingsResponseTypeDef = TypedDict(
+    "CreateUserSettingsResponseTypeDef",
+    {
+        "userSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
 DeleteIdentityProviderRequestRequestTypeDef = TypedDict(
     "DeleteIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderArn": str,
     },
 )
 
+DeleteIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "DeleteIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+
 DeleteNetworkSettingsRequestRequestTypeDef = TypedDict(
     "DeleteNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 
@@ -332,14 +489,21 @@
 DisassociateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DisassociateBrowserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
+DisassociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "DisassociateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "portalArn": str,
+    },
+)
+
 DisassociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "DisassociateNetworkSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
@@ -395,14 +559,21 @@
 )
 
 
 class IdentityProviderTypeDef(_RequiredIdentityProviderTypeDef, _OptionalIdentityProviderTypeDef):
     pass
 
 
+GetIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "GetIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+
 GetNetworkSettingsRequestRequestTypeDef = TypedDict(
     "GetNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 
@@ -439,14 +610,15 @@
     "PortalTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
         "browserSettingsArn": str,
         "browserType": Literal["Chrome"],
         "creationDate": datetime,
         "displayName": str,
+        "ipAccessSettingsArn": str,
         "networkSettingsArn": str,
         "portalArn": str,
         "portalEndpoint": str,
         "portalStatus": PortalStatusType,
         "rendererType": Literal["AppStream"],
         "statusReason": str,
         "trustStoreArn": str,
@@ -459,14 +631,23 @@
 GetPortalServiceProviderMetadataRequestRequestTypeDef = TypedDict(
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
+GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    {
+        "portalArn": str,
+        "serviceProviderSamlMetadata": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTrustStoreCertificateRequestRequestTypeDef = TypedDict(
     "GetTrustStoreCertificateRequestRequestTypeDef",
     {
         "thumbprint": str,
         "trustStoreArn": str,
     },
 )
@@ -555,14 +736,25 @@
         "identityProviderArn": str,
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
+IpAccessSettingsSummaryTypeDef = TypedDict(
+    "IpAccessSettingsSummaryTypeDef",
+    {
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipAccessSettingsArn": str,
+    },
+    total=False,
+)
+
 ListBrowserSettingsRequestRequestTypeDef = TypedDict(
     "ListBrowserSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -587,14 +779,23 @@
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
 
+ListIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "ListIpAccessSettingsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 ListNetworkSettingsRequestRequestTypeDef = TypedDict(
     "ListNetworkSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -622,14 +823,15 @@
     "PortalSummaryTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
         "browserSettingsArn": str,
         "browserType": Literal["Chrome"],
         "creationDate": datetime,
         "displayName": str,
+        "ipAccessSettingsArn": str,
         "networkSettingsArn": str,
         "portalArn": str,
         "portalEndpoint": str,
         "portalStatus": PortalStatusType,
         "rendererType": Literal["AppStream"],
         "trustStoreArn": str,
         "userAccessLoggingSettingsArn": str,
@@ -723,14 +925,25 @@
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
         "userSettingsArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -849,14 +1062,22 @@
 
 class UpdateTrustStoreRequestRequestTypeDef(
     _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
 ):
     pass
 
 
+UpdateTrustStoreResponseTypeDef = TypedDict(
+    "UpdateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -901,174 +1122,55 @@
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateBrowserSettingsResponseTypeDef = TypedDict(
-    "AssociateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateNetworkSettingsResponseTypeDef = TypedDict(
-    "AssociateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateTrustStoreResponseTypeDef = TypedDict(
-    "AssociateTrustStoreResponseTypeDef",
-    {
-        "portalArn": str,
-        "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateUserSettingsResponseTypeDef = TypedDict(
-    "AssociateUserSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBrowserSettingsResponseTypeDef = TypedDict(
-    "CreateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
-    {
-        "identityProviderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNetworkSettingsResponseTypeDef = TypedDict(
-    "CreateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePortalResponseTypeDef = TypedDict(
-    "CreatePortalResponseTypeDef",
-    {
-        "portalArn": str,
-        "portalEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTrustStoreResponseTypeDef = TypedDict(
-    "CreateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserSettingsResponseTypeDef = TypedDict(
-    "CreateUserSettingsResponseTypeDef",
-    {
-        "userSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    {
-        "portalArn": str,
-        "serviceProviderSamlMetadata": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTrustStoreResponseTypeDef = TypedDict(
-    "UpdateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBrowserSettingsResponseTypeDef = TypedDict(
     "GetBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBrowserSettingsResponseTypeDef = TypedDict(
     "UpdateBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrustStoreCertificatesResponseTypeDef = TypedDict(
     "ListTrustStoreCertificatesResponseTypeDef",
     {
         "certificateList": List[CertificateSummaryTypeDef],
         "nextToken": str,
         "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrustStoreCertificateResponseTypeDef = TypedDict(
     "GetTrustStoreCertificateResponseTypeDef",
     {
         "certificate": CertificateTypeDef,
         "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrowserSettingsRequestRequestTypeDef",
     {
         "browserPolicy": str,
@@ -1205,15 +1307,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1231,148 +1333,248 @@
 
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipRules": Sequence[IpRuleTypeDef],
+    },
+)
+_OptionalCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "additionalEncryptionContext": Mapping[str, str],
+        "clientToken": str,
+        "customerManagedKey": str,
+        "description": str,
+        "displayName": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateIpAccessSettingsRequestRequestTypeDef(
+    _RequiredCreateIpAccessSettingsRequestRequestTypeDef,
+    _OptionalCreateIpAccessSettingsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredIpAccessSettingsTypeDef = TypedDict(
+    "_RequiredIpAccessSettingsTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalIpAccessSettingsTypeDef = TypedDict(
+    "_OptionalIpAccessSettingsTypeDef",
+    {
+        "associatedPortalArns": List[str],
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipRules": List[IpRuleTypeDef],
+    },
+    total=False,
+)
+
+
+class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
+    pass
+
+
+_RequiredUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "description": str,
+        "displayName": str,
+        "ipRules": Sequence[IpRuleTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateIpAccessSettingsRequestRequestTypeDef(
+    _RequiredUpdateIpAccessSettingsRequestRequestTypeDef,
+    _OptionalUpdateIpAccessSettingsRequestRequestTypeDef,
+):
+    pass
+
+
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkSettingsResponseTypeDef = TypedDict(
     "GetNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNetworkSettingsResponseTypeDef = TypedDict(
     "UpdateNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPortalResponseTypeDef = TypedDict(
     "GetPortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrustStoreResponseTypeDef = TypedDict(
     "GetTrustStoreResponseTypeDef",
     {
         "trustStore": TrustStoreTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "GetUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserSettingsResponseTypeDef = TypedDict(
     "UpdateUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "identityProviders": List[IdentityProviderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListIpAccessSettingsResponseTypeDef = TypedDict(
+    "ListIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "ListUserAccessLoggingSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userAccessLoggingSettings": List[UserAccessLoggingSettingsSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserSettingsResponseTypeDef = TypedDict(
     "ListUserSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userSettings": List[UserSettingsSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetIpAccessSettingsResponseTypeDef = TypedDict(
+    "GetIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettings": IpAccessSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateIpAccessSettingsResponseTypeDef = TypedDict(
+    "UpdateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettings": IpAccessSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web/type_defs.pyi` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -31,172 +31,238 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateBrowserSettingsResponseTypeDef",
+    "AssociateIpAccessSettingsRequestRequestTypeDef",
+    "AssociateIpAccessSettingsResponseTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
+    "AssociateNetworkSettingsResponseTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
+    "AssociateTrustStoreResponseTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
     "AssociateUserSettingsRequestRequestTypeDef",
+    "AssociateUserSettingsResponseTypeDef",
     "BrowserSettingsSummaryTypeDef",
     "BrowserSettingsTypeDef",
     "CertificateSummaryTypeDef",
     "CertificateTypeDef",
     "TagTypeDef",
+    "CreateBrowserSettingsResponseTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "IpRuleTypeDef",
+    "CreateIpAccessSettingsResponseTypeDef",
+    "CreateNetworkSettingsResponseTypeDef",
+    "CreatePortalResponseTypeDef",
+    "CreateTrustStoreResponseTypeDef",
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    "CreateUserSettingsResponseTypeDef",
     "DeleteBrowserSettingsRequestRequestTypeDef",
     "DeleteIdentityProviderRequestRequestTypeDef",
+    "DeleteIpAccessSettingsRequestRequestTypeDef",
     "DeleteNetworkSettingsRequestRequestTypeDef",
     "DeletePortalRequestRequestTypeDef",
     "DeleteTrustStoreRequestRequestTypeDef",
     "DeleteUserAccessLoggingSettingsRequestRequestTypeDef",
     "DeleteUserSettingsRequestRequestTypeDef",
     "DisassociateBrowserSettingsRequestRequestTypeDef",
+    "DisassociateIpAccessSettingsRequestRequestTypeDef",
     "DisassociateNetworkSettingsRequestRequestTypeDef",
     "DisassociateTrustStoreRequestRequestTypeDef",
     "DisassociateUserAccessLoggingSettingsRequestRequestTypeDef",
     "DisassociateUserSettingsRequestRequestTypeDef",
     "GetBrowserSettingsRequestRequestTypeDef",
     "GetIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeDef",
+    "GetIpAccessSettingsRequestRequestTypeDef",
     "GetNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsTypeDef",
     "GetPortalRequestRequestTypeDef",
     "PortalTypeDef",
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
+    "GetPortalServiceProviderMetadataResponseTypeDef",
     "GetTrustStoreCertificateRequestRequestTypeDef",
     "GetTrustStoreRequestRequestTypeDef",
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
     "IdentityProviderSummaryTypeDef",
+    "IpAccessSettingsSummaryTypeDef",
     "ListBrowserSettingsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
+    "ListIpAccessSettingsRequestRequestTypeDef",
     "ListNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsSummaryTypeDef",
     "ListPortalsRequestRequestTypeDef",
     "PortalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrowserSettingsRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
     "UpdateNetworkSettingsRequestRequestTypeDef",
     "UpdatePortalRequestRequestTypeDef",
     "UpdateTrustStoreRequestRequestTypeDef",
+    "UpdateTrustStoreResponseTypeDef",
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "AssociateBrowserSettingsResponseTypeDef",
-    "AssociateNetworkSettingsResponseTypeDef",
-    "AssociateTrustStoreResponseTypeDef",
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    "AssociateUserSettingsResponseTypeDef",
-    "CreateBrowserSettingsResponseTypeDef",
-    "CreateIdentityProviderResponseTypeDef",
-    "CreateNetworkSettingsResponseTypeDef",
-    "CreatePortalResponseTypeDef",
-    "CreateTrustStoreResponseTypeDef",
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    "CreateUserSettingsResponseTypeDef",
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    "UpdateTrustStoreResponseTypeDef",
     "ListBrowserSettingsResponseTypeDef",
     "GetBrowserSettingsResponseTypeDef",
     "UpdateBrowserSettingsResponseTypeDef",
     "ListTrustStoreCertificatesResponseTypeDef",
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "CreateTrustStoreRequestRequestTypeDef",
     "CreateUserAccessLoggingSettingsRequestRequestTypeDef",
     "CreateUserSettingsRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateIpAccessSettingsRequestRequestTypeDef",
+    "IpAccessSettingsTypeDef",
+    "UpdateIpAccessSettingsRequestRequestTypeDef",
     "GetIdentityProviderResponseTypeDef",
     "UpdateIdentityProviderResponseTypeDef",
     "GetNetworkSettingsResponseTypeDef",
     "UpdateNetworkSettingsResponseTypeDef",
     "GetPortalResponseTypeDef",
     "UpdatePortalResponseTypeDef",
     "GetTrustStoreResponseTypeDef",
     "GetUserAccessLoggingSettingsResponseTypeDef",
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
+    "ListIpAccessSettingsResponseTypeDef",
     "ListNetworkSettingsResponseTypeDef",
     "ListPortalsResponseTypeDef",
     "ListTrustStoresResponseTypeDef",
     "ListUserAccessLoggingSettingsResponseTypeDef",
     "ListUserSettingsResponseTypeDef",
+    "GetIpAccessSettingsResponseTypeDef",
+    "UpdateIpAccessSettingsResponseTypeDef",
 )
 
 AssociateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateBrowserSettingsResponseTypeDef = TypedDict(
+    "AssociateBrowserSettingsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "browserSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "AssociateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+    },
+)
+
+AssociateIpAccessSettingsResponseTypeDef = TypedDict(
+    "AssociateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "AssociateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
         "portalArn": str,
     },
 )
 
+AssociateNetworkSettingsResponseTypeDef = TypedDict(
+    "AssociateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "portalArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateTrustStoreRequestRequestTypeDef = TypedDict(
     "AssociateTrustStoreRequestRequestTypeDef",
     {
         "portalArn": str,
         "trustStoreArn": str,
     },
 )
 
+AssociateTrustStoreResponseTypeDef = TypedDict(
+    "AssociateTrustStoreResponseTypeDef",
+    {
+        "portalArn": str,
+        "trustStoreArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userAccessLoggingSettingsArn": str,
     },
 )
 
+AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "AssociateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateUserSettingsRequestRequestTypeDef = TypedDict(
     "AssociateUserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
         "userSettingsArn": str,
     },
 )
 
+AssociateUserSettingsResponseTypeDef = TypedDict(
+    "AssociateUserSettingsResponseTypeDef",
+    {
+        "portalArn": str,
+        "userSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BrowserSettingsSummaryTypeDef = TypedDict(
     "BrowserSettingsSummaryTypeDef",
     {
         "browserSettingsArn": str,
     },
     total=False,
 )
@@ -248,14 +314,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateBrowserSettingsResponseTypeDef = TypedDict(
+    "CreateBrowserSettingsResponseTypeDef",
+    {
+        "browserSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
         "portalArn": str,
@@ -271,28 +345,109 @@
 
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
+    {
+        "identityProviderArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredIpRuleTypeDef = TypedDict(
+    "_RequiredIpRuleTypeDef",
+    {
+        "ipRange": str,
+    },
+)
+_OptionalIpRuleTypeDef = TypedDict(
+    "_OptionalIpRuleTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
+    pass
+
+CreateIpAccessSettingsResponseTypeDef = TypedDict(
+    "CreateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateNetworkSettingsResponseTypeDef = TypedDict(
+    "CreateNetworkSettingsResponseTypeDef",
+    {
+        "networkSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePortalResponseTypeDef = TypedDict(
+    "CreatePortalResponseTypeDef",
+    {
+        "portalArn": str,
+        "portalEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTrustStoreResponseTypeDef = TypedDict(
+    "CreateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
+    "CreateUserAccessLoggingSettingsResponseTypeDef",
+    {
+        "userAccessLoggingSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateUserSettingsResponseTypeDef = TypedDict(
+    "CreateUserSettingsResponseTypeDef",
+    {
+        "userSettingsArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
 DeleteIdentityProviderRequestRequestTypeDef = TypedDict(
     "DeleteIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderArn": str,
     },
 )
 
+DeleteIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "DeleteIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+
 DeleteNetworkSettingsRequestRequestTypeDef = TypedDict(
     "DeleteNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 
@@ -327,14 +482,21 @@
 DisassociateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DisassociateBrowserSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
+DisassociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "DisassociateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "portalArn": str,
+    },
+)
+
 DisassociateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "DisassociateNetworkSettingsRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
@@ -388,14 +550,21 @@
     },
     total=False,
 )
 
 class IdentityProviderTypeDef(_RequiredIdentityProviderTypeDef, _OptionalIdentityProviderTypeDef):
     pass
 
+GetIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "GetIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+
 GetNetworkSettingsRequestRequestTypeDef = TypedDict(
     "GetNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 
@@ -430,14 +599,15 @@
     "PortalTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
         "browserSettingsArn": str,
         "browserType": Literal["Chrome"],
         "creationDate": datetime,
         "displayName": str,
+        "ipAccessSettingsArn": str,
         "networkSettingsArn": str,
         "portalArn": str,
         "portalEndpoint": str,
         "portalStatus": PortalStatusType,
         "rendererType": Literal["AppStream"],
         "statusReason": str,
         "trustStoreArn": str,
@@ -450,14 +620,23 @@
 GetPortalServiceProviderMetadataRequestRequestTypeDef = TypedDict(
     "GetPortalServiceProviderMetadataRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
+GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
+    "GetPortalServiceProviderMetadataResponseTypeDef",
+    {
+        "portalArn": str,
+        "serviceProviderSamlMetadata": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTrustStoreCertificateRequestRequestTypeDef = TypedDict(
     "GetTrustStoreCertificateRequestRequestTypeDef",
     {
         "thumbprint": str,
         "trustStoreArn": str,
     },
 )
@@ -542,14 +721,25 @@
         "identityProviderArn": str,
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
+IpAccessSettingsSummaryTypeDef = TypedDict(
+    "IpAccessSettingsSummaryTypeDef",
+    {
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipAccessSettingsArn": str,
+    },
+    total=False,
+)
+
 ListBrowserSettingsRequestRequestTypeDef = TypedDict(
     "ListBrowserSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -572,14 +762,23 @@
 
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
+ListIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "ListIpAccessSettingsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 ListNetworkSettingsRequestRequestTypeDef = TypedDict(
     "ListNetworkSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -607,14 +806,15 @@
     "PortalSummaryTypeDef",
     {
         "authenticationType": AuthenticationTypeType,
         "browserSettingsArn": str,
         "browserType": Literal["Chrome"],
         "creationDate": datetime,
         "displayName": str,
+        "ipAccessSettingsArn": str,
         "networkSettingsArn": str,
         "portalArn": str,
         "portalEndpoint": str,
         "portalStatus": PortalStatusType,
         "rendererType": Literal["AppStream"],
         "trustStoreArn": str,
         "userAccessLoggingSettingsArn": str,
@@ -706,14 +906,25 @@
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
         "userSettingsArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -822,14 +1033,22 @@
 )
 
 class UpdateTrustStoreRequestRequestTypeDef(
     _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
 ):
     pass
 
+UpdateTrustStoreResponseTypeDef = TypedDict(
+    "UpdateTrustStoreResponseTypeDef",
+    {
+        "trustStoreArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -870,174 +1089,55 @@
 
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
-AssociateBrowserSettingsResponseTypeDef = TypedDict(
-    "AssociateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateNetworkSettingsResponseTypeDef = TypedDict(
-    "AssociateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "portalArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateTrustStoreResponseTypeDef = TypedDict(
-    "AssociateTrustStoreResponseTypeDef",
-    {
-        "portalArn": str,
-        "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "AssociateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateUserSettingsResponseTypeDef = TypedDict(
-    "AssociateUserSettingsResponseTypeDef",
-    {
-        "portalArn": str,
-        "userSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBrowserSettingsResponseTypeDef = TypedDict(
-    "CreateBrowserSettingsResponseTypeDef",
-    {
-        "browserSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIdentityProviderResponseTypeDef = TypedDict(
-    "CreateIdentityProviderResponseTypeDef",
-    {
-        "identityProviderArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNetworkSettingsResponseTypeDef = TypedDict(
-    "CreateNetworkSettingsResponseTypeDef",
-    {
-        "networkSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePortalResponseTypeDef = TypedDict(
-    "CreatePortalResponseTypeDef",
-    {
-        "portalArn": str,
-        "portalEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTrustStoreResponseTypeDef = TypedDict(
-    "CreateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
-    "CreateUserAccessLoggingSettingsResponseTypeDef",
-    {
-        "userAccessLoggingSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateUserSettingsResponseTypeDef = TypedDict(
-    "CreateUserSettingsResponseTypeDef",
-    {
-        "userSettingsArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPortalServiceProviderMetadataResponseTypeDef = TypedDict(
-    "GetPortalServiceProviderMetadataResponseTypeDef",
-    {
-        "portalArn": str,
-        "serviceProviderSamlMetadata": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTrustStoreResponseTypeDef = TypedDict(
-    "UpdateTrustStoreResponseTypeDef",
-    {
-        "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListBrowserSettingsResponseTypeDef = TypedDict(
     "ListBrowserSettingsResponseTypeDef",
     {
         "browserSettings": List[BrowserSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBrowserSettingsResponseTypeDef = TypedDict(
     "GetBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBrowserSettingsResponseTypeDef = TypedDict(
     "UpdateBrowserSettingsResponseTypeDef",
     {
         "browserSettings": BrowserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrustStoreCertificatesResponseTypeDef = TypedDict(
     "ListTrustStoreCertificatesResponseTypeDef",
     {
         "certificateList": List[CertificateSummaryTypeDef],
         "nextToken": str,
         "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrustStoreCertificateResponseTypeDef = TypedDict(
     "GetTrustStoreCertificateResponseTypeDef",
     {
         "certificate": CertificateTypeDef,
         "trustStoreArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBrowserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrowserSettingsRequestRequestTypeDef",
     {
         "browserPolicy": str,
@@ -1164,15 +1264,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1188,148 +1288,242 @@
 )
 
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipRules": Sequence[IpRuleTypeDef],
+    },
+)
+_OptionalCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "additionalEncryptionContext": Mapping[str, str],
+        "clientToken": str,
+        "customerManagedKey": str,
+        "description": str,
+        "displayName": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateIpAccessSettingsRequestRequestTypeDef(
+    _RequiredCreateIpAccessSettingsRequestRequestTypeDef,
+    _OptionalCreateIpAccessSettingsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredIpAccessSettingsTypeDef = TypedDict(
+    "_RequiredIpAccessSettingsTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalIpAccessSettingsTypeDef = TypedDict(
+    "_OptionalIpAccessSettingsTypeDef",
+    {
+        "associatedPortalArns": List[str],
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipRules": List[IpRuleTypeDef],
+    },
+    total=False,
+)
+
+class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
+    pass
+
+_RequiredUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIpAccessSettingsRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "description": str,
+        "displayName": str,
+        "ipRules": Sequence[IpRuleTypeDef],
+    },
+    total=False,
+)
+
+class UpdateIpAccessSettingsRequestRequestTypeDef(
+    _RequiredUpdateIpAccessSettingsRequestRequestTypeDef,
+    _OptionalUpdateIpAccessSettingsRequestRequestTypeDef,
+):
+    pass
+
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNetworkSettingsResponseTypeDef = TypedDict(
     "GetNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNetworkSettingsResponseTypeDef = TypedDict(
     "UpdateNetworkSettingsResponseTypeDef",
     {
         "networkSettings": NetworkSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPortalResponseTypeDef = TypedDict(
     "GetPortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePortalResponseTypeDef = TypedDict(
     "UpdatePortalResponseTypeDef",
     {
         "portal": PortalTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrustStoreResponseTypeDef = TypedDict(
     "GetTrustStoreResponseTypeDef",
     {
         "trustStore": TrustStoreTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "GetUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     {
         "userAccessLoggingSettings": UserAccessLoggingSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateUserSettingsResponseTypeDef = TypedDict(
     "UpdateUserSettingsResponseTypeDef",
     {
         "userSettings": UserSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "identityProviders": List[IdentityProviderSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListIpAccessSettingsResponseTypeDef = TypedDict(
+    "ListIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPortalsResponseTypeDef = TypedDict(
     "ListPortalsResponseTypeDef",
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserAccessLoggingSettingsResponseTypeDef = TypedDict(
     "ListUserAccessLoggingSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userAccessLoggingSettings": List[UserAccessLoggingSettingsSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUserSettingsResponseTypeDef = TypedDict(
     "ListUserSettingsResponseTypeDef",
     {
         "nextToken": str,
         "userSettings": List[UserSettingsSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetIpAccessSettingsResponseTypeDef = TypedDict(
+    "GetIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettings": IpAccessSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateIpAccessSettingsResponseTypeDef = TypedDict(
+    "UpdateIpAccessSettingsResponseTypeDef",
+    {
+        "ipAccessSettings": IpAccessSettingsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/PKG-INFO` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.26.46
-Summary: Type annotations for boto3.WorkSpacesWeb 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.WorkSpacesWeb 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces-web?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,161 +304,176 @@
 
 `mypy_boto3_workspaces_web.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces_web.type_defs import (
     AssociateBrowserSettingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateBrowserSettingsResponseTypeDef,
+    AssociateIpAccessSettingsRequestRequestTypeDef,
+    AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsRequestRequestTypeDef,
+    AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreRequestRequestTypeDef,
+    AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsRequestRequestTypeDef,
+    AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsRequestRequestTypeDef,
+    AssociateUserSettingsResponseTypeDef,
     BrowserSettingsSummaryTypeDef,
     BrowserSettingsTypeDef,
     CertificateSummaryTypeDef,
     CertificateTypeDef,
     TagTypeDef,
+    CreateBrowserSettingsResponseTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    IpRuleTypeDef,
+    CreateIpAccessSettingsResponseTypeDef,
+    CreateNetworkSettingsResponseTypeDef,
+    CreatePortalResponseTypeDef,
+    CreateTrustStoreResponseTypeDef,
+    CreateUserAccessLoggingSettingsResponseTypeDef,
+    CreateUserSettingsResponseTypeDef,
     DeleteBrowserSettingsRequestRequestTypeDef,
     DeleteIdentityProviderRequestRequestTypeDef,
+    DeleteIpAccessSettingsRequestRequestTypeDef,
     DeleteNetworkSettingsRequestRequestTypeDef,
     DeletePortalRequestRequestTypeDef,
     DeleteTrustStoreRequestRequestTypeDef,
     DeleteUserAccessLoggingSettingsRequestRequestTypeDef,
     DeleteUserSettingsRequestRequestTypeDef,
     DisassociateBrowserSettingsRequestRequestTypeDef,
+    DisassociateIpAccessSettingsRequestRequestTypeDef,
     DisassociateNetworkSettingsRequestRequestTypeDef,
     DisassociateTrustStoreRequestRequestTypeDef,
     DisassociateUserAccessLoggingSettingsRequestRequestTypeDef,
     DisassociateUserSettingsRequestRequestTypeDef,
     GetBrowserSettingsRequestRequestTypeDef,
     GetIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeDef,
+    GetIpAccessSettingsRequestRequestTypeDef,
     GetNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsTypeDef,
     GetPortalRequestRequestTypeDef,
     PortalTypeDef,
     GetPortalServiceProviderMetadataRequestRequestTypeDef,
+    GetPortalServiceProviderMetadataResponseTypeDef,
     GetTrustStoreCertificateRequestRequestTypeDef,
     GetTrustStoreRequestRequestTypeDef,
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
+    IpAccessSettingsSummaryTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
+    ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrowserSettingsRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
     UpdateNetworkSettingsRequestRequestTypeDef,
     UpdatePortalRequestRequestTypeDef,
     UpdateTrustStoreRequestRequestTypeDef,
+    UpdateTrustStoreResponseTypeDef,
     UpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    AssociateBrowserSettingsResponseTypeDef,
-    AssociateNetworkSettingsResponseTypeDef,
-    AssociateTrustStoreResponseTypeDef,
-    AssociateUserAccessLoggingSettingsResponseTypeDef,
-    AssociateUserSettingsResponseTypeDef,
-    CreateBrowserSettingsResponseTypeDef,
-    CreateIdentityProviderResponseTypeDef,
-    CreateNetworkSettingsResponseTypeDef,
-    CreatePortalResponseTypeDef,
-    CreateTrustStoreResponseTypeDef,
-    CreateUserAccessLoggingSettingsResponseTypeDef,
-    CreateUserSettingsResponseTypeDef,
-    GetPortalServiceProviderMetadataResponseTypeDef,
-    UpdateTrustStoreResponseTypeDef,
     ListBrowserSettingsResponseTypeDef,
     GetBrowserSettingsResponseTypeDef,
     UpdateBrowserSettingsResponseTypeDef,
     ListTrustStoreCertificatesResponseTypeDef,
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateIpAccessSettingsRequestRequestTypeDef,
+    IpAccessSettingsTypeDef,
+    UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
+    ListIpAccessSettingsResponseTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
+    GetIpAccessSettingsResponseTypeDef,
+    UpdateIpAccessSettingsResponseTypeDef,
 )
 
 
 def get_structure() -> AssociateBrowserSettingsRequestRequestTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-workspaces-web-1.26.46/mypy_boto3_workspaces_web.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-web-1.27.0/mypy_boto3_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.26.46/setup.py` & `mypy-boto3-workspaces-web-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-workspaces-web.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces-web",
-    version="1.26.46",
+    version="1.27.0",
     packages=["mypy_boto3_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpacesWeb 1.26.46 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.WorkSpacesWeb 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/",
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


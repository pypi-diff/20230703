# Comparing `tmp/mypy-boto3-cognito-identity-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cognito-identity-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-identity-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:15 2022, max compression
+gzip compressed data, was "mypy-boto3-cognito-identity-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-cognito-identity-1.26.0.post1.tar` & `mypy-boto3-cognito-identity-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.864818 mypy-boto3-cognito-identity-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15099 2022-11-01 21:43:15.856819 mypy-boto3-cognito-identity-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13623 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.856819 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19522 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    19491 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7812 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7810 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    18265 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18241 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:15.856819 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15099 2022-11-01 21:43:15.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-01 21:43:15.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:15.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:15.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-01 21:43:15.000000 mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:15.864818 mypy-boto3-cognito-identity-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-11-01 21:32:02.000000 mypy-boto3-cognito-identity-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.043026 mypy-boto3-cognito-identity-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-03 19:50:34.039025 mypy-boto3-cognito-identity-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.031025 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-07-03 19:34:32.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.039025 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-03 19:50:33.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:50:33.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:33.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:33.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:50:33.000000 mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.043026 mypy-boto3-cognito-identity-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 19:34:31.000000 mypy-boto3-cognito-identity-1.27.0/setup.py
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/LICENSE` & `mypy-boto3-cognito-identity-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/PKG-INFO` & `mypy-boto3-cognito-identity-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CognitoIdentity 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CognitoIdentity 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
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
 
 <a id="mypy-boto3-cognito-identity"></a>
 
 # mypy-boto3-cognito-identity
 
 [![PyPI - mypy-boto3-cognito-identity](https://img.shields.io/pypi/v/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,57 +329,57 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
+    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
+    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCredentialsForIdentityResponseTypeDef,
-    GetIdResponseTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
-    GetOpenIdTokenResponseTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityPoolTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
+    GetCredentialsForIdentityResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
@@ -389,42 +390,42 @@
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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/README.md` & `mypy-boto3-cognito-identity-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cognito-identity"></a>
 
 # mypy-boto3-cognito-identity
 
 [![PyPI - mypy-boto3-cognito-identity](https://img.shields.io/pypi/v/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,57 +297,57 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
+    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
+    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCredentialsForIdentityResponseTypeDef,
-    GetIdResponseTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
-    GetOpenIdTokenResponseTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityPoolTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
+    GetCredentialsForIdentityResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
@@ -358,42 +358,42 @@
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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/__init__.py` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/__init__.pyi` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/__main__.py` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentity 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CognitoIdentity 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/client.py` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         *,
         SourceUserIdentifier: str,
         DestinationUserIdentifier: str,
         DeveloperProviderName: str,
         IdentityPoolId: str
     ) -> MergeDeveloperIdentitiesResponseTypeDef:
         """
-        Merges two users having different `IdentityId` s, existing in the same identity
+        Merges two users having different `IdentityId`s, existing in the same identity
         pool, and identified by the same developer provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.merge_developer_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#merge_developer_identities)
         """
 
     def set_identity_pool_roles(
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/client.pyi` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         *,
         SourceUserIdentifier: str,
         DestinationUserIdentifier: str,
         DeveloperProviderName: str,
         IdentityPoolId: str
     ) -> MergeDeveloperIdentitiesResponseTypeDef:
         """
-        Merges two users having different `IdentityId` s, existing in the same identity
+        Merges two users having different `IdentityId`s, existing in the same identity
         pool, and identified by the same developer provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.merge_developer_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/client/#merge_developer_identities)
         """
     def set_identity_pool_roles(
         self,
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/literals.py` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AmbiguousRoleResolutionTypeType",
     "ErrorCodeType",
     "ListIdentityPoolsPaginatorName",
     "MappingRuleMatchTypeType",
     "RoleMappingTypeType",
     "CognitoIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AmbiguousRoleResolutionTypeType = Literal["AuthenticatedRole", "Deny"]
 ErrorCodeType = Literal["AccessDenied", "InternalServerError"]
 ListIdentityPoolsPaginatorName = Literal["list_identity_pools"]
 MappingRuleMatchTypeType = Literal["Contains", "Equals", "NotEqual", "StartsWith"]
 RoleMappingTypeType = Literal["Rules", "Token"]
 CognitoIdentityServiceName = Literal["cognito-identity"]
 ServiceName = Literal[
@@ -50,23 +48,25 @@
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
@@ -76,30 +76,35 @@
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
@@ -125,14 +130,15 @@
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
@@ -177,51 +183,57 @@
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
@@ -234,14 +246,15 @@
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
@@ -253,28 +266,35 @@
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
@@ -283,14 +303,15 @@
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
@@ -301,55 +322,64 @@
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
@@ -377,14 +407,15 @@
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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/literals.pyi` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AmbiguousRoleResolutionTypeType",
     "ErrorCodeType",
     "ListIdentityPoolsPaginatorName",
     "MappingRuleMatchTypeType",
     "RoleMappingTypeType",
     "CognitoIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AmbiguousRoleResolutionTypeType = Literal["AuthenticatedRole", "Deny"]
 ErrorCodeType = Literal["AccessDenied", "InternalServerError"]
 ListIdentityPoolsPaginatorName = Literal["list_identity_pools"]
 MappingRuleMatchTypeType = Literal["Contains", "Equals", "NotEqual", "StartsWith"]
 RoleMappingTypeType = Literal["Rules", "Token"]
 CognitoIdentityServiceName = Literal["cognito-identity"]
 ServiceName = Literal[
@@ -48,23 +50,25 @@
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
@@ -74,30 +78,35 @@
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
@@ -123,14 +132,15 @@
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
@@ -175,51 +185,57 @@
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
@@ -232,14 +248,15 @@
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
@@ -251,28 +268,35 @@
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
@@ -281,14 +305,15 @@
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
@@ -299,55 +324,64 @@
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
@@ -375,14 +409,15 @@
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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/paginator.py` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListIdentityPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/paginator.pyi` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListIdentityPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentityPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/paginators/#listidentitypoolspaginator)
         """
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/type_defs.py` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,57 +28,57 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityInputRequestTypeDef",
     "GetIdInputRequestTypeDef",
+    "GetIdResponseTypeDef",
     "GetIdentityPoolRolesInputRequestTypeDef",
     "GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef",
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     "GetOpenIdTokenInputRequestTypeDef",
+    "GetOpenIdTokenResponseTypeDef",
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityDescriptionTypeDef",
     "IdentityPoolShortDescriptionTypeDef",
     "ListIdentitiesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
+    "LookupDeveloperIdentityResponseTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
+    "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCredentialsForIdentityResponseTypeDef",
-    "GetIdResponseTypeDef",
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    "GetOpenIdTokenResponseTypeDef",
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityPoolTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LookupDeveloperIdentityResponseTypeDef",
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    "SetPrincipalTagAttributeMapResponseTypeDef",
+    "GetCredentialsForIdentityResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "RulesConfigurationTypeTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
@@ -105,25 +105,14 @@
 DeleteIdentitiesInputRequestTypeDef = TypedDict(
     "DeleteIdentitiesInputRequestTypeDef",
     {
         "IdentityIdsToDelete": Sequence[str],
     },
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
 UnprocessedIdentityIdTypeDef = TypedDict(
     "UnprocessedIdentityIdTypeDef",
     {
         "IdentityId": str,
         "ErrorCode": ErrorCodeType,
     },
     total=False,
@@ -146,14 +135,21 @@
 DescribeIdentityPoolInputRequestTypeDef = TypedDict(
     "DescribeIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
     "_RequiredGetCredentialsForIdentityInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
@@ -191,14 +187,22 @@
 
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
 
+GetIdResponseTypeDef = TypedDict(
+    "GetIdResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -223,14 +227,23 @@
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
 
+GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
@@ -244,22 +257,53 @@
 
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
 
+GetOpenIdTokenResponseTypeDef = TypedDict(
+    "GetOpenIdTokenResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
 
+GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+IdentityDescriptionResponseMetadataTypeDef = TypedDict(
+    "IdentityDescriptionResponseMetadataTypeDef",
+    {
+        "IdentityId": str,
+        "Logins": List[str],
+        "CreationDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IdentityDescriptionTypeDef = TypedDict(
     "IdentityDescriptionTypeDef",
     {
         "IdentityId": str,
         "Logins": List[str],
         "CreationDate": datetime,
         "LastModifiedDate": datetime,
@@ -295,20 +339,18 @@
 
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 _RequiredListIdentityPoolsInputRequestTypeDef = TypedDict(
     "_RequiredListIdentityPoolsInputRequestTypeDef",
     {
@@ -333,14 +375,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
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
 _RequiredLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
     "_RequiredLookupDeveloperIdentityInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
@@ -358,14 +408,24 @@
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
 
+LookupDeveloperIdentityResponseTypeDef = TypedDict(
+    "LookupDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "DeveloperUserIdentifierList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -378,14 +438,43 @@
         "SourceUserIdentifier": str,
         "DestinationUserIdentifier": str,
         "DeveloperProviderName": str,
         "IdentityPoolId": str,
     },
 )
 
+MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "_RequiredSetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -402,14 +491,25 @@
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
 
+SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "SetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -494,167 +594,67 @@
 
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCredentialsForIdentityResponseTypeDef = TypedDict(
-    "GetCredentialsForIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIdResponseTypeDef = TypedDict(
-    "GetIdResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOpenIdTokenResponseTypeDef = TypedDict(
-    "GetOpenIdTokenResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IdentityDescriptionResponseMetadataTypeDef = TypedDict(
-    "IdentityDescriptionResponseMetadataTypeDef",
-    {
-        "IdentityId": str,
-        "Logins": List[str],
-        "CreationDate": datetime,
-        "LastModifiedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 IdentityPoolTypeDef = TypedDict(
     "IdentityPoolTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
         "AllowClassicFlow": bool,
         "SupportedLoginProviders": Dict[str, str],
         "DeveloperProviderName": str,
         "OpenIdConnectProviderARNs": List[str],
         "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": List[str],
         "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LookupDeveloperIdentityResponseTypeDef = TypedDict(
-    "LookupDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "DeveloperUserIdentifierList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
-    "MergeDeveloperIdentitiesResponseTypeDef",
+GetCredentialsForIdentityResponseTypeDef = TypedDict(
+    "GetCredentialsForIdentityResponseTypeDef",
     {
         "IdentityId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "SetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Credentials": CredentialsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteIdentitiesResponseTypeDef = TypedDict(
     "DeleteIdentitiesResponseTypeDef",
     {
         "UnprocessedIdentityIds": List[UnprocessedIdentityIdTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentitiesResponseTypeDef = TypedDict(
     "ListIdentitiesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Identities": List[IdentityDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityPoolsResponseTypeDef = TypedDict(
     "ListIdentityPoolsResponseTypeDef",
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
         "Rules": List[MappingRuleTypeDef],
     },
 )
 
@@ -680,15 +680,15 @@
 
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
         "RoleMappings": Dict[str, RoleMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity/type_defs.pyi` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -27,57 +27,57 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetCredentialsForIdentityInputRequestTypeDef",
     "GetIdInputRequestTypeDef",
+    "GetIdResponseTypeDef",
     "GetIdentityPoolRolesInputRequestTypeDef",
     "GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef",
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     "GetOpenIdTokenInputRequestTypeDef",
+    "GetOpenIdTokenResponseTypeDef",
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityDescriptionTypeDef",
     "IdentityPoolShortDescriptionTypeDef",
     "ListIdentitiesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
+    "LookupDeveloperIdentityResponseTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
+    "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCredentialsForIdentityResponseTypeDef",
-    "GetIdResponseTypeDef",
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    "GetOpenIdTokenResponseTypeDef",
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    "IdentityDescriptionResponseMetadataTypeDef",
     "IdentityPoolTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "LookupDeveloperIdentityResponseTypeDef",
-    "MergeDeveloperIdentitiesResponseTypeDef",
-    "SetPrincipalTagAttributeMapResponseTypeDef",
+    "GetCredentialsForIdentityResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "RulesConfigurationTypeTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
@@ -104,25 +104,14 @@
 DeleteIdentitiesInputRequestTypeDef = TypedDict(
     "DeleteIdentitiesInputRequestTypeDef",
     {
         "IdentityIdsToDelete": Sequence[str],
     },
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
 UnprocessedIdentityIdTypeDef = TypedDict(
     "UnprocessedIdentityIdTypeDef",
     {
         "IdentityId": str,
         "ErrorCode": ErrorCodeType,
     },
     total=False,
@@ -145,14 +134,21 @@
 DescribeIdentityPoolInputRequestTypeDef = TypedDict(
     "DescribeIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
     "_RequiredGetCredentialsForIdentityInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetCredentialsForIdentityInputRequestTypeDef = TypedDict(
@@ -186,14 +182,22 @@
 )
 
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
+GetIdResponseTypeDef = TypedDict(
+    "GetIdResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "GetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
@@ -216,14 +220,23 @@
 
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
+GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
+    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetOpenIdTokenInputRequestTypeDef = TypedDict(
     "_RequiredGetOpenIdTokenInputRequestTypeDef",
     {
         "IdentityId": str,
     },
 )
 _OptionalGetOpenIdTokenInputRequestTypeDef = TypedDict(
@@ -235,22 +248,53 @@
 )
 
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
+GetOpenIdTokenResponseTypeDef = TypedDict(
+    "GetOpenIdTokenResponseTypeDef",
+    {
+        "IdentityId": str,
+        "Token": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "GetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
 
+GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "GetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+IdentityDescriptionResponseMetadataTypeDef = TypedDict(
+    "IdentityDescriptionResponseMetadataTypeDef",
+    {
+        "IdentityId": str,
+        "Logins": List[str],
+        "CreationDate": datetime,
+        "LastModifiedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IdentityDescriptionTypeDef = TypedDict(
     "IdentityDescriptionTypeDef",
     {
         "IdentityId": str,
         "Logins": List[str],
         "CreationDate": datetime,
         "LastModifiedDate": datetime,
@@ -284,20 +328,18 @@
 )
 
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
+    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 _RequiredListIdentityPoolsInputRequestTypeDef = TypedDict(
     "_RequiredListIdentityPoolsInputRequestTypeDef",
     {
@@ -320,14 +362,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
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
 _RequiredLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
     "_RequiredLookupDeveloperIdentityInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalLookupDeveloperIdentityInputRequestTypeDef = TypedDict(
@@ -343,14 +393,24 @@
 
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
+LookupDeveloperIdentityResponseTypeDef = TypedDict(
+    "LookupDeveloperIdentityResponseTypeDef",
+    {
+        "IdentityId": str,
+        "DeveloperUserIdentifierList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -363,14 +423,43 @@
         "SourceUserIdentifier": str,
         "DestinationUserIdentifier": str,
         "DeveloperProviderName": str,
         "IdentityPoolId": str,
     },
 )
 
+MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
+    "MergeDeveloperIdentitiesResponseTypeDef",
+    {
+        "IdentityId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef = TypedDict(
     "_RequiredSetPrincipalTagAttributeMapInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
     },
 )
@@ -385,14 +474,25 @@
 
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
+SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
+    "SetPrincipalTagAttributeMapResponseTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityProviderName": str,
+        "UseDefaults": bool,
+        "PrincipalTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -473,167 +573,67 @@
 )
 
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCredentialsForIdentityResponseTypeDef = TypedDict(
-    "GetCredentialsForIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Credentials": CredentialsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIdResponseTypeDef = TypedDict(
-    "GetIdResponseTypeDef",
-    {
-        "IdentityId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
-    "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetOpenIdTokenResponseTypeDef = TypedDict(
-    "GetOpenIdTokenResponseTypeDef",
-    {
-        "IdentityId": str,
-        "Token": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "GetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IdentityDescriptionResponseMetadataTypeDef = TypedDict(
-    "IdentityDescriptionResponseMetadataTypeDef",
-    {
-        "IdentityId": str,
-        "Logins": List[str],
-        "CreationDate": datetime,
-        "LastModifiedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 IdentityPoolTypeDef = TypedDict(
     "IdentityPoolTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
         "AllowClassicFlow": bool,
         "SupportedLoginProviders": Dict[str, str],
         "DeveloperProviderName": str,
         "OpenIdConnectProviderARNs": List[str],
         "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": List[str],
         "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LookupDeveloperIdentityResponseTypeDef = TypedDict(
-    "LookupDeveloperIdentityResponseTypeDef",
-    {
-        "IdentityId": str,
-        "DeveloperUserIdentifierList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeDeveloperIdentitiesResponseTypeDef = TypedDict(
-    "MergeDeveloperIdentitiesResponseTypeDef",
+GetCredentialsForIdentityResponseTypeDef = TypedDict(
+    "GetCredentialsForIdentityResponseTypeDef",
     {
         "IdentityId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
-    "SetPrincipalTagAttributeMapResponseTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityProviderName": str,
-        "UseDefaults": bool,
-        "PrincipalTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Credentials": CredentialsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteIdentitiesResponseTypeDef = TypedDict(
     "DeleteIdentitiesResponseTypeDef",
     {
         "UnprocessedIdentityIds": List[UnprocessedIdentityIdTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentitiesResponseTypeDef = TypedDict(
     "ListIdentitiesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Identities": List[IdentityDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIdentityPoolsResponseTypeDef = TypedDict(
     "ListIdentityPoolsResponseTypeDef",
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
-    "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
         "Rules": List[MappingRuleTypeDef],
     },
 )
 
@@ -657,15 +657,15 @@
 
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
         "RoleMappings": Dict[str, RoleMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
```

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/PKG-INFO` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CognitoIdentity 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CognitoIdentity 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
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
 
 <a id="mypy-boto3-cognito-identity"></a>
 
 # mypy-boto3-cognito-identity
 
 [![PyPI - mypy-boto3-cognito-identity](https://img.shields.io/pypi/v/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,57 +329,57 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetCredentialsForIdentityInputRequestTypeDef,
     GetIdInputRequestTypeDef,
+    GetIdResponseTypeDef,
     GetIdentityPoolRolesInputRequestTypeDef,
     GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
+    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
     GetOpenIdTokenInputRequestTypeDef,
+    GetOpenIdTokenResponseTypeDef,
     GetPrincipalTagAttributeMapInputRequestTypeDef,
+    GetPrincipalTagAttributeMapResponseTypeDef,
+    IdentityDescriptionResponseMetadataTypeDef,
     IdentityDescriptionTypeDef,
     IdentityPoolShortDescriptionTypeDef,
     ListIdentitiesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
+    LookupDeveloperIdentityResponseTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
+    MergeDeveloperIdentitiesResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
+    SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCredentialsForIdentityResponseTypeDef,
-    GetIdResponseTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
-    GetOpenIdTokenResponseTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseMetadataTypeDef,
     IdentityPoolTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
+    GetCredentialsForIdentityResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     RulesConfigurationTypeTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
@@ -389,42 +390,42 @@
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

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/mypy_boto3_cognito_identity.egg-info/SOURCES.txt` & `mypy-boto3-cognito-identity-1.27.0/mypy_boto3_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.26.0.post1/setup.py` & `mypy-boto3-cognito-identity-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cognito-identity.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-identity",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentity 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CognitoIdentity 1.27.0 service generated with"
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
     keywords="boto3 cognito-identity type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cognito_identity": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cognito_identity": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/",
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


# Comparing `tmp/mypy-boto3-verifiedpermissions-1.26.165.tar.gz` & `tmp/mypy-boto3-verifiedpermissions-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-verifiedpermissions-1.26.165.tar", last modified: Fri Jun 30 19:48:24 2023, max compression
+gzip compressed data, was "mypy-boto3-verifiedpermissions-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
```

## Comparing `mypy-boto3-verifiedpermissions-1.26.165.tar` & `mypy-boto3-verifiedpermissions-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:24.105281 mypy-boto3-verifiedpermissions-1.26.165/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-06-30 19:48:24.105281 mypy-boto3-verifiedpermissions-1.26.165/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:24.105281 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31198 2023-06-30 19:48:11.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31147 2023-06-30 19:48:11.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:48:24.105281 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-06-30 19:48:23.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-30 19:48:23.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:48:23.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:48:23.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 19:48:23.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 19:48:23.000000 mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:48:24.105281 mypy-boto3-verifiedpermissions-1.26.165/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-30 19:48:10.000000 mypy-boto3-verifiedpermissions-1.26.165/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.000122 mypy-boto3-verifiedpermissions-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-07-03 19:51:34.996122 mypy-boto3-verifiedpermissions-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.996122 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31246 2023-07-03 19:49:18.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31195 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.996122 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-07-03 19:51:34.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:51:34.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:34.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:51:34.000000 mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.000122 mypy-boto3-verifiedpermissions-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-03 19:49:17.000000 mypy-boto3-verifiedpermissions-1.27.0/setup.py
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/LICENSE` & `mypy-boto3-verifiedpermissions-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.26.165
-Summary: Type annotations for boto3.VerifiedPermissions 1.26.165 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.VerifiedPermissions 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.26.165](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -343,72 +343,72 @@
 
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateIdentitySourceOutputTypeDef,
     ValidationSettingsTypeDef,
+    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
+    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
+    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
+    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
+    PutSchemaOutputTypeDef,
+    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
+    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
-    ConfigurationTypeDef,
-    CreateIdentitySourceOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    CreatePolicyStoreOutputTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
-    GetPolicyTemplateOutputTypeDef,
-    GetSchemaOutputTypeDef,
-    PutSchemaOutputTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdatePolicyOutputTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
+    ConfigurationTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
     GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/README.md` & `mypy-boto3-verifiedpermissions-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.26.165](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -311,72 +311,72 @@
 
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateIdentitySourceOutputTypeDef,
     ValidationSettingsTypeDef,
+    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
+    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
+    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
+    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
+    PutSchemaOutputTypeDef,
+    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
+    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
-    ConfigurationTypeDef,
-    CreateIdentitySourceOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    CreatePolicyStoreOutputTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
-    GetPolicyTemplateOutputTypeDef,
-    GetSchemaOutputTypeDef,
-    PutSchemaOutputTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdatePolicyOutputTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
+    ConfigurationTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
     GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/__init__.py` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/__init__.pyi` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/__main__.py` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VerifiedPermissions 1.26.165\nVersion:        "
-        " 1.26.165\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.VerifiedPermissions 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.165")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/client.py` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/client.pyi` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/literals.py` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/literals.pyi` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/paginator.py` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,84 +42,78 @@
 __all__ = (
     "ListIdentitySourcesPaginator",
     "ListPoliciesPaginator",
     "ListPolicyStoresPaginator",
     "ListPolicyTemplatesPaginator",
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
 class ListIdentitySourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listidentitysourcespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
-
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
-
 class ListPolicyStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
-
 class ListPolicyTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
-        self, *, policyStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, policyStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPolicyTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
         """
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/paginator.pyi` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,78 +42,84 @@
 __all__ = (
     "ListIdentitySourcesPaginator",
     "ListPoliciesPaginator",
     "ListPolicyStoresPaginator",
     "ListPolicyTemplatesPaginator",
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
 class ListIdentitySourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listidentitysourcespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
+
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
+
 class ListPolicyStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
+
 class ListPolicyTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
-        self, *, policyStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, policyStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPolicyTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
         """
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/type_defs.py` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,72 +28,72 @@
 
 
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateIdentitySourceOutputTypeDef",
     "ValidationSettingsTypeDef",
+    "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
+    "CreatePolicyTemplateOutputTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
+    "GetPolicyTemplateOutputTypeDef",
     "GetSchemaInputRequestTypeDef",
+    "GetSchemaOutputTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
+    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
+    "PaginatorConfigTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
+    "PutSchemaOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
+    "UpdateIdentitySourceOutputTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
+    "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
+    "UpdatePolicyTemplateOutputTypeDef",
     "AttributeValueTypeDef",
+    "CreatePolicyOutputTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
-    "ConfigurationTypeDef",
-    "CreateIdentitySourceOutputTypeDef",
-    "CreatePolicyOutputTypeDef",
-    "CreatePolicyStoreOutputTypeDef",
-    "CreatePolicyTemplateOutputTypeDef",
-    "GetPolicyTemplateOutputTypeDef",
-    "GetSchemaOutputTypeDef",
-    "PutSchemaOutputTypeDef",
-    "UpdateIdentitySourceOutputTypeDef",
     "UpdatePolicyOutputTypeDef",
-    "UpdatePolicyStoreOutputTypeDef",
-    "UpdatePolicyTemplateOutputTypeDef",
+    "ConfigurationTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
     "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
+    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
-    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
-    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
@@ -155,32 +155,43 @@
     "ContextDefinitionTypeDef",
     {
         "contextMap": Mapping[str, "AttributeValueTypeDef"],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateIdentitySourceOutputTypeDef = TypedDict(
+    "CreateIdentitySourceOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
 )
 
+CreatePolicyStoreOutputTypeDef = TypedDict(
+    "CreatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "statement": str,
     },
 )
@@ -197,14 +208,25 @@
 class CreatePolicyTemplateInputRequestTypeDef(
     _RequiredCreatePolicyTemplateInputRequestTypeDef,
     _OptionalCreatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
 
+CreatePolicyTemplateOutputTypeDef = TypedDict(
+    "CreatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIdentitySourceInputRequestTypeDef = TypedDict(
     "DeleteIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
         "identitySourceId": str,
     },
 )
@@ -284,21 +306,45 @@
     "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
     },
 )
 
+GetPolicyTemplateOutputTypeDef = TypedDict(
+    "GetPolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "description": str,
+        "statement": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
+GetSchemaOutputTypeDef = TypedDict(
+    "GetSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "schema": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IdentitySourceFilterTypeDef = TypedDict(
     "IdentitySourceFilterTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
@@ -310,20 +356,18 @@
         "userPoolArn": str,
         "discoveryUrl": str,
         "openIdIssuer": Literal["COGNITO"],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPolicyStoresInputRequestTypeDef = TypedDict(
     "ListPolicyStoresInputRequestTypeDef",
     {
@@ -338,14 +382,36 @@
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
     },
 )
 
+_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
+    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPolicyTemplatesInputRequestTypeDef = TypedDict(
     "_RequiredListPolicyTemplatesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPolicyTemplatesInputRequestTypeDef = TypedDict(
@@ -384,14 +450,24 @@
 
 class PolicyTemplateItemTypeDef(
     _RequiredPolicyTemplateItemTypeDef, _OptionalPolicyTemplateItemTypeDef
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
 _RequiredStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredStaticPolicyDefinitionDetailTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalStaticPolicyDefinitionDetailTypeDef = TypedDict(
@@ -442,14 +518,36 @@
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": str,
     },
     total=False,
 )
 
+PutSchemaOutputTypeDef = TypedDict(
+    "PutSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "namespaces": List[str],
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
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
 _RequiredUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_RequiredUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "userPoolArn": str,
     },
 )
 _OptionalUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
@@ -464,14 +562,25 @@
 class UpdateCognitoUserPoolConfigurationTypeDef(
     _RequiredUpdateCognitoUserPoolConfigurationTypeDef,
     _OptionalUpdateCognitoUserPoolConfigurationTypeDef,
 ):
     pass
 
 
+UpdateIdentitySourceOutputTypeDef = TypedDict(
+    "UpdateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_RequiredUpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalUpdateStaticPolicyDefinitionTypeDef = TypedDict(
@@ -485,14 +594,25 @@
 
 class UpdateStaticPolicyDefinitionTypeDef(
     _RequiredUpdateStaticPolicyDefinitionTypeDef, _OptionalUpdateStaticPolicyDefinitionTypeDef
 ):
     pass
 
 
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "statement": str,
     },
@@ -509,27 +629,52 @@
 class UpdatePolicyTemplateInputRequestTypeDef(
     _RequiredUpdatePolicyTemplateInputRequestTypeDef,
     _OptionalUpdatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
 
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "boolean": bool,
         "entityIdentifier": EntityIdentifierTypeDef,
         "long": int,
         "string": str,
         "set": Sequence[Dict[str, Any]],
         "record": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEntityItemTypeDef = TypedDict(
     "_RequiredEntityItemTypeDef",
     {
         "identifier": EntityIdentifierTypeDef,
     },
 )
 _OptionalEntityItemTypeDef = TypedDict(
@@ -619,149 +764,34 @@
 
 class TemplateLinkedPolicyDefinitionTypeDef(
     _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
 ):
     pass
 
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
-    },
-    total=False,
-)
-
-CreateIdentitySourceOutputTypeDef = TypedDict(
-    "CreateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePolicyStoreOutputTypeDef = TypedDict(
-    "CreatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePolicyTemplateOutputTypeDef = TypedDict(
-    "CreatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPolicyTemplateOutputTypeDef = TypedDict(
-    "GetPolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "description": str,
-        "statement": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaOutputTypeDef = TypedDict(
-    "GetSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "schema": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSchemaOutputTypeDef = TypedDict(
-    "PutSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "namespaces": List[str],
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateIdentitySourceOutputTypeDef = TypedDict(
-    "UpdateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePolicyOutputTypeDef = TypedDict(
     "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
     {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
     },
@@ -785,15 +815,15 @@
     "GetPolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
         "arn": str,
         "validationSettings": ValidationSettingsTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -803,144 +833,114 @@
 
 IsAuthorizedOutputTypeDef = TypedDict(
     "IsAuthorizedOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
-    "_RequiredListIdentitySourcesInputRequestTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
-    "_OptionalListIdentitySourcesInputRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "filters": Sequence[IdentitySourceFilterTypeDef],
-    },
-    total=False,
-)
-
-
-class ListIdentitySourcesInputRequestTypeDef(
-    _RequiredListIdentitySourcesInputRequestTypeDef, _OptionalListIdentitySourcesInputRequestTypeDef
-):
-    pass
-
-
-IdentitySourceItemTypeDef = TypedDict(
-    "IdentitySourceItemTypeDef",
-    {
-        "createdDate": datetime,
-        "details": IdentitySourceItemDetailsTypeDef,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "principalEntityType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
     "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     {
         "filters": Sequence[IdentitySourceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
     _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
 ):
     pass
 
 
-ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+_RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
+    "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
-_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+_OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
+    "_OptionalListIdentitySourcesInputRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+        "filters": Sequence[IdentitySourceFilterTypeDef],
     },
     total=False,
 )
 
 
-class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
-    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+class ListIdentitySourcesInputRequestTypeDef(
+    _RequiredListIdentitySourcesInputRequestTypeDef, _OptionalListIdentitySourcesInputRequestTypeDef
 ):
     pass
 
 
+IdentitySourceItemTypeDef = TypedDict(
+    "IdentitySourceItemTypeDef",
+    {
+        "createdDate": datetime,
+        "details": IdentitySourceItemDetailsTypeDef,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "principalEntityType": str,
+    },
+)
+
 ListPolicyStoresOutputTypeDef = TypedDict(
     "ListPolicyStoresOutputTypeDef",
     {
         "nextToken": str,
         "policyStores": List[PolicyStoreItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPolicyTemplatesOutputTypeDef = TypedDict(
     "ListPolicyTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "policyTemplates": List[PolicyTemplateItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1035,15 +1035,15 @@
 
 
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateIdentitySourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1134,15 +1134,15 @@
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "filter": PolicyFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListPoliciesInputListPoliciesPaginateTypeDef(
     _RequiredListPoliciesInputListPoliciesPaginateTypeDef,
@@ -1181,15 +1181,15 @@
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPolicyItemTypeDef = TypedDict(
     "_RequiredPolicyItemTypeDef",
     {
         "policyStoreId": str,
@@ -1237,10 +1237,10 @@
 
 
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions/type_defs.pyi` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,72 +27,72 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateIdentitySourceOutputTypeDef",
     "ValidationSettingsTypeDef",
+    "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
+    "CreatePolicyTemplateOutputTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
+    "GetPolicyTemplateOutputTypeDef",
     "GetSchemaInputRequestTypeDef",
+    "GetSchemaOutputTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
+    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
+    "PaginatorConfigTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
+    "PutSchemaOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
+    "UpdateIdentitySourceOutputTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
+    "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
+    "UpdatePolicyTemplateOutputTypeDef",
     "AttributeValueTypeDef",
+    "CreatePolicyOutputTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
-    "ConfigurationTypeDef",
-    "CreateIdentitySourceOutputTypeDef",
-    "CreatePolicyOutputTypeDef",
-    "CreatePolicyStoreOutputTypeDef",
-    "CreatePolicyTemplateOutputTypeDef",
-    "GetPolicyTemplateOutputTypeDef",
-    "GetSchemaOutputTypeDef",
-    "PutSchemaOutputTypeDef",
-    "UpdateIdentitySourceOutputTypeDef",
     "UpdatePolicyOutputTypeDef",
-    "UpdatePolicyStoreOutputTypeDef",
-    "UpdatePolicyTemplateOutputTypeDef",
+    "ConfigurationTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
     "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
+    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
-    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
-    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
@@ -152,32 +152,43 @@
     "ContextDefinitionTypeDef",
     {
         "contextMap": Mapping[str, "AttributeValueTypeDef"],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateIdentitySourceOutputTypeDef = TypedDict(
+    "CreateIdentitySourceOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
 )
 
+CreatePolicyStoreOutputTypeDef = TypedDict(
+    "CreatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "statement": str,
     },
 )
@@ -192,14 +203,25 @@
 
 class CreatePolicyTemplateInputRequestTypeDef(
     _RequiredCreatePolicyTemplateInputRequestTypeDef,
     _OptionalCreatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
+CreatePolicyTemplateOutputTypeDef = TypedDict(
+    "CreatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIdentitySourceInputRequestTypeDef = TypedDict(
     "DeleteIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
         "identitySourceId": str,
     },
 )
@@ -279,21 +301,45 @@
     "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
     },
 )
 
+GetPolicyTemplateOutputTypeDef = TypedDict(
+    "GetPolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "description": str,
+        "statement": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
+GetSchemaOutputTypeDef = TypedDict(
+    "GetSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "schema": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 IdentitySourceFilterTypeDef = TypedDict(
     "IdentitySourceFilterTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
@@ -305,20 +351,18 @@
         "userPoolArn": str,
         "discoveryUrl": str,
         "openIdIssuer": Literal["COGNITO"],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPolicyStoresInputRequestTypeDef = TypedDict(
     "ListPolicyStoresInputRequestTypeDef",
     {
@@ -333,14 +377,34 @@
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
     },
 )
 
+_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
+    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+):
+    pass
+
 _RequiredListPolicyTemplatesInputRequestTypeDef = TypedDict(
     "_RequiredListPolicyTemplatesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPolicyTemplatesInputRequestTypeDef = TypedDict(
@@ -375,14 +439,24 @@
 )
 
 class PolicyTemplateItemTypeDef(
     _RequiredPolicyTemplateItemTypeDef, _OptionalPolicyTemplateItemTypeDef
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
 _RequiredStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredStaticPolicyDefinitionDetailTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalStaticPolicyDefinitionDetailTypeDef = TypedDict(
@@ -429,14 +503,36 @@
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": str,
     },
     total=False,
 )
 
+PutSchemaOutputTypeDef = TypedDict(
+    "PutSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "namespaces": List[str],
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
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
 _RequiredUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_RequiredUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "userPoolArn": str,
     },
 )
 _OptionalUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
@@ -449,14 +545,25 @@
 
 class UpdateCognitoUserPoolConfigurationTypeDef(
     _RequiredUpdateCognitoUserPoolConfigurationTypeDef,
     _OptionalUpdateCognitoUserPoolConfigurationTypeDef,
 ):
     pass
 
+UpdateIdentitySourceOutputTypeDef = TypedDict(
+    "UpdateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_RequiredUpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalUpdateStaticPolicyDefinitionTypeDef = TypedDict(
@@ -468,14 +575,25 @@
 )
 
 class UpdateStaticPolicyDefinitionTypeDef(
     _RequiredUpdateStaticPolicyDefinitionTypeDef, _OptionalUpdateStaticPolicyDefinitionTypeDef
 ):
     pass
 
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "statement": str,
     },
@@ -490,27 +608,52 @@
 
 class UpdatePolicyTemplateInputRequestTypeDef(
     _RequiredUpdatePolicyTemplateInputRequestTypeDef,
     _OptionalUpdatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "boolean": bool,
         "entityIdentifier": EntityIdentifierTypeDef,
         "long": int,
         "string": str,
         "set": Sequence[Dict[str, Any]],
         "record": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEntityItemTypeDef = TypedDict(
     "_RequiredEntityItemTypeDef",
     {
         "identifier": EntityIdentifierTypeDef,
     },
 )
 _OptionalEntityItemTypeDef = TypedDict(
@@ -592,149 +735,34 @@
 )
 
 class TemplateLinkedPolicyDefinitionTypeDef(
     _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
 ):
     pass
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
-    },
-    total=False,
-)
-
-CreateIdentitySourceOutputTypeDef = TypedDict(
-    "CreateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePolicyStoreOutputTypeDef = TypedDict(
-    "CreatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePolicyTemplateOutputTypeDef = TypedDict(
-    "CreatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPolicyTemplateOutputTypeDef = TypedDict(
-    "GetPolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "description": str,
-        "statement": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaOutputTypeDef = TypedDict(
-    "GetSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "schema": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSchemaOutputTypeDef = TypedDict(
-    "PutSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "namespaces": List[str],
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateIdentitySourceOutputTypeDef = TypedDict(
-    "UpdateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdatePolicyOutputTypeDef = TypedDict(
     "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
     {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
     },
@@ -756,15 +784,15 @@
     "GetPolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
         "arn": str,
         "validationSettings": ValidationSettingsTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -774,41 +802,62 @@
 
 IsAuthorizedOutputTypeDef = TypedDict(
     "IsAuthorizedOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "filters": Sequence[IdentitySourceFilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
+    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
@@ -834,78 +883,29 @@
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
     },
 )
 
-_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    {
-        "filters": Sequence[IdentitySourceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
-    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-):
-    pass
-
-ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
-    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-):
-    pass
-
 ListPolicyStoresOutputTypeDef = TypedDict(
     "ListPolicyStoresOutputTypeDef",
     {
         "nextToken": str,
         "policyStores": List[PolicyStoreItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPolicyTemplatesOutputTypeDef = TypedDict(
     "ListPolicyTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "policyTemplates": List[PolicyTemplateItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -998,15 +998,15 @@
     pass
 
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateIdentitySourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1091,15 +1091,15 @@
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "filter": PolicyFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListPoliciesInputListPoliciesPaginateTypeDef(
     _RequiredListPoliciesInputListPoliciesPaginateTypeDef,
     _OptionalListPoliciesInputListPoliciesPaginateTypeDef,
@@ -1134,15 +1134,15 @@
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPolicyItemTypeDef = TypedDict(
     "_RequiredPolicyItemTypeDef",
     {
         "policyStoreId": str,
@@ -1186,10 +1186,10 @@
     pass
 
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.26.165
-Summary: Type annotations for boto3.VerifiedPermissions 1.26.165 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.VerifiedPermissions 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.26.165](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -343,72 +343,72 @@
 
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateIdentitySourceOutputTypeDef,
     ValidationSettingsTypeDef,
+    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
+    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
+    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
+    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
+    PutSchemaOutputTypeDef,
+    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
+    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
-    ConfigurationTypeDef,
-    CreateIdentitySourceOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    CreatePolicyStoreOutputTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
-    GetPolicyTemplateOutputTypeDef,
-    GetSchemaOutputTypeDef,
-    PutSchemaOutputTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdatePolicyOutputTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
+    ConfigurationTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
     GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
```

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt` & `mypy-boto3-verifiedpermissions-1.27.0/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.26.165/setup.py` & `mypy-boto3-verifiedpermissions-1.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-verifiedpermissions",
-    version="1.26.165",
+    version="1.27.0",
     packages=["mypy_boto3_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VerifiedPermissions 1.26.165 service generated with"
+        "Type annotations for boto3.VerifiedPermissions 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


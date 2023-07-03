# Comparing `tmp/mypy-boto3-payment-cryptography-1.26.150.tar.gz` & `tmp/mypy-boto3-payment-cryptography-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-1.26.150.tar", last modified: Thu Jun  8 19:32:29 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-1.27.0.tar", last modified: Mon Jul  3 19:51:14 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-1.26.150.tar` & `mypy-boto3-payment-cryptography-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.755941 mypy-boto3-payment-cryptography-1.26.150/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-06-08 19:32:29.747941 mypy-boto3-payment-cryptography-1.26.150/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.743941 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-06-08 19:32:13.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.747941 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:29.755941 mypy-boto3-payment-cryptography-1.26.150/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-08 19:32:12.000000 mypy-boto3-payment-cryptography-1.26.150/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.463791 mypy-boto3-payment-cryptography-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-03 19:51:14.455791 mypy-boto3-payment-cryptography-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.447790 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.455791 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-03 19:51:14.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 19:51:14.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:14.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 19:51:14.000000 mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:14.463791 mypy-boto3-payment-cryptography-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 19:43:19.000000 mypy-boto3-payment-cryptography-1.27.0/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/LICENSE` & `mypy-boto3-payment-cryptography-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.26.150/PKG-INFO` & `mypy-boto3-payment-cryptography-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.26.150
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -340,53 +340,53 @@
 `mypy_boto3_payment_cryptography.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography.type_defs import (
     AliasTypeDef,
     CreateAliasInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAliasInputRequestTypeDef,
     DeleteKeyInputRequestTypeDef,
     ExportTr31KeyBlockTypeDef,
     ExportTr34KeyBlockTypeDef,
     WrappedKeyTypeDef,
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
+    GetParametersForExportOutputTypeDef,
     GetParametersForImportInputRequestTypeDef,
+    GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
+    GetPublicKeyCertificateOutputTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
     KeyModesOfUseTypeDef,
-    PaginatorConfigTypeDef,
+    ListAliasesInputListAliasesPaginateTypeDef,
     ListAliasesInputRequestTypeDef,
+    ListKeysInputListKeysPaginateTypeDef,
     ListKeysInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
-    GetParametersForExportOutputTypeDef,
-    GetParametersForImportOutputTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
     KeyAttributesTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ExportKeyInputRequestTypeDef,
     CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/README.md` & `mypy-boto3-payment-cryptography-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -308,53 +308,53 @@
 `mypy_boto3_payment_cryptography.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography.type_defs import (
     AliasTypeDef,
     CreateAliasInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAliasInputRequestTypeDef,
     DeleteKeyInputRequestTypeDef,
     ExportTr31KeyBlockTypeDef,
     ExportTr34KeyBlockTypeDef,
     WrappedKeyTypeDef,
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
+    GetParametersForExportOutputTypeDef,
     GetParametersForImportInputRequestTypeDef,
+    GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
+    GetPublicKeyCertificateOutputTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
     KeyModesOfUseTypeDef,
-    PaginatorConfigTypeDef,
+    ListAliasesInputListAliasesPaginateTypeDef,
     ListAliasesInputRequestTypeDef,
+    ListKeysInputListKeysPaginateTypeDef,
     ListKeysInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
-    GetParametersForExportOutputTypeDef,
-    GetParametersForImportOutputTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
     KeyAttributesTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ExportKeyInputRequestTypeDef,
     CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/__init__.py` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/__init__.pyi` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/__main__.py` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PaymentCryptographyControlPlane 1.26.150\nVersion:        "
-        " 1.26.150\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PaymentCryptographyControlPlane 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.150")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/client.py` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/client.pyi` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/literals.py` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
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
@@ -140,14 +141,15 @@
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
@@ -412,14 +414,15 @@
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

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/literals.pyi` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
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
@@ -138,14 +139,15 @@
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
@@ -410,14 +412,15 @@
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

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/paginator.py` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,43 +51,43 @@
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
         """
 
 
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, KeyState: KeyStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, KeyState: KeyStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/paginator.pyi` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,41 +48,41 @@
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
         """
 
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, KeyState: KeyStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, KeyState: KeyStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/type_defs.py` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,53 +35,53 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
     "ExportTr31KeyBlockTypeDef",
     "ExportTr34KeyBlockTypeDef",
     "WrappedKeyTypeDef",
     "GetAliasInputRequestTypeDef",
     "GetKeyInputRequestTypeDef",
     "GetParametersForExportInputRequestTypeDef",
+    "GetParametersForExportOutputTypeDef",
     "GetParametersForImportInputRequestTypeDef",
+    "GetParametersForImportOutputTypeDef",
     "GetPublicKeyCertificateInputRequestTypeDef",
+    "GetPublicKeyCertificateOutputTypeDef",
     "ImportTr31KeyBlockTypeDef",
     "ImportTr34KeyBlockTypeDef",
     "KeyModesOfUseTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAliasesInputListAliasesPaginateTypeDef",
     "ListAliasesInputRequestTypeDef",
+    "ListKeysInputListKeysPaginateTypeDef",
     "ListKeysInputRequestTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreKeyInputRequestTypeDef",
     "StartKeyUsageInputRequestTypeDef",
     "StopKeyUsageInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "CreateAliasOutputTypeDef",
     "GetAliasOutputTypeDef",
-    "GetParametersForExportOutputTypeDef",
-    "GetParametersForImportOutputTypeDef",
-    "GetPublicKeyCertificateOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ExportKeyMaterialTypeDef",
     "ExportKeyOutputTypeDef",
     "KeyAttributesTypeDef",
-    "ListAliasesInputListAliasesPaginateTypeDef",
-    "ListKeysInputListKeysPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ExportKeyInputRequestTypeDef",
     "CreateKeyInputRequestTypeDef",
     "KeySummaryTypeDef",
     "KeyTypeDef",
     "RootCertificatePublicKeyTypeDef",
     "TrustedCertificatePublicKeyTypeDef",
     "ListKeysOutputTypeDef",
@@ -132,25 +132,14 @@
 
 class CreateAliasInputRequestTypeDef(
     _RequiredCreateAliasInputRequestTypeDef, _OptionalCreateAliasInputRequestTypeDef
 ):
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
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -252,29 +241,62 @@
     "GetParametersForExportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "SigningKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
+GetParametersForExportOutputTypeDef = TypedDict(
+    "GetParametersForExportOutputTypeDef",
+    {
+        "ExportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "SigningKeyAlgorithm": KeyAlgorithmType,
+        "SigningKeyCertificate": str,
+        "SigningKeyCertificateChain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetParametersForImportInputRequestTypeDef = TypedDict(
     "GetParametersForImportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "WrappingKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
+GetParametersForImportOutputTypeDef = TypedDict(
+    "GetParametersForImportOutputTypeDef",
+    {
+        "ImportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "WrappingKeyAlgorithm": KeyAlgorithmType,
+        "WrappingKeyCertificate": str,
+        "WrappingKeyCertificateChain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPublicKeyCertificateInputRequestTypeDef = TypedDict(
     "GetPublicKeyCertificateInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
+GetPublicKeyCertificateOutputTypeDef = TypedDict(
+    "GetPublicKeyCertificateOutputTypeDef",
+    {
+        "KeyCertificate": str,
+        "KeyCertificateChain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImportTr31KeyBlockTypeDef = TypedDict(
     "ImportTr31KeyBlockTypeDef",
     {
         "WrappedKeyBlock": str,
         "WrappingKeyIdentifier": str,
     },
 )
@@ -316,43 +338,72 @@
         "Unwrap": bool,
         "Verify": bool,
         "Wrap": bool,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesInputListAliasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAliasesInputRequestTypeDef = TypedDict(
     "ListAliasesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListKeysInputListKeysPaginateTypeDef = TypedDict(
+    "ListKeysInputListKeysPaginateTypeDef",
+    {
+        "KeyState": KeyStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKeysInputRequestTypeDef = TypedDict(
     "ListKeysInputRequestTypeDef",
     {
         "KeyState": KeyStateType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -367,14 +418,35 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 RestoreKeyInputRequestTypeDef = TypedDict(
     "RestoreKeyInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
@@ -421,82 +493,49 @@
     pass
 
 
 CreateAliasOutputTypeDef = TypedDict(
     "CreateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAliasOutputTypeDef = TypedDict(
     "GetAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetParametersForExportOutputTypeDef = TypedDict(
-    "GetParametersForExportOutputTypeDef",
-    {
-        "ExportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "SigningKeyAlgorithm": KeyAlgorithmType,
-        "SigningKeyCertificate": str,
-        "SigningKeyCertificateChain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetParametersForImportOutputTypeDef = TypedDict(
-    "GetParametersForImportOutputTypeDef",
-    {
-        "ImportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "WrappingKeyAlgorithm": KeyAlgorithmType,
-        "WrappingKeyCertificate": str,
-        "WrappingKeyCertificateChain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPublicKeyCertificateOutputTypeDef = TypedDict(
-    "GetPublicKeyCertificateOutputTypeDef",
-    {
-        "KeyCertificate": str,
-        "KeyCertificateChain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAliasesOutputTypeDef = TypedDict(
     "ListAliasesOutputTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAliasOutputTypeDef = TypedDict(
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
@@ -513,67 +552,28 @@
     total=False,
 )
 
 ExportKeyOutputTypeDef = TypedDict(
     "ExportKeyOutputTypeDef",
     {
         "WrappedKey": WrappedKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KeyAttributesTypeDef = TypedDict(
     "KeyAttributesTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "KeyClass": KeyClassType,
         "KeyModesOfUse": KeyModesOfUseTypeDef,
         "KeyUsage": KeyUsageType,
     },
 )
 
-ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesInputListAliasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKeysInputListKeysPaginateTypeDef = TypedDict(
-    "ListKeysInputListKeysPaginateTypeDef",
-    {
-        "KeyState": KeyStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 ExportKeyInputRequestTypeDef = TypedDict(
     "ExportKeyInputRequestTypeDef",
     {
         "ExportKeyIdentifier": str,
         "KeyMaterial": ExportKeyMaterialTypeDef,
     },
 )
@@ -662,71 +662,71 @@
 )
 
 ListKeysOutputTypeDef = TypedDict(
     "ListKeysOutputTypeDef",
     {
         "Keys": List[KeySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateKeyOutputTypeDef = TypedDict(
     "CreateKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKeyOutputTypeDef = TypedDict(
     "DeleteKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyOutputTypeDef = TypedDict(
     "GetKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportKeyOutputTypeDef = TypedDict(
     "ImportKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreKeyOutputTypeDef = TypedDict(
     "RestoreKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartKeyUsageOutputTypeDef = TypedDict(
     "StartKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopKeyUsageOutputTypeDef = TypedDict(
     "StopKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportKeyMaterialTypeDef = TypedDict(
     "ImportKeyMaterialTypeDef",
     {
         "RootCertificatePublicKey": RootCertificatePublicKeyTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography/type_defs.pyi` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,53 +34,53 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
     "ExportTr31KeyBlockTypeDef",
     "ExportTr34KeyBlockTypeDef",
     "WrappedKeyTypeDef",
     "GetAliasInputRequestTypeDef",
     "GetKeyInputRequestTypeDef",
     "GetParametersForExportInputRequestTypeDef",
+    "GetParametersForExportOutputTypeDef",
     "GetParametersForImportInputRequestTypeDef",
+    "GetParametersForImportOutputTypeDef",
     "GetPublicKeyCertificateInputRequestTypeDef",
+    "GetPublicKeyCertificateOutputTypeDef",
     "ImportTr31KeyBlockTypeDef",
     "ImportTr34KeyBlockTypeDef",
     "KeyModesOfUseTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAliasesInputListAliasesPaginateTypeDef",
     "ListAliasesInputRequestTypeDef",
+    "ListKeysInputListKeysPaginateTypeDef",
     "ListKeysInputRequestTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreKeyInputRequestTypeDef",
     "StartKeyUsageInputRequestTypeDef",
     "StopKeyUsageInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "CreateAliasOutputTypeDef",
     "GetAliasOutputTypeDef",
-    "GetParametersForExportOutputTypeDef",
-    "GetParametersForImportOutputTypeDef",
-    "GetPublicKeyCertificateOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ExportKeyMaterialTypeDef",
     "ExportKeyOutputTypeDef",
     "KeyAttributesTypeDef",
-    "ListAliasesInputListAliasesPaginateTypeDef",
-    "ListKeysInputListKeysPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ExportKeyInputRequestTypeDef",
     "CreateKeyInputRequestTypeDef",
     "KeySummaryTypeDef",
     "KeyTypeDef",
     "RootCertificatePublicKeyTypeDef",
     "TrustedCertificatePublicKeyTypeDef",
     "ListKeysOutputTypeDef",
@@ -127,25 +127,14 @@
 )
 
 class CreateAliasInputRequestTypeDef(
     _RequiredCreateAliasInputRequestTypeDef, _OptionalCreateAliasInputRequestTypeDef
 ):
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
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -241,29 +230,62 @@
     "GetParametersForExportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "SigningKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
+GetParametersForExportOutputTypeDef = TypedDict(
+    "GetParametersForExportOutputTypeDef",
+    {
+        "ExportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "SigningKeyAlgorithm": KeyAlgorithmType,
+        "SigningKeyCertificate": str,
+        "SigningKeyCertificateChain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetParametersForImportInputRequestTypeDef = TypedDict(
     "GetParametersForImportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "WrappingKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
+GetParametersForImportOutputTypeDef = TypedDict(
+    "GetParametersForImportOutputTypeDef",
+    {
+        "ImportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "WrappingKeyAlgorithm": KeyAlgorithmType,
+        "WrappingKeyCertificate": str,
+        "WrappingKeyCertificateChain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetPublicKeyCertificateInputRequestTypeDef = TypedDict(
     "GetPublicKeyCertificateInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
+GetPublicKeyCertificateOutputTypeDef = TypedDict(
+    "GetPublicKeyCertificateOutputTypeDef",
+    {
+        "KeyCertificate": str,
+        "KeyCertificateChain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImportTr31KeyBlockTypeDef = TypedDict(
     "ImportTr31KeyBlockTypeDef",
     {
         "WrappedKeyBlock": str,
         "WrappingKeyIdentifier": str,
     },
 )
@@ -303,43 +325,70 @@
         "Unwrap": bool,
         "Verify": bool,
         "Wrap": bool,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesInputListAliasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAliasesInputRequestTypeDef = TypedDict(
     "ListAliasesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListKeysInputListKeysPaginateTypeDef = TypedDict(
+    "ListKeysInputListKeysPaginateTypeDef",
+    {
+        "KeyState": KeyStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKeysInputRequestTypeDef = TypedDict(
     "ListKeysInputRequestTypeDef",
     {
         "KeyState": KeyStateType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -352,14 +401,35 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 RestoreKeyInputRequestTypeDef = TypedDict(
     "RestoreKeyInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
@@ -404,82 +474,49 @@
 ):
     pass
 
 CreateAliasOutputTypeDef = TypedDict(
     "CreateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAliasOutputTypeDef = TypedDict(
     "GetAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetParametersForExportOutputTypeDef = TypedDict(
-    "GetParametersForExportOutputTypeDef",
-    {
-        "ExportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "SigningKeyAlgorithm": KeyAlgorithmType,
-        "SigningKeyCertificate": str,
-        "SigningKeyCertificateChain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetParametersForImportOutputTypeDef = TypedDict(
-    "GetParametersForImportOutputTypeDef",
-    {
-        "ImportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "WrappingKeyAlgorithm": KeyAlgorithmType,
-        "WrappingKeyCertificate": str,
-        "WrappingKeyCertificateChain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPublicKeyCertificateOutputTypeDef = TypedDict(
-    "GetPublicKeyCertificateOutputTypeDef",
-    {
-        "KeyCertificate": str,
-        "KeyCertificateChain": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAliasesOutputTypeDef = TypedDict(
     "ListAliasesOutputTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAliasOutputTypeDef = TypedDict(
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
@@ -496,65 +533,28 @@
     total=False,
 )
 
 ExportKeyOutputTypeDef = TypedDict(
     "ExportKeyOutputTypeDef",
     {
         "WrappedKey": WrappedKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KeyAttributesTypeDef = TypedDict(
     "KeyAttributesTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "KeyClass": KeyClassType,
         "KeyModesOfUse": KeyModesOfUseTypeDef,
         "KeyUsage": KeyUsageType,
     },
 )
 
-ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesInputListAliasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKeysInputListKeysPaginateTypeDef = TypedDict(
-    "ListKeysInputListKeysPaginateTypeDef",
-    {
-        "KeyState": KeyStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 ExportKeyInputRequestTypeDef = TypedDict(
     "ExportKeyInputRequestTypeDef",
     {
         "ExportKeyIdentifier": str,
         "KeyMaterial": ExportKeyMaterialTypeDef,
     },
 )
@@ -639,71 +639,71 @@
 )
 
 ListKeysOutputTypeDef = TypedDict(
     "ListKeysOutputTypeDef",
     {
         "Keys": List[KeySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateKeyOutputTypeDef = TypedDict(
     "CreateKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteKeyOutputTypeDef = TypedDict(
     "DeleteKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyOutputTypeDef = TypedDict(
     "GetKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportKeyOutputTypeDef = TypedDict(
     "ImportKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreKeyOutputTypeDef = TypedDict(
     "RestoreKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartKeyUsageOutputTypeDef = TypedDict(
     "StartKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopKeyUsageOutputTypeDef = TypedDict(
     "StopKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportKeyMaterialTypeDef = TypedDict(
     "ImportKeyMaterialTypeDef",
     {
         "RootCertificatePublicKey": RootCertificatePublicKeyTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.26.150
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -340,53 +340,53 @@
 `mypy_boto3_payment_cryptography.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography.type_defs import (
     AliasTypeDef,
     CreateAliasInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAliasInputRequestTypeDef,
     DeleteKeyInputRequestTypeDef,
     ExportTr31KeyBlockTypeDef,
     ExportTr34KeyBlockTypeDef,
     WrappedKeyTypeDef,
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
+    GetParametersForExportOutputTypeDef,
     GetParametersForImportInputRequestTypeDef,
+    GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
+    GetPublicKeyCertificateOutputTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
     KeyModesOfUseTypeDef,
-    PaginatorConfigTypeDef,
+    ListAliasesInputListAliasesPaginateTypeDef,
     ListAliasesInputRequestTypeDef,
+    ListKeysInputListKeysPaginateTypeDef,
     ListKeysInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
-    GetParametersForExportOutputTypeDef,
-    GetParametersForImportOutputTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
     KeyAttributesTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ExportKeyInputRequestTypeDef,
     CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.26.150/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-1.27.0/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.26.150/setup.py` & `mypy-boto3-payment-cryptography-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography",
-    version="1.26.150",
+    version="1.27.0",
     packages=["mypy_boto3_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PaymentCryptographyControlPlane 1.26.150 service generated with"
+        "Type annotations for boto3.PaymentCryptographyControlPlane 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


# Comparing `tmp/mypy-boto3-payment-cryptography-data-1.26.150.tar.gz` & `tmp/mypy-boto3-payment-cryptography-data-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-data-1.26.150.tar", last modified: Thu Jun  8 19:32:29 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-data-1.27.0.tar", last modified: Mon Jul  3 19:51:13 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-data-1.26.150.tar` & `mypy-boto3-payment-cryptography-data-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.699941 mypy-boto3-payment-cryptography-data-1.26.150/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-06-08 19:32:29.699941 mypy-boto3-payment-cryptography-data-1.26.150/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.695940 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-06-08 19:32:11.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-06-08 19:32:11.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.699941 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 19:32:29.000000 mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:29.699941 mypy-boto3-payment-cryptography-data-1.26.150/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-08 19:32:10.000000 mypy-boto3-payment-cryptography-data-1.26.150/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.291772 mypy-boto3-payment-cryptography-data-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-03 19:51:13.291772 mypy-boto3-payment-cryptography-data-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.291772 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.291772 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-03 19:51:13.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-03 19:51:13.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:13.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 19:51:13.000000 mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:13.291772 mypy-boto3-payment-cryptography-data-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-03 19:43:20.000000 mypy-boto3-payment-cryptography-data-1.27.0/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/LICENSE` & `mypy-boto3-payment-cryptography-data-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/PKG-INFO` & `mypy-boto3-payment-cryptography-data-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography-data
-Version: 1.26.150
-Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography-data?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -316,49 +316,49 @@
     CardVerificationValue1TypeDef,
     CardVerificationValue2TypeDef,
     DynamicCardVerificationCodeTypeDef,
     DynamicCardVerificationValueTypeDef,
     DiscoverDynamicCardVerificationCodeTypeDef,
     CryptogramVerificationArpcMethod1TypeDef,
     CryptogramVerificationArpcMethod2TypeDef,
-    ResponseMetadataTypeDef,
+    DecryptDataOutputTypeDef,
     DukptAttributesTypeDef,
     DukptDerivationAttributesTypeDef,
     DukptEncryptionAttributesTypeDef,
+    EncryptDataOutputTypeDef,
     SymmetricEncryptionAttributesTypeDef,
+    GenerateCardValidationDataOutputTypeDef,
+    GenerateMacOutputTypeDef,
     PinDataTypeDef,
     Ibm3624NaturalPinTypeDef,
     Ibm3624PinFromOffsetTypeDef,
     Ibm3624PinOffsetTypeDef,
     Ibm3624PinVerificationTypeDef,
     Ibm3624RandomPinTypeDef,
     MacAlgorithmDukptTypeDef,
     SessionKeyDerivationValueTypeDef,
     VisaPinTypeDef,
     VisaPinVerificationValueTypeDef,
     VisaPinVerificationTypeDef,
+    ReEncryptDataOutputTypeDef,
+    ResponseMetadataTypeDef,
     SessionKeyAmexTypeDef,
     SessionKeyEmv2000TypeDef,
     SessionKeyEmvCommonTypeDef,
     SessionKeyMastercardTypeDef,
     SessionKeyVisaTypeDef,
-    TranslationPinDataIsoFormat034TypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
-    DecryptDataOutputTypeDef,
-    EncryptDataOutputTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
-    ReEncryptDataOutputTypeDef,
     TranslatePinDataOutputTypeDef,
+    TranslationPinDataIsoFormat034TypeDef,
     VerifyAuthRequestCryptogramOutputTypeDef,
     VerifyCardValidationDataOutputTypeDef,
     VerifyMacOutputTypeDef,
     VerifyPinDataOutputTypeDef,
+    CardGenerationAttributesTypeDef,
+    CardVerificationAttributesTypeDef,
+    CryptogramAuthResponseTypeDef,
     EncryptionDecryptionAttributesTypeDef,
     ReEncryptionAttributesTypeDef,
     GeneratePinDataOutputTypeDef,
     MacAlgorithmEmvTypeDef,
     PinGenerationAttributesTypeDef,
     PinVerificationAttributesTypeDef,
     SessionKeyDerivationTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/README.md` & `mypy-boto3-payment-cryptography-data-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography-data?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -284,49 +284,49 @@
     CardVerificationValue1TypeDef,
     CardVerificationValue2TypeDef,
     DynamicCardVerificationCodeTypeDef,
     DynamicCardVerificationValueTypeDef,
     DiscoverDynamicCardVerificationCodeTypeDef,
     CryptogramVerificationArpcMethod1TypeDef,
     CryptogramVerificationArpcMethod2TypeDef,
-    ResponseMetadataTypeDef,
+    DecryptDataOutputTypeDef,
     DukptAttributesTypeDef,
     DukptDerivationAttributesTypeDef,
     DukptEncryptionAttributesTypeDef,
+    EncryptDataOutputTypeDef,
     SymmetricEncryptionAttributesTypeDef,
+    GenerateCardValidationDataOutputTypeDef,
+    GenerateMacOutputTypeDef,
     PinDataTypeDef,
     Ibm3624NaturalPinTypeDef,
     Ibm3624PinFromOffsetTypeDef,
     Ibm3624PinOffsetTypeDef,
     Ibm3624PinVerificationTypeDef,
     Ibm3624RandomPinTypeDef,
     MacAlgorithmDukptTypeDef,
     SessionKeyDerivationValueTypeDef,
     VisaPinTypeDef,
     VisaPinVerificationValueTypeDef,
     VisaPinVerificationTypeDef,
+    ReEncryptDataOutputTypeDef,
+    ResponseMetadataTypeDef,
     SessionKeyAmexTypeDef,
     SessionKeyEmv2000TypeDef,
     SessionKeyEmvCommonTypeDef,
     SessionKeyMastercardTypeDef,
     SessionKeyVisaTypeDef,
-    TranslationPinDataIsoFormat034TypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
-    DecryptDataOutputTypeDef,
-    EncryptDataOutputTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
-    ReEncryptDataOutputTypeDef,
     TranslatePinDataOutputTypeDef,
+    TranslationPinDataIsoFormat034TypeDef,
     VerifyAuthRequestCryptogramOutputTypeDef,
     VerifyCardValidationDataOutputTypeDef,
     VerifyMacOutputTypeDef,
     VerifyPinDataOutputTypeDef,
+    CardGenerationAttributesTypeDef,
+    CardVerificationAttributesTypeDef,
+    CryptogramAuthResponseTypeDef,
     EncryptionDecryptionAttributesTypeDef,
     ReEncryptionAttributesTypeDef,
     GeneratePinDataOutputTypeDef,
     MacAlgorithmEmvTypeDef,
     PinGenerationAttributesTypeDef,
     PinVerificationAttributesTypeDef,
     SessionKeyDerivationTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/__init__.py` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/__init__.pyi` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/__main__.py` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PaymentCryptographyDataPlane 1.26.150\nVersion:        "
-        " 1.26.150\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PaymentCryptographyDataPlane 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane\nOther"
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

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/client.py` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/client.pyi` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/literals.py` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
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
@@ -113,14 +114,15 @@
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
@@ -385,14 +387,15 @@
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

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/literals.pyi` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
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
@@ -111,14 +112,15 @@
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
@@ -383,14 +385,15 @@
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

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/type_defs.py` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,62 +27,61 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AmexCardSecurityCodeVersion1TypeDef",
     "AmexCardSecurityCodeVersion2TypeDef",
     "AsymmetricEncryptionAttributesTypeDef",
     "CardHolderVerificationValueTypeDef",
     "CardVerificationValue1TypeDef",
     "CardVerificationValue2TypeDef",
     "DynamicCardVerificationCodeTypeDef",
     "DynamicCardVerificationValueTypeDef",
     "DiscoverDynamicCardVerificationCodeTypeDef",
     "CryptogramVerificationArpcMethod1TypeDef",
     "CryptogramVerificationArpcMethod2TypeDef",
-    "ResponseMetadataTypeDef",
+    "DecryptDataOutputTypeDef",
     "DukptAttributesTypeDef",
     "DukptDerivationAttributesTypeDef",
     "DukptEncryptionAttributesTypeDef",
+    "EncryptDataOutputTypeDef",
     "SymmetricEncryptionAttributesTypeDef",
+    "GenerateCardValidationDataOutputTypeDef",
+    "GenerateMacOutputTypeDef",
     "PinDataTypeDef",
     "Ibm3624NaturalPinTypeDef",
     "Ibm3624PinFromOffsetTypeDef",
     "Ibm3624PinOffsetTypeDef",
     "Ibm3624PinVerificationTypeDef",
     "Ibm3624RandomPinTypeDef",
     "MacAlgorithmDukptTypeDef",
     "SessionKeyDerivationValueTypeDef",
     "VisaPinTypeDef",
     "VisaPinVerificationValueTypeDef",
     "VisaPinVerificationTypeDef",
+    "ReEncryptDataOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SessionKeyAmexTypeDef",
     "SessionKeyEmv2000TypeDef",
     "SessionKeyEmvCommonTypeDef",
     "SessionKeyMastercardTypeDef",
     "SessionKeyVisaTypeDef",
-    "TranslationPinDataIsoFormat034TypeDef",
-    "CardGenerationAttributesTypeDef",
-    "CardVerificationAttributesTypeDef",
-    "CryptogramAuthResponseTypeDef",
-    "DecryptDataOutputTypeDef",
-    "EncryptDataOutputTypeDef",
-    "GenerateCardValidationDataOutputTypeDef",
-    "GenerateMacOutputTypeDef",
-    "ReEncryptDataOutputTypeDef",
     "TranslatePinDataOutputTypeDef",
+    "TranslationPinDataIsoFormat034TypeDef",
     "VerifyAuthRequestCryptogramOutputTypeDef",
     "VerifyCardValidationDataOutputTypeDef",
     "VerifyMacOutputTypeDef",
     "VerifyPinDataOutputTypeDef",
+    "CardGenerationAttributesTypeDef",
+    "CardVerificationAttributesTypeDef",
+    "CryptogramAuthResponseTypeDef",
     "EncryptionDecryptionAttributesTypeDef",
     "ReEncryptionAttributesTypeDef",
     "GeneratePinDataOutputTypeDef",
     "MacAlgorithmEmvTypeDef",
     "PinGenerationAttributesTypeDef",
     "PinVerificationAttributesTypeDef",
     "SessionKeyDerivationTypeDef",
@@ -194,30 +193,27 @@
     "_OptionalCryptogramVerificationArpcMethod2TypeDef",
     {
         "ProprietaryAuthenticationData": str,
     },
     total=False,
 )
 
-
 class CryptogramVerificationArpcMethod2TypeDef(
     _RequiredCryptogramVerificationArpcMethod2TypeDef,
     _OptionalCryptogramVerificationArpcMethod2TypeDef,
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DecryptDataOutputTypeDef = TypedDict(
+    "DecryptDataOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "PlainText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DukptAttributesTypeDef = TypedDict(
     "DukptAttributesTypeDef",
     {
         "DukptDerivationType": DukptDerivationTypeType,
@@ -236,21 +232,19 @@
     {
         "DukptKeyDerivationType": DukptDerivationTypeType,
         "DukptKeyVariant": DukptKeyVariantType,
     },
     total=False,
 )
 
-
 class DukptDerivationAttributesTypeDef(
     _RequiredDukptDerivationAttributesTypeDef, _OptionalDukptDerivationAttributesTypeDef
 ):
     pass
 
-
 _RequiredDukptEncryptionAttributesTypeDef = TypedDict(
     "_RequiredDukptEncryptionAttributesTypeDef",
     {
         "KeySerialNumber": str,
     },
 )
 _OptionalDukptEncryptionAttributesTypeDef = TypedDict(
@@ -260,20 +254,28 @@
         "DukptKeyVariant": DukptKeyVariantType,
         "InitializationVector": str,
         "Mode": DukptEncryptionModeType,
     },
     total=False,
 )
 
-
 class DukptEncryptionAttributesTypeDef(
     _RequiredDukptEncryptionAttributesTypeDef, _OptionalDukptEncryptionAttributesTypeDef
 ):
     pass
 
+EncryptDataOutputTypeDef = TypedDict(
+    "EncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredSymmetricEncryptionAttributesTypeDef = TypedDict(
     "_RequiredSymmetricEncryptionAttributesTypeDef",
     {
         "Mode": EncryptionModeType,
     },
 )
@@ -282,20 +284,38 @@
     {
         "InitializationVector": str,
         "PaddingType": PaddingTypeType,
     },
     total=False,
 )
 
-
 class SymmetricEncryptionAttributesTypeDef(
     _RequiredSymmetricEncryptionAttributesTypeDef, _OptionalSymmetricEncryptionAttributesTypeDef
 ):
     pass
 
+GenerateCardValidationDataOutputTypeDef = TypedDict(
+    "GenerateCardValidationDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ValidationData": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GenerateMacOutputTypeDef = TypedDict(
+    "GenerateMacOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "Mac": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 PinDataTypeDef = TypedDict(
     "PinDataTypeDef",
     {
         "PinOffset": str,
         "VerificationValue": str,
     },
@@ -361,21 +381,19 @@
     "_OptionalMacAlgorithmDukptTypeDef",
     {
         "DukptDerivationType": DukptDerivationTypeType,
     },
     total=False,
 )
 
-
 class MacAlgorithmDukptTypeDef(
     _RequiredMacAlgorithmDukptTypeDef, _OptionalMacAlgorithmDukptTypeDef
 ):
     pass
 
-
 SessionKeyDerivationValueTypeDef = TypedDict(
     "SessionKeyDerivationValueTypeDef",
     {
         "ApplicationCryptogram": str,
         "ApplicationTransactionCounter": str,
     },
     total=False,
@@ -400,14 +418,35 @@
     "VisaPinVerificationTypeDef",
     {
         "PinVerificationKeyIndex": int,
         "VerificationValue": str,
     },
 )
 
+ReEncryptDataOutputTypeDef = TypedDict(
+    "ReEncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
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
 SessionKeyAmexTypeDef = TypedDict(
     "SessionKeyAmexTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
@@ -444,156 +483,106 @@
     "SessionKeyVisaTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
 
-TranslationPinDataIsoFormat034TypeDef = TypedDict(
-    "TranslationPinDataIsoFormat034TypeDef",
-    {
-        "PrimaryAccountNumber": str,
-    },
-)
-
-CardGenerationAttributesTypeDef = TypedDict(
-    "CardGenerationAttributesTypeDef",
-    {
-        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
-        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
-        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
-        "CardVerificationValue1": CardVerificationValue1TypeDef,
-        "CardVerificationValue2": CardVerificationValue2TypeDef,
-        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
-        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
-    },
-    total=False,
-)
-
-CardVerificationAttributesTypeDef = TypedDict(
-    "CardVerificationAttributesTypeDef",
-    {
-        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
-        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
-        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
-        "CardVerificationValue1": CardVerificationValue1TypeDef,
-        "CardVerificationValue2": CardVerificationValue2TypeDef,
-        "DiscoverDynamicCardVerificationCode": DiscoverDynamicCardVerificationCodeTypeDef,
-        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
-        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
-    },
-    total=False,
-)
-
-CryptogramAuthResponseTypeDef = TypedDict(
-    "CryptogramAuthResponseTypeDef",
-    {
-        "ArpcMethod1": CryptogramVerificationArpcMethod1TypeDef,
-        "ArpcMethod2": CryptogramVerificationArpcMethod2TypeDef,
-    },
-    total=False,
-)
-
-DecryptDataOutputTypeDef = TypedDict(
-    "DecryptDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PlainText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EncryptDataOutputTypeDef = TypedDict(
-    "EncryptDataOutputTypeDef",
-    {
-        "CipherText": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GenerateCardValidationDataOutputTypeDef = TypedDict(
-    "GenerateCardValidationDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ValidationData": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GenerateMacOutputTypeDef = TypedDict(
-    "GenerateMacOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "Mac": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReEncryptDataOutputTypeDef = TypedDict(
-    "ReEncryptDataOutputTypeDef",
+TranslatePinDataOutputTypeDef = TypedDict(
+    "TranslatePinDataOutputTypeDef",
     {
-        "CipherText": str,
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PinBlock": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TranslatePinDataOutputTypeDef = TypedDict(
-    "TranslatePinDataOutputTypeDef",
+TranslationPinDataIsoFormat034TypeDef = TypedDict(
+    "TranslationPinDataIsoFormat034TypeDef",
     {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PinBlock": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PrimaryAccountNumber": str,
     },
 )
 
 VerifyAuthRequestCryptogramOutputTypeDef = TypedDict(
     "VerifyAuthRequestCryptogramOutputTypeDef",
     {
         "AuthResponseValue": str,
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyCardValidationDataOutputTypeDef = TypedDict(
     "VerifyCardValidationDataOutputTypeDef",
     {
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyMacOutputTypeDef = TypedDict(
     "VerifyMacOutputTypeDef",
     {
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyPinDataOutputTypeDef = TypedDict(
     "VerifyPinDataOutputTypeDef",
     {
         "EncryptionKeyArn": str,
         "EncryptionKeyCheckValue": str,
         "VerificationKeyArn": str,
         "VerificationKeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CardGenerationAttributesTypeDef = TypedDict(
+    "CardGenerationAttributesTypeDef",
+    {
+        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
+        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
+        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
+        "CardVerificationValue1": CardVerificationValue1TypeDef,
+        "CardVerificationValue2": CardVerificationValue2TypeDef,
+        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
+        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
+    },
+    total=False,
+)
+
+CardVerificationAttributesTypeDef = TypedDict(
+    "CardVerificationAttributesTypeDef",
+    {
+        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
+        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
+        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
+        "CardVerificationValue1": CardVerificationValue1TypeDef,
+        "CardVerificationValue2": CardVerificationValue2TypeDef,
+        "DiscoverDynamicCardVerificationCode": DiscoverDynamicCardVerificationCodeTypeDef,
+        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
+        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
     },
+    total=False,
+)
+
+CryptogramAuthResponseTypeDef = TypedDict(
+    "CryptogramAuthResponseTypeDef",
+    {
+        "ArpcMethod1": CryptogramVerificationArpcMethod1TypeDef,
+        "ArpcMethod2": CryptogramVerificationArpcMethod2TypeDef,
+    },
+    total=False,
 )
 
 EncryptionDecryptionAttributesTypeDef = TypedDict(
     "EncryptionDecryptionAttributesTypeDef",
     {
         "Asymmetric": AsymmetricEncryptionAttributesTypeDef,
         "Dukpt": DukptEncryptionAttributesTypeDef,
@@ -616,15 +605,15 @@
     {
         "EncryptedPinBlock": str,
         "EncryptionKeyArn": str,
         "EncryptionKeyCheckValue": str,
         "GenerationKeyArn": str,
         "GenerationKeyCheckValue": str,
         "PinData": PinDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MacAlgorithmEmvTypeDef = TypedDict(
     "MacAlgorithmEmvTypeDef",
     {
         "MajorKeyDerivationMode": MajorKeyDerivationModeType,
@@ -692,22 +681,20 @@
     "_OptionalGenerateCardValidationDataInputRequestTypeDef",
     {
         "ValidationDataLength": int,
     },
     total=False,
 )
 
-
 class GenerateCardValidationDataInputRequestTypeDef(
     _RequiredGenerateCardValidationDataInputRequestTypeDef,
     _OptionalGenerateCardValidationDataInputRequestTypeDef,
 ):
     pass
 
-
 VerifyCardValidationDataInputRequestTypeDef = TypedDict(
     "VerifyCardValidationDataInputRequestTypeDef",
     {
         "KeyIdentifier": str,
         "PrimaryAccountNumber": str,
         "ValidationData": str,
         "VerificationAttributes": CardVerificationAttributesTypeDef,
@@ -769,21 +756,19 @@
     "_OptionalGeneratePinDataInputRequestTypeDef",
     {
         "PinDataLength": int,
     },
     total=False,
 )
 
-
 class GeneratePinDataInputRequestTypeDef(
     _RequiredGeneratePinDataInputRequestTypeDef, _OptionalGeneratePinDataInputRequestTypeDef
 ):
     pass
 
-
 _RequiredVerifyPinDataInputRequestTypeDef = TypedDict(
     "_RequiredVerifyPinDataInputRequestTypeDef",
     {
         "EncryptedPinBlock": str,
         "EncryptionKeyIdentifier": str,
         "PinBlockFormat": PinBlockFormatForPinDataType,
         "PrimaryAccountNumber": str,
@@ -796,21 +781,19 @@
     {
         "DukptAttributes": DukptAttributesTypeDef,
         "PinDataLength": int,
     },
     total=False,
 )
 
-
 class VerifyPinDataInputRequestTypeDef(
     _RequiredVerifyPinDataInputRequestTypeDef, _OptionalVerifyPinDataInputRequestTypeDef
 ):
     pass
 
-
 _RequiredVerifyAuthRequestCryptogramInputRequestTypeDef = TypedDict(
     "_RequiredVerifyAuthRequestCryptogramInputRequestTypeDef",
     {
         "AuthRequestCryptogram": str,
         "KeyIdentifier": str,
         "MajorKeyDerivationMode": MajorKeyDerivationModeType,
         "SessionKeyDerivationAttributes": SessionKeyDerivationTypeDef,
@@ -821,22 +804,20 @@
     "_OptionalVerifyAuthRequestCryptogramInputRequestTypeDef",
     {
         "AuthResponseAttributes": CryptogramAuthResponseTypeDef,
     },
     total=False,
 )
 
-
 class VerifyAuthRequestCryptogramInputRequestTypeDef(
     _RequiredVerifyAuthRequestCryptogramInputRequestTypeDef,
     _OptionalVerifyAuthRequestCryptogramInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredTranslatePinDataInputRequestTypeDef = TypedDict(
     "_RequiredTranslatePinDataInputRequestTypeDef",
     {
         "EncryptedPinBlock": str,
         "IncomingKeyIdentifier": str,
         "IncomingTranslationAttributes": TranslationIsoFormatsTypeDef,
         "OutgoingKeyIdentifier": str,
@@ -848,21 +829,19 @@
     {
         "IncomingDukptAttributes": DukptDerivationAttributesTypeDef,
         "OutgoingDukptAttributes": DukptDerivationAttributesTypeDef,
     },
     total=False,
 )
 
-
 class TranslatePinDataInputRequestTypeDef(
     _RequiredTranslatePinDataInputRequestTypeDef, _OptionalTranslatePinDataInputRequestTypeDef
 ):
     pass
 
-
 _RequiredGenerateMacInputRequestTypeDef = TypedDict(
     "_RequiredGenerateMacInputRequestTypeDef",
     {
         "GenerationAttributes": MacAttributesTypeDef,
         "KeyIdentifier": str,
         "MessageData": str,
     },
@@ -871,21 +850,19 @@
     "_OptionalGenerateMacInputRequestTypeDef",
     {
         "MacLength": int,
     },
     total=False,
 )
 
-
 class GenerateMacInputRequestTypeDef(
     _RequiredGenerateMacInputRequestTypeDef, _OptionalGenerateMacInputRequestTypeDef
 ):
     pass
 
-
 _RequiredVerifyMacInputRequestTypeDef = TypedDict(
     "_RequiredVerifyMacInputRequestTypeDef",
     {
         "KeyIdentifier": str,
         "Mac": str,
         "MessageData": str,
         "VerificationAttributes": MacAttributesTypeDef,
@@ -895,12 +872,11 @@
     "_OptionalVerifyMacInputRequestTypeDef",
     {
         "MacLength": int,
     },
     total=False,
 )
 
-
 class VerifyMacInputRequestTypeDef(
     _RequiredVerifyMacInputRequestTypeDef, _OptionalVerifyMacInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data/type_defs.pyi` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,61 +27,62 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AmexCardSecurityCodeVersion1TypeDef",
     "AmexCardSecurityCodeVersion2TypeDef",
     "AsymmetricEncryptionAttributesTypeDef",
     "CardHolderVerificationValueTypeDef",
     "CardVerificationValue1TypeDef",
     "CardVerificationValue2TypeDef",
     "DynamicCardVerificationCodeTypeDef",
     "DynamicCardVerificationValueTypeDef",
     "DiscoverDynamicCardVerificationCodeTypeDef",
     "CryptogramVerificationArpcMethod1TypeDef",
     "CryptogramVerificationArpcMethod2TypeDef",
-    "ResponseMetadataTypeDef",
+    "DecryptDataOutputTypeDef",
     "DukptAttributesTypeDef",
     "DukptDerivationAttributesTypeDef",
     "DukptEncryptionAttributesTypeDef",
+    "EncryptDataOutputTypeDef",
     "SymmetricEncryptionAttributesTypeDef",
+    "GenerateCardValidationDataOutputTypeDef",
+    "GenerateMacOutputTypeDef",
     "PinDataTypeDef",
     "Ibm3624NaturalPinTypeDef",
     "Ibm3624PinFromOffsetTypeDef",
     "Ibm3624PinOffsetTypeDef",
     "Ibm3624PinVerificationTypeDef",
     "Ibm3624RandomPinTypeDef",
     "MacAlgorithmDukptTypeDef",
     "SessionKeyDerivationValueTypeDef",
     "VisaPinTypeDef",
     "VisaPinVerificationValueTypeDef",
     "VisaPinVerificationTypeDef",
+    "ReEncryptDataOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SessionKeyAmexTypeDef",
     "SessionKeyEmv2000TypeDef",
     "SessionKeyEmvCommonTypeDef",
     "SessionKeyMastercardTypeDef",
     "SessionKeyVisaTypeDef",
-    "TranslationPinDataIsoFormat034TypeDef",
-    "CardGenerationAttributesTypeDef",
-    "CardVerificationAttributesTypeDef",
-    "CryptogramAuthResponseTypeDef",
-    "DecryptDataOutputTypeDef",
-    "EncryptDataOutputTypeDef",
-    "GenerateCardValidationDataOutputTypeDef",
-    "GenerateMacOutputTypeDef",
-    "ReEncryptDataOutputTypeDef",
     "TranslatePinDataOutputTypeDef",
+    "TranslationPinDataIsoFormat034TypeDef",
     "VerifyAuthRequestCryptogramOutputTypeDef",
     "VerifyCardValidationDataOutputTypeDef",
     "VerifyMacOutputTypeDef",
     "VerifyPinDataOutputTypeDef",
+    "CardGenerationAttributesTypeDef",
+    "CardVerificationAttributesTypeDef",
+    "CryptogramAuthResponseTypeDef",
     "EncryptionDecryptionAttributesTypeDef",
     "ReEncryptionAttributesTypeDef",
     "GeneratePinDataOutputTypeDef",
     "MacAlgorithmEmvTypeDef",
     "PinGenerationAttributesTypeDef",
     "PinVerificationAttributesTypeDef",
     "SessionKeyDerivationTypeDef",
@@ -193,28 +194,29 @@
     "_OptionalCryptogramVerificationArpcMethod2TypeDef",
     {
         "ProprietaryAuthenticationData": str,
     },
     total=False,
 )
 
+
 class CryptogramVerificationArpcMethod2TypeDef(
     _RequiredCryptogramVerificationArpcMethod2TypeDef,
     _OptionalCryptogramVerificationArpcMethod2TypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+DecryptDataOutputTypeDef = TypedDict(
+    "DecryptDataOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "PlainText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DukptAttributesTypeDef = TypedDict(
     "DukptAttributesTypeDef",
     {
         "DukptDerivationType": DukptDerivationTypeType,
@@ -233,19 +235,21 @@
     {
         "DukptKeyDerivationType": DukptDerivationTypeType,
         "DukptKeyVariant": DukptKeyVariantType,
     },
     total=False,
 )
 
+
 class DukptDerivationAttributesTypeDef(
     _RequiredDukptDerivationAttributesTypeDef, _OptionalDukptDerivationAttributesTypeDef
 ):
     pass
 
+
 _RequiredDukptEncryptionAttributesTypeDef = TypedDict(
     "_RequiredDukptEncryptionAttributesTypeDef",
     {
         "KeySerialNumber": str,
     },
 )
 _OptionalDukptEncryptionAttributesTypeDef = TypedDict(
@@ -255,19 +259,31 @@
         "DukptKeyVariant": DukptKeyVariantType,
         "InitializationVector": str,
         "Mode": DukptEncryptionModeType,
     },
     total=False,
 )
 
+
 class DukptEncryptionAttributesTypeDef(
     _RequiredDukptEncryptionAttributesTypeDef, _OptionalDukptEncryptionAttributesTypeDef
 ):
     pass
 
+
+EncryptDataOutputTypeDef = TypedDict(
+    "EncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSymmetricEncryptionAttributesTypeDef = TypedDict(
     "_RequiredSymmetricEncryptionAttributesTypeDef",
     {
         "Mode": EncryptionModeType,
     },
 )
 _OptionalSymmetricEncryptionAttributesTypeDef = TypedDict(
@@ -275,19 +291,41 @@
     {
         "InitializationVector": str,
         "PaddingType": PaddingTypeType,
     },
     total=False,
 )
 
+
 class SymmetricEncryptionAttributesTypeDef(
     _RequiredSymmetricEncryptionAttributesTypeDef, _OptionalSymmetricEncryptionAttributesTypeDef
 ):
     pass
 
+
+GenerateCardValidationDataOutputTypeDef = TypedDict(
+    "GenerateCardValidationDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ValidationData": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GenerateMacOutputTypeDef = TypedDict(
+    "GenerateMacOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "Mac": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PinDataTypeDef = TypedDict(
     "PinDataTypeDef",
     {
         "PinOffset": str,
         "VerificationValue": str,
     },
     total=False,
@@ -352,19 +390,21 @@
     "_OptionalMacAlgorithmDukptTypeDef",
     {
         "DukptDerivationType": DukptDerivationTypeType,
     },
     total=False,
 )
 
+
 class MacAlgorithmDukptTypeDef(
     _RequiredMacAlgorithmDukptTypeDef, _OptionalMacAlgorithmDukptTypeDef
 ):
     pass
 
+
 SessionKeyDerivationValueTypeDef = TypedDict(
     "SessionKeyDerivationValueTypeDef",
     {
         "ApplicationCryptogram": str,
         "ApplicationTransactionCounter": str,
     },
     total=False,
@@ -389,14 +429,35 @@
     "VisaPinVerificationTypeDef",
     {
         "PinVerificationKeyIndex": int,
         "VerificationValue": str,
     },
 )
 
+ReEncryptDataOutputTypeDef = TypedDict(
+    "ReEncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
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
 SessionKeyAmexTypeDef = TypedDict(
     "SessionKeyAmexTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
@@ -433,156 +494,106 @@
     "SessionKeyVisaTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
 
-TranslationPinDataIsoFormat034TypeDef = TypedDict(
-    "TranslationPinDataIsoFormat034TypeDef",
-    {
-        "PrimaryAccountNumber": str,
-    },
-)
-
-CardGenerationAttributesTypeDef = TypedDict(
-    "CardGenerationAttributesTypeDef",
-    {
-        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
-        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
-        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
-        "CardVerificationValue1": CardVerificationValue1TypeDef,
-        "CardVerificationValue2": CardVerificationValue2TypeDef,
-        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
-        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
-    },
-    total=False,
-)
-
-CardVerificationAttributesTypeDef = TypedDict(
-    "CardVerificationAttributesTypeDef",
-    {
-        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
-        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
-        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
-        "CardVerificationValue1": CardVerificationValue1TypeDef,
-        "CardVerificationValue2": CardVerificationValue2TypeDef,
-        "DiscoverDynamicCardVerificationCode": DiscoverDynamicCardVerificationCodeTypeDef,
-        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
-        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
-    },
-    total=False,
-)
-
-CryptogramAuthResponseTypeDef = TypedDict(
-    "CryptogramAuthResponseTypeDef",
-    {
-        "ArpcMethod1": CryptogramVerificationArpcMethod1TypeDef,
-        "ArpcMethod2": CryptogramVerificationArpcMethod2TypeDef,
-    },
-    total=False,
-)
-
-DecryptDataOutputTypeDef = TypedDict(
-    "DecryptDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PlainText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EncryptDataOutputTypeDef = TypedDict(
-    "EncryptDataOutputTypeDef",
-    {
-        "CipherText": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GenerateCardValidationDataOutputTypeDef = TypedDict(
-    "GenerateCardValidationDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ValidationData": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GenerateMacOutputTypeDef = TypedDict(
-    "GenerateMacOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "Mac": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReEncryptDataOutputTypeDef = TypedDict(
-    "ReEncryptDataOutputTypeDef",
+TranslatePinDataOutputTypeDef = TypedDict(
+    "TranslatePinDataOutputTypeDef",
     {
-        "CipherText": str,
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PinBlock": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TranslatePinDataOutputTypeDef = TypedDict(
-    "TranslatePinDataOutputTypeDef",
+TranslationPinDataIsoFormat034TypeDef = TypedDict(
+    "TranslationPinDataIsoFormat034TypeDef",
     {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PinBlock": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PrimaryAccountNumber": str,
     },
 )
 
 VerifyAuthRequestCryptogramOutputTypeDef = TypedDict(
     "VerifyAuthRequestCryptogramOutputTypeDef",
     {
         "AuthResponseValue": str,
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyCardValidationDataOutputTypeDef = TypedDict(
     "VerifyCardValidationDataOutputTypeDef",
     {
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyMacOutputTypeDef = TypedDict(
     "VerifyMacOutputTypeDef",
     {
         "KeyArn": str,
         "KeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VerifyPinDataOutputTypeDef = TypedDict(
     "VerifyPinDataOutputTypeDef",
     {
         "EncryptionKeyArn": str,
         "EncryptionKeyCheckValue": str,
         "VerificationKeyArn": str,
         "VerificationKeyCheckValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CardGenerationAttributesTypeDef = TypedDict(
+    "CardGenerationAttributesTypeDef",
+    {
+        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
+        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
+        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
+        "CardVerificationValue1": CardVerificationValue1TypeDef,
+        "CardVerificationValue2": CardVerificationValue2TypeDef,
+        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
+        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
     },
+    total=False,
+)
+
+CardVerificationAttributesTypeDef = TypedDict(
+    "CardVerificationAttributesTypeDef",
+    {
+        "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
+        "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
+        "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
+        "CardVerificationValue1": CardVerificationValue1TypeDef,
+        "CardVerificationValue2": CardVerificationValue2TypeDef,
+        "DiscoverDynamicCardVerificationCode": DiscoverDynamicCardVerificationCodeTypeDef,
+        "DynamicCardVerificationCode": DynamicCardVerificationCodeTypeDef,
+        "DynamicCardVerificationValue": DynamicCardVerificationValueTypeDef,
+    },
+    total=False,
+)
+
+CryptogramAuthResponseTypeDef = TypedDict(
+    "CryptogramAuthResponseTypeDef",
+    {
+        "ArpcMethod1": CryptogramVerificationArpcMethod1TypeDef,
+        "ArpcMethod2": CryptogramVerificationArpcMethod2TypeDef,
+    },
+    total=False,
 )
 
 EncryptionDecryptionAttributesTypeDef = TypedDict(
     "EncryptionDecryptionAttributesTypeDef",
     {
         "Asymmetric": AsymmetricEncryptionAttributesTypeDef,
         "Dukpt": DukptEncryptionAttributesTypeDef,
@@ -605,15 +616,15 @@
     {
         "EncryptedPinBlock": str,
         "EncryptionKeyArn": str,
         "EncryptionKeyCheckValue": str,
         "GenerationKeyArn": str,
         "GenerationKeyCheckValue": str,
         "PinData": PinDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MacAlgorithmEmvTypeDef = TypedDict(
     "MacAlgorithmEmvTypeDef",
     {
         "MajorKeyDerivationMode": MajorKeyDerivationModeType,
@@ -681,20 +692,22 @@
     "_OptionalGenerateCardValidationDataInputRequestTypeDef",
     {
         "ValidationDataLength": int,
     },
     total=False,
 )
 
+
 class GenerateCardValidationDataInputRequestTypeDef(
     _RequiredGenerateCardValidationDataInputRequestTypeDef,
     _OptionalGenerateCardValidationDataInputRequestTypeDef,
 ):
     pass
 
+
 VerifyCardValidationDataInputRequestTypeDef = TypedDict(
     "VerifyCardValidationDataInputRequestTypeDef",
     {
         "KeyIdentifier": str,
         "PrimaryAccountNumber": str,
         "ValidationData": str,
         "VerificationAttributes": CardVerificationAttributesTypeDef,
@@ -756,19 +769,21 @@
     "_OptionalGeneratePinDataInputRequestTypeDef",
     {
         "PinDataLength": int,
     },
     total=False,
 )
 
+
 class GeneratePinDataInputRequestTypeDef(
     _RequiredGeneratePinDataInputRequestTypeDef, _OptionalGeneratePinDataInputRequestTypeDef
 ):
     pass
 
+
 _RequiredVerifyPinDataInputRequestTypeDef = TypedDict(
     "_RequiredVerifyPinDataInputRequestTypeDef",
     {
         "EncryptedPinBlock": str,
         "EncryptionKeyIdentifier": str,
         "PinBlockFormat": PinBlockFormatForPinDataType,
         "PrimaryAccountNumber": str,
@@ -781,19 +796,21 @@
     {
         "DukptAttributes": DukptAttributesTypeDef,
         "PinDataLength": int,
     },
     total=False,
 )
 
+
 class VerifyPinDataInputRequestTypeDef(
     _RequiredVerifyPinDataInputRequestTypeDef, _OptionalVerifyPinDataInputRequestTypeDef
 ):
     pass
 
+
 _RequiredVerifyAuthRequestCryptogramInputRequestTypeDef = TypedDict(
     "_RequiredVerifyAuthRequestCryptogramInputRequestTypeDef",
     {
         "AuthRequestCryptogram": str,
         "KeyIdentifier": str,
         "MajorKeyDerivationMode": MajorKeyDerivationModeType,
         "SessionKeyDerivationAttributes": SessionKeyDerivationTypeDef,
@@ -804,20 +821,22 @@
     "_OptionalVerifyAuthRequestCryptogramInputRequestTypeDef",
     {
         "AuthResponseAttributes": CryptogramAuthResponseTypeDef,
     },
     total=False,
 )
 
+
 class VerifyAuthRequestCryptogramInputRequestTypeDef(
     _RequiredVerifyAuthRequestCryptogramInputRequestTypeDef,
     _OptionalVerifyAuthRequestCryptogramInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredTranslatePinDataInputRequestTypeDef = TypedDict(
     "_RequiredTranslatePinDataInputRequestTypeDef",
     {
         "EncryptedPinBlock": str,
         "IncomingKeyIdentifier": str,
         "IncomingTranslationAttributes": TranslationIsoFormatsTypeDef,
         "OutgoingKeyIdentifier": str,
@@ -829,19 +848,21 @@
     {
         "IncomingDukptAttributes": DukptDerivationAttributesTypeDef,
         "OutgoingDukptAttributes": DukptDerivationAttributesTypeDef,
     },
     total=False,
 )
 
+
 class TranslatePinDataInputRequestTypeDef(
     _RequiredTranslatePinDataInputRequestTypeDef, _OptionalTranslatePinDataInputRequestTypeDef
 ):
     pass
 
+
 _RequiredGenerateMacInputRequestTypeDef = TypedDict(
     "_RequiredGenerateMacInputRequestTypeDef",
     {
         "GenerationAttributes": MacAttributesTypeDef,
         "KeyIdentifier": str,
         "MessageData": str,
     },
@@ -850,19 +871,21 @@
     "_OptionalGenerateMacInputRequestTypeDef",
     {
         "MacLength": int,
     },
     total=False,
 )
 
+
 class GenerateMacInputRequestTypeDef(
     _RequiredGenerateMacInputRequestTypeDef, _OptionalGenerateMacInputRequestTypeDef
 ):
     pass
 
+
 _RequiredVerifyMacInputRequestTypeDef = TypedDict(
     "_RequiredVerifyMacInputRequestTypeDef",
     {
         "KeyIdentifier": str,
         "Mac": str,
         "MessageData": str,
         "VerificationAttributes": MacAttributesTypeDef,
@@ -872,11 +895,12 @@
     "_OptionalVerifyMacInputRequestTypeDef",
     {
         "MacLength": int,
     },
     total=False,
 )
 
+
 class VerifyMacInputRequestTypeDef(
     _RequiredVerifyMacInputRequestTypeDef, _OptionalVerifyMacInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography-data
-Version: 1.26.150
-Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography-data?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -316,49 +316,49 @@
     CardVerificationValue1TypeDef,
     CardVerificationValue2TypeDef,
     DynamicCardVerificationCodeTypeDef,
     DynamicCardVerificationValueTypeDef,
     DiscoverDynamicCardVerificationCodeTypeDef,
     CryptogramVerificationArpcMethod1TypeDef,
     CryptogramVerificationArpcMethod2TypeDef,
-    ResponseMetadataTypeDef,
+    DecryptDataOutputTypeDef,
     DukptAttributesTypeDef,
     DukptDerivationAttributesTypeDef,
     DukptEncryptionAttributesTypeDef,
+    EncryptDataOutputTypeDef,
     SymmetricEncryptionAttributesTypeDef,
+    GenerateCardValidationDataOutputTypeDef,
+    GenerateMacOutputTypeDef,
     PinDataTypeDef,
     Ibm3624NaturalPinTypeDef,
     Ibm3624PinFromOffsetTypeDef,
     Ibm3624PinOffsetTypeDef,
     Ibm3624PinVerificationTypeDef,
     Ibm3624RandomPinTypeDef,
     MacAlgorithmDukptTypeDef,
     SessionKeyDerivationValueTypeDef,
     VisaPinTypeDef,
     VisaPinVerificationValueTypeDef,
     VisaPinVerificationTypeDef,
+    ReEncryptDataOutputTypeDef,
+    ResponseMetadataTypeDef,
     SessionKeyAmexTypeDef,
     SessionKeyEmv2000TypeDef,
     SessionKeyEmvCommonTypeDef,
     SessionKeyMastercardTypeDef,
     SessionKeyVisaTypeDef,
-    TranslationPinDataIsoFormat034TypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
-    DecryptDataOutputTypeDef,
-    EncryptDataOutputTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
-    ReEncryptDataOutputTypeDef,
     TranslatePinDataOutputTypeDef,
+    TranslationPinDataIsoFormat034TypeDef,
     VerifyAuthRequestCryptogramOutputTypeDef,
     VerifyCardValidationDataOutputTypeDef,
     VerifyMacOutputTypeDef,
     VerifyPinDataOutputTypeDef,
+    CardGenerationAttributesTypeDef,
+    CardVerificationAttributesTypeDef,
+    CryptogramAuthResponseTypeDef,
     EncryptionDecryptionAttributesTypeDef,
     ReEncryptionAttributesTypeDef,
     GeneratePinDataOutputTypeDef,
     MacAlgorithmEmvTypeDef,
     PinGenerationAttributesTypeDef,
     PinVerificationAttributesTypeDef,
     SessionKeyDerivationTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-data-1.27.0/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.26.150/setup.py` & `mypy-boto3-payment-cryptography-data-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography-data",
-    version="1.26.150",
+    version="1.27.0",
     packages=["mypy_boto3_payment_cryptography_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PaymentCryptographyDataPlane 1.26.150 service generated with"
+        "Type annotations for boto3.PaymentCryptographyDataPlane 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


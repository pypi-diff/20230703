# Comparing `tmp/mypy-boto3-1.26.99.tar.gz` & `tmp/mypy-boto3-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-1.26.99.tar", last modified: Fri Mar 24 19:32:25 2023, max compression
+gzip compressed data, was "mypy-boto3-1.27.0.tar", last modified: Mon Jul  3 19:50:17 2023, max compression
```

## Comparing `mypy-boto3-1.26.99.tar` & `mypy-boto3-1.27.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.589893 mypy-boto3-1.26.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-24 19:32:25.589893 mypy-boto3-1.26.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.589893 mypy-boto3-1.26.99/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 19:31:51.000000 mypy-boto3-1.26.99/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 19:31:51.000000 mypy-boto3-1.26.99/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 19:31:51.000000 mypy-boto3-1.26.99/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-24 19:31:51.000000 mypy-boto3-1.26.99/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:51.000000 mypy-boto3-1.26.99/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   103410 2023-03-24 19:31:51.000000 mypy-boto3-1.26.99/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.589893 mypy-boto3-1.26.99/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-24 19:32:25.000000 mypy-boto3-1.26.99/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-24 19:32:25.000000 mypy-boto3-1.26.99/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-1.26.99/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-1.26.99/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-24 19:32:25.000000 mypy-boto3-1.26.99/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-24 19:32:25.000000 mypy-boto3-1.26.99/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:32:25.589893 mypy-boto3-1.26.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-24 19:31:49.000000 mypy-boto3-1.26.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.742733 mypy-boto3-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:31:43.000000 mypy-boto3-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-03 19:50:17.742733 mypy-boto3-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-03 19:31:43.000000 mypy-boto3-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.726733 mypy-boto3-1.27.0/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 19:31:43.000000 mypy-boto3-1.27.0/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-03 19:31:43.000000 mypy-boto3-1.27.0/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   105966 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:31:44.000000 mypy-boto3-1.27.0/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.742733 mypy-boto3-1.27.0/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-03 19:50:17.000000 mypy-boto3-1.27.0/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 19:50:17.000000 mypy-boto3-1.27.0/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-1.27.0/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-1.27.0/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 19:50:17.000000 mypy-boto3-1.27.0/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 19:50:17.000000 mypy-boto3-1.27.0/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:17.742733 mypy-boto3-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-03 19:31:43.000000 mypy-boto3-1.27.0/setup.py
```

### Comparing `mypy-boto3-1.26.99/LICENSE` & `mypy-boto3-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.26.99/PKG-INFO` & `mypy-boto3-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.26.99
-Summary: Type annotations for boto3 1.26.99 master module generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3 1.27.0 master module generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,26 +32,26 @@
 
 <a id="mypy-boto3"></a>
 
 # mypy-boto3
 
 [![PyPI - mypy-boto3](https://img.shields.io/pypi/v/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/1.26.99/index.html)
+[boto3 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/1.27.0/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy-boto3-1.26.99/README.md` & `mypy-boto3-1.27.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <a id="mypy-boto3"></a>
 
 # mypy-boto3
 
 [![PyPI - mypy-boto3](https://img.shields.io/pypi/v/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/1.26.99/index.html)
+[boto3 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/1.27.0/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy-boto3-1.26.99/mypy_boto3/boto3_init_stub.py` & `mypy-boto3-1.27.0/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.26.99/mypy_boto3/boto3_session_stub.py` & `mypy-boto3-1.27.0/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.26.99/mypy_boto3/main.py` & `mypy-boto3-1.27.0/mypy_boto3/main.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.26.99/mypy_boto3/submodules.py` & `mypy-boto3-1.27.0/mypy_boto3/submodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         module_name="mypy_boto3_account",
         import_name="account",
         boto3_name="account",
         class_name="Account",
         pypi_name="mypy-boto3-account",
         has_resource=False,
         has_waiter=False,
-        has_paginator=False,
+        has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_acm",
         import_name="acm",
         boto3_name="acm",
         class_name="ACM",
         pypi_name="mypy-boto3-acm",
@@ -169,14 +169,24 @@
         class_name="AppConfigData",
         pypi_name="mypy-boto3-appconfigdata",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
+        module_name="mypy_boto3_appfabric",
+        import_name="appfabric",
+        boto3_name="appfabric",
+        class_name="AppFabric",
+        pypi_name="mypy-boto3-appfabric",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
         module_name="mypy_boto3_appflow",
         import_name="appflow",
         boto3_name="appflow",
         class_name="Appflow",
         pypi_name="mypy-boto3-appflow",
         has_resource=False,
         has_waiter=False,
@@ -639,14 +649,24 @@
         class_name="CodeGuruReviewer",
         pypi_name="mypy-boto3-codeguru-reviewer",
         has_resource=False,
         has_waiter=True,
         has_paginator=True,
     ),
     Submodule(
+        module_name="mypy_boto3_codeguru_security",
+        import_name="codeguru_security",
+        boto3_name="codeguru-security",
+        class_name="CodeGuruSecurity",
+        pypi_name="mypy-boto3-codeguru-security",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
         module_name="mypy_boto3_codeguruprofiler",
         import_name="codeguruprofiler",
         boto3_name="codeguruprofiler",
         class_name="CodeGuruProfiler",
         pypi_name="mypy-boto3-codeguruprofiler",
         has_resource=False,
         has_waiter=False,
@@ -836,15 +856,15 @@
         module_name="mypy_boto3_customer_profiles",
         import_name="customer_profiles",
         boto3_name="customer-profiles",
         class_name="CustomerProfiles",
         pypi_name="mypy-boto3-customer-profiles",
         has_resource=False,
         has_waiter=False,
-        has_paginator=False,
+        has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_databrew",
         import_name="databrew",
         boto3_name="databrew",
         class_name="GlueDataBrew",
         pypi_name="mypy-boto3-databrew",
@@ -1226,15 +1246,15 @@
         module_name="mypy_boto3_finspace",
         import_name="finspace",
         boto3_name="finspace",
         class_name="finspace",
         pypi_name="mypy-boto3-finspace",
         has_resource=False,
         has_waiter=False,
-        has_paginator=False,
+        has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_finspace_data",
         import_name="finspace_data",
         boto3_name="finspace-data",
         class_name="FinSpaceData",
         pypi_name="mypy-boto3-finspace-data",
@@ -2056,15 +2076,15 @@
         module_name="mypy_boto3_marketplace_catalog",
         import_name="marketplace_catalog",
         boto3_name="marketplace-catalog",
         class_name="MarketplaceCatalog",
         pypi_name="mypy-boto3-marketplace-catalog",
         has_resource=False,
         has_waiter=False,
-        has_paginator=False,
+        has_paginator=True,
     ),
     Submodule(
         module_name="mypy_boto3_marketplace_entitlement",
         import_name="marketplace_entitlement",
         boto3_name="marketplace-entitlement",
         class_name="MarketplaceEntitlementService",
         pypi_name="mypy-boto3-marketplace-entitlement",
@@ -2129,14 +2149,24 @@
         class_name="MediaPackageVod",
         pypi_name="mypy-boto3-mediapackage-vod",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
+        module_name="mypy_boto3_mediapackagev2",
+        import_name="mediapackagev2",
+        boto3_name="mediapackagev2",
+        class_name="mediapackagev2",
+        pypi_name="mypy-boto3-mediapackagev2",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
         module_name="mypy_boto3_mediastore",
         import_name="mediastore",
         boto3_name="mediastore",
         class_name="MediaStore",
         pypi_name="mypy-boto3-mediastore",
         has_resource=False,
         has_waiter=False,
@@ -2389,14 +2419,24 @@
         class_name="Organizations",
         pypi_name="mypy-boto3-organizations",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
+        module_name="mypy_boto3_osis",
+        import_name="osis",
+        boto3_name="osis",
+        class_name="OpenSearchIngestion",
+        pypi_name="mypy-boto3-osis",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=False,
+    ),
+    Submodule(
         module_name="mypy_boto3_outposts",
         import_name="outposts",
         boto3_name="outposts",
         class_name="Outposts",
         pypi_name="mypy-boto3-outposts",
         has_resource=False,
         has_waiter=False,
@@ -2409,14 +2449,34 @@
         class_name="Panorama",
         pypi_name="mypy-boto3-panorama",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
+        module_name="mypy_boto3_payment_cryptography",
+        import_name="payment_cryptography",
+        boto3_name="payment-cryptography",
+        class_name="PaymentCryptographyControlPlane",
+        pypi_name="mypy-boto3-payment-cryptography",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
+        module_name="mypy_boto3_payment_cryptography_data",
+        import_name="payment_cryptography_data",
+        boto3_name="payment-cryptography-data",
+        class_name="PaymentCryptographyDataPlane",
+        pypi_name="mypy-boto3-payment-cryptography-data",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=False,
+    ),
+    Submodule(
         module_name="mypy_boto3_personalize",
         import_name="personalize",
         boto3_name="personalize",
         class_name="Personalize",
         pypi_name="mypy-boto3-personalize",
         has_resource=False,
         has_waiter=False,
@@ -3319,24 +3379,44 @@
         class_name="Translate",
         pypi_name="mypy-boto3-translate",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
+        module_name="mypy_boto3_verifiedpermissions",
+        import_name="verifiedpermissions",
+        boto3_name="verifiedpermissions",
+        class_name="VerifiedPermissions",
+        pypi_name="mypy-boto3-verifiedpermissions",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
         module_name="mypy_boto3_voice_id",
         import_name="voice_id",
         boto3_name="voice-id",
         class_name="VoiceID",
         pypi_name="mypy-boto3-voice-id",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
+        module_name="mypy_boto3_vpc_lattice",
+        import_name="vpc_lattice",
+        boto3_name="vpc-lattice",
+        class_name="VPCLattice",
+        pypi_name="mypy-boto3-vpc-lattice",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
         module_name="mypy_boto3_waf",
         import_name="waf",
         boto3_name="waf",
         class_name="WAF",
         pypi_name="mypy-boto3-waf",
         has_resource=False,
         has_waiter=False,
```

### Comparing `mypy-boto3-1.26.99/mypy_boto3.egg-info/PKG-INFO` & `mypy-boto3-1.27.0/mypy_boto3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.26.99
-Summary: Type annotations for boto3 1.26.99 master module generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3 1.27.0 master module generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,26 +32,26 @@
 
 <a id="mypy-boto3"></a>
 
 # mypy-boto3
 
 [![PyPI - mypy-boto3](https://img.shields.io/pypi/v/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3?color=blue)](https://pypistats.org/packages/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/1.26.99/index.html)
+[boto3 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/1.27.0/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy-boto3-1.26.99/setup.py` & `mypy-boto3-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.26.99",
+    version="1.27.0",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3 1.26.99 master module generated with mypy-boto3-builder 7.14.2"
+        "Type annotations for boto3 1.27.0 master module generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


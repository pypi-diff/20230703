# Comparing `tmp/mypy-boto3-codeguru-security-1.26.153.tar.gz` & `tmp/mypy-boto3-codeguru-security-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-security-1.26.153.tar", last modified: Tue Jun 13 19:33:35 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-security-1.27.0.tar", last modified: Mon Jul  3 19:50:32 2023, max compression
```

## Comparing `mypy-boto3-codeguru-security-1.26.153.tar` & `mypy-boto3-codeguru-security-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:35.520413 mypy-boto3-codeguru-security-1.26.153/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-06-13 19:33:35.520413 mypy-boto3-codeguru-security-1.26.153/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:35.508413 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-06-13 19:31:56.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:35.508413 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-06-13 19:33:35.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-13 19:33:35.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:33:35.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:33:35.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 19:33:35.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 19:33:35.000000 mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:33:35.520413 mypy-boto3-codeguru-security-1.26.153/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-13 19:31:55.000000 mypy-boto3-codeguru-security-1.26.153/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.570999 mypy-boto3-codeguru-security-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-07-03 19:50:32.570999 mypy-boto3-codeguru-security-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.562999 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-03 19:34:23.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-07-03 19:34:23.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-03 19:34:23.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.570999 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-07-03 19:50:32.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:50:32.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:32.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:32.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:32.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:32.000000 mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:32.570999 mypy-boto3-codeguru-security-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-security-1.27.0/setup.py
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/LICENSE` & `mypy-boto3-codeguru-security-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.26.153/PKG-INFO` & `mypy-boto3-codeguru-security-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.26.153
-Summary: Type annotations for boto3.CodeGuruSecurity 1.26.153 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeGuruSecurity 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.26.153](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -338,48 +338,48 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
-    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    PaginatorConfigTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
+    GetScanResponseTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
-    GetScanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/README.md` & `mypy-boto3-codeguru-security-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.26.153](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -306,48 +306,48 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
-    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    PaginatorConfigTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
+    GetScanResponseTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
-    GetScanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/__init__.py` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/__init__.pyi` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/__main__.py` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruSecurity 1.26.153\nVersion:         1.26.153\nBuilder"
+        "Type annotations for boto3.CodeGuruSecurity 1.27.0\nVersion:         1.27.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.153")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/client.py` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/client.pyi` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/literals.py` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/literals.pyi` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/paginator.py` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#getfindingspaginator)
         """
 
 
@@ -75,28 +75,28 @@
     """
 
     def paginate(
         self,
         *,
         endDate: Union[datetime, str],
         startDate: Union[datetime, str],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 
 class ListScansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/paginator.pyi` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#getfindingspaginator)
         """
 
 class ListFindingsMetricsPaginator(Paginator):
@@ -71,27 +71,27 @@
     """
 
     def paginate(
         self,
         *,
         endDate: Union[datetime, str],
         startDate: Union[datetime, str],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 class ListScansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/type_defs.py` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,48 +30,48 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
-    "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
+    "CreateUploadUrlResponseTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
+    "GetScanResponseTypeDef",
+    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     "ListFindingsMetricsRequestRequestTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ScanNameWithFindingNumTypeDef",
+    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountFindingsMetricTypeDef",
     "BatchGetFindingsRequestRequestTypeDef",
-    "CreateUploadUrlResponseTypeDef",
-    "GetScanResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
-    "GetFindingsRequestGetFindingsPaginateTypeDef",
-    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -105,25 +105,14 @@
     "FindingIdentifierTypeDef",
     {
         "findingId": str,
         "scanName": str,
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
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
     total=False,
@@ -149,14 +138,24 @@
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "codeArtifactId": str,
+        "requestHeaders": Dict[str, str],
+        "s3Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
@@ -166,24 +165,37 @@
     {
         "id": str,
         "subResourceId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "scanName": str,
+    },
+)
+_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetFindingsRequestGetFindingsPaginateTypeDef(
+    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
+    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -227,14 +239,52 @@
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
 
+GetScanResponseTypeDef = TypedDict(
+    "GetScanResponseTypeDef",
+    {
+        "analysisType": AnalysisTypeType,
+        "createdAt": datetime,
+        "numberOfRevisions": int,
+        "runId": str,
+        "scanName": str,
+        "scanNameArn": str,
+        "scanState": ScanStateType,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
+    },
+)
+_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
+    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestRequestTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -251,14 +301,22 @@
 class ListFindingsMetricsRequestRequestTypeDef(
     _RequiredListFindingsMetricsRequestRequestTypeDef,
     _OptionalListFindingsMetricsRequestRequestTypeDef,
 ):
     pass
 
 
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -290,23 +348,41 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
     total=False,
@@ -317,14 +393,25 @@
     {
         "code": str,
         "description": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -352,47 +439,14 @@
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "codeArtifactId": str,
-        "requestHeaders": Dict[str, str],
-        "s3Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetScanResponseTypeDef = TypedDict(
-    "GetScanResponseTypeDef",
-    {
-        "analysisType": AnalysisTypeType,
-        "createdAt": datetime,
-        "numberOfRevisions": int,
-        "runId": str,
-        "scanName": str,
-        "scanNameArn": str,
-        "scanState": ScanStateType,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 FilePathTypeDef = TypedDict(
     "FilePathTypeDef",
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
@@ -430,101 +484,47 @@
     "CreateScanResponseTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
     },
 )
 
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "scanName": str,
-    },
-)
-_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "status": StatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetFindingsRequestGetFindingsPaginateTypeDef(
-    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
-    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
-    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-):
-    pass
-
-
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricsSummaryTypeDef = TypedDict(
     "MetricsSummaryTypeDef",
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
@@ -546,15 +546,15 @@
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "filePath": FilePathTypeDef,
@@ -566,15 +566,15 @@
     total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "createdAt": datetime,
@@ -598,19 +598,19 @@
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security/type_defs.pyi` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -29,48 +29,48 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
-    "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
+    "CreateUploadUrlResponseTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
+    "GetScanResponseTypeDef",
+    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     "ListFindingsMetricsRequestRequestTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ScanNameWithFindingNumTypeDef",
+    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountFindingsMetricTypeDef",
     "BatchGetFindingsRequestRequestTypeDef",
-    "CreateUploadUrlResponseTypeDef",
-    "GetScanResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
-    "GetFindingsRequestGetFindingsPaginateTypeDef",
-    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -104,25 +104,14 @@
     "FindingIdentifierTypeDef",
     {
         "findingId": str,
         "scanName": str,
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
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
     total=False,
@@ -148,14 +137,24 @@
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "codeArtifactId": str,
+        "requestHeaders": Dict[str, str],
+        "s3Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
@@ -165,24 +164,35 @@
     {
         "id": str,
         "subResourceId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "scanName": str,
+    },
+)
+_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetFindingsRequestGetFindingsPaginateTypeDef(
+    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
+    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -222,14 +232,50 @@
 )
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
+GetScanResponseTypeDef = TypedDict(
+    "GetScanResponseTypeDef",
+    {
+        "analysisType": AnalysisTypeType,
+        "createdAt": datetime,
+        "numberOfRevisions": int,
+        "runId": str,
+        "scanName": str,
+        "scanNameArn": str,
+        "scanState": ScanStateType,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
+    },
+)
+_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
+    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+):
+    pass
+
 _RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestRequestTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -244,14 +290,22 @@
 
 class ListFindingsMetricsRequestRequestTypeDef(
     _RequiredListFindingsMetricsRequestRequestTypeDef,
     _OptionalListFindingsMetricsRequestRequestTypeDef,
 ):
     pass
 
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -281,23 +335,41 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
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
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
     total=False,
@@ -308,14 +380,25 @@
     {
         "code": str,
         "description": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -343,47 +426,14 @@
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "codeArtifactId": str,
-        "requestHeaders": Dict[str, str],
-        "s3Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetScanResponseTypeDef = TypedDict(
-    "GetScanResponseTypeDef",
-    {
-        "analysisType": AnalysisTypeType,
-        "createdAt": datetime,
-        "numberOfRevisions": int,
-        "runId": str,
-        "scanName": str,
-        "scanNameArn": str,
-        "scanState": ScanStateType,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 FilePathTypeDef = TypedDict(
     "FilePathTypeDef",
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
@@ -419,97 +469,47 @@
     "CreateScanResponseTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
     },
 )
 
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "scanName": str,
-    },
-)
-_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "status": StatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetFindingsRequestGetFindingsPaginateTypeDef(
-    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
-    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
-    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-):
-    pass
-
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricsSummaryTypeDef = TypedDict(
     "MetricsSummaryTypeDef",
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
@@ -531,15 +531,15 @@
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "filePath": FilePathTypeDef,
@@ -551,15 +551,15 @@
     total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "createdAt": datetime,
@@ -583,19 +583,19 @@
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/PKG-INFO` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.26.153
-Summary: Type annotations for boto3.CodeGuruSecurity 1.26.153 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeGuruSecurity 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.26.153](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -338,48 +338,48 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
-    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    PaginatorConfigTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
+    GetScanResponseTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
+    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
-    GetScanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.26.153/mypy_boto3_codeguru_security.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-security-1.27.0/mypy_boto3_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.26.153/setup.py` & `mypy-boto3-codeguru-security-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-security",
-    version="1.26.153",
+    version="1.27.0",
     packages=["mypy_boto3_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruSecurity 1.26.153 service generated with"
+        "Type annotations for boto3.CodeGuruSecurity 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


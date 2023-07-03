# Comparing `tmp/mypy-boto3-finspace-1.26.147.tar.gz` & `tmp/mypy-boto3-finspace-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.26.147.tar", last modified: Mon Jun  5 19:33:55 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.27.0.tar", last modified: Mon Jul  3 19:50:46 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.26.147.tar` & `mypy-boto3-finspace-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:55.844227 mypy-boto3-finspace-1.26.147/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-06-05 19:33:55.840227 mypy-boto3-finspace-1.26.147/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:55.832227 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34873 2023-06-05 19:33:23.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34835 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:55.840227 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:33:55.844227 mypy-boto3-finspace-1.26.147/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-03 19:37:44.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/setup.py
```

### Comparing `mypy-boto3-finspace-1.26.147/LICENSE` & `mypy-boto3-finspace-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.26.147/PKG-INFO` & `mypy-boto3-finspace-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.26.147
-Summary: Type annotations for boto3.finspace 1.26.147 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.finspace 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.26.147](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,85 +339,85 @@
 from mypy_boto3_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
+    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
+    CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
+    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
+    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
     TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
+    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
     EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    CreateKxDatabaseResponseTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
-    CreateKxUserResponseTypeDef,
-    GetKxConnectionStringResponseTypeDef,
-    GetKxDatabaseResponseTypeDef,
-    GetKxUserResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
```

### Comparing `mypy-boto3-finspace-1.26.147/README.md` & `mypy-boto3-finspace-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.26.147](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -307,85 +307,85 @@
 from mypy_boto3_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
+    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
+    CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
+    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
+    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
     TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
+    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
     EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    CreateKxDatabaseResponseTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
-    CreateKxUserResponseTypeDef,
-    GetKxConnectionStringResponseTypeDef,
-    GetKxDatabaseResponseTypeDef,
-    GetKxUserResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__init__.py` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__init__.pyi` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.26.147\nVersion:         1.26.147\nBuilder version:"
+        "Type annotations for boto3.finspace 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.147")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/client.py` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/client.pyi` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -330,14 +332,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
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
@@ -421,14 +425,15 @@
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

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.pyi` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
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
@@ -149,14 +150,15 @@
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
@@ -328,14 +330,16 @@
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "osis",
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
@@ -419,14 +423,15 @@
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

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/paginator.py` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListKxEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKxEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/paginator.pyi` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListKxEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKxEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/type_defs.py` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,93 +33,92 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AutoScalingConfigurationTypeDef",
     "CapacityConfigurationTypeDef",
     "ChangeRequestTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
+    "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
+    "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
+    "CreateKxUserResponseTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
+    "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
+    "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
     "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
+    "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
     "ListKxClustersRequestRequestTypeDef",
     "ListKxDatabasesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
+    "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
+    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
     "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "CreateKxDatabaseResponseTypeDef",
-    "CreateKxEnvironmentResponseTypeDef",
-    "CreateKxUserResponseTypeDef",
-    "GetKxConnectionStringResponseTypeDef",
-    "GetKxDatabaseResponseTypeDef",
-    "GetKxUserResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateKxDatabaseResponseTypeDef",
-    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
     "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
@@ -159,19 +158,17 @@
     "_OptionalChangeRequestTypeDef",
     {
         "s3Path": str,
     },
     total=False,
 )
 
-
 class ChangeRequestTypeDef(_RequiredChangeRequestTypeDef, _OptionalChangeRequestTypeDef):
     pass
 
-
 CodeConfigurationTypeDef = TypedDict(
     "CodeConfigurationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "s3ObjectVersion": str,
     },
@@ -196,22 +193,21 @@
     {
         "emailAddress": str,
         "firstName": str,
         "lastName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "environmentId": str,
+        "environmentArn": str,
+        "environmentUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "errorMessage": str,
@@ -269,20 +265,31 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateKxDatabaseRequestRequestTypeDef(
     _RequiredCreateKxDatabaseRequestRequestTypeDef, _OptionalCreateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
+CreateKxDatabaseResponseTypeDef = TypedDict(
+    "CreateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxEnvironmentRequestRequestTypeDef",
     {
         "name": str,
         "kmsKeyId": str,
     },
@@ -293,21 +300,33 @@
         "description": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateKxEnvironmentRequestRequestTypeDef(
     _RequiredCreateKxEnvironmentRequestRequestTypeDef,
     _OptionalCreateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
+CreateKxEnvironmentResponseTypeDef = TypedDict(
+    "CreateKxEnvironmentResponseTypeDef",
+    {
+        "name": str,
+        "status": EnvironmentStatusType,
+        "environmentId": str,
+        "description": str,
+        "environmentArn": str,
+        "kmsKeyId": str,
+        "creationTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
@@ -318,20 +337,29 @@
     {
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateKxUserRequestRequestTypeDef(
     _RequiredCreateKxUserRequestRequestTypeDef, _OptionalCreateKxUserRequestRequestTypeDef
 ):
     pass
 
+CreateKxUserResponseTypeDef = TypedDict(
+    "CreateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
@@ -355,21 +383,19 @@
     "_OptionalDeleteKxClusterRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteKxClusterRequestRequestTypeDef(
     _RequiredDeleteKxClusterRequestRequestTypeDef, _OptionalDeleteKxClusterRequestRequestTypeDef
 ):
     pass
 
-
 DeleteKxDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -419,22 +445,47 @@
     {
         "userArn": str,
         "environmentId": str,
         "clusterName": str,
     },
 )
 
+GetKxConnectionStringResponseTypeDef = TypedDict(
+    "GetKxConnectionStringResponseTypeDef",
+    {
+        "signedConnectionString": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetKxDatabaseRequestRequestTypeDef = TypedDict(
     "GetKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
     },
 )
 
+GetKxDatabaseResponseTypeDef = TypedDict(
+    "GetKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "lastCompletedChangesetId": str,
+        "numBytes": int,
+        "numChangesets": int,
+        "numFiles": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -450,14 +501,25 @@
     "GetKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
+GetKxUserResponseTypeDef = TypedDict(
+    "GetKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KxChangesetListEntryTypeDef = TypedDict(
     "KxChangesetListEntryTypeDef",
     {
         "changesetId": str,
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
@@ -546,21 +608,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListKxChangesetsRequestRequestTypeDef(
     _RequiredListKxChangesetsRequestRequestTypeDef, _OptionalListKxChangesetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListKxClusterNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListKxClusterNodesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
     },
 )
@@ -569,22 +629,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListKxClusterNodesRequestRequestTypeDef(
     _RequiredListKxClusterNodesRequestRequestTypeDef,
     _OptionalListKxClusterNodesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListKxClustersRequestRequestTypeDef = TypedDict(
     "_RequiredListKxClustersRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalListKxClustersRequestRequestTypeDef = TypedDict(
@@ -593,21 +651,19 @@
         "clusterType": KxClusterTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListKxClustersRequestRequestTypeDef(
     _RequiredListKxClustersRequestRequestTypeDef, _OptionalListKxClustersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListKxDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListKxDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalListKxDatabasesRequestRequestTypeDef = TypedDict(
@@ -615,27 +671,23 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListKxDatabasesRequestRequestTypeDef(
     _RequiredListKxDatabasesRequestRequestTypeDef, _OptionalListKxDatabasesRequestRequestTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListKxEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListKxEnvironmentsRequestRequestTypeDef",
     {
@@ -656,28 +708,55 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListKxUsersRequestRequestTypeDef(
     _RequiredListKxUsersRequestRequestTypeDef, _OptionalListKxUsersRequestRequestTypeDef
 ):
     pass
 
-
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -702,20 +781,29 @@
     "_OptionalUpdateKxDatabaseRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateKxDatabaseRequestRequestTypeDef(
     _RequiredUpdateKxDatabaseRequestRequestTypeDef, _OptionalUpdateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
+UpdateKxDatabaseResponseTypeDef = TypedDict(
+    "UpdateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "environmentId": str,
+        "description": str,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
@@ -725,22 +813,20 @@
         "name": str,
         "description": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateKxEnvironmentRequestRequestTypeDef(
     _RequiredUpdateKxEnvironmentRequestRequestTypeDef,
     _OptionalUpdateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -749,20 +835,29 @@
     "_OptionalUpdateKxUserRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateKxUserRequestRequestTypeDef(
     _RequiredUpdateKxUserRequestRequestTypeDef, _OptionalUpdateKxUserRequestRequestTypeDef
 ):
     pass
 
+UpdateKxUserResponseTypeDef = TypedDict(
+    "UpdateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CreateKxChangesetRequestRequestTypeDef = TypedDict(
     "CreateKxChangesetRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
@@ -802,21 +897,19 @@
         "description": str,
         "federationMode": FederationModeType,
         "federationParameters": FederationParametersTypeDef,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -829,147 +922,31 @@
         "federationParameters": FederationParametersTypeDef,
         "superuserParameters": SuperuserParametersTypeDef,
         "dataBundles": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "environmentArn": str,
-        "environmentUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKxDatabaseResponseTypeDef = TypedDict(
-    "CreateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKxEnvironmentResponseTypeDef = TypedDict(
-    "CreateKxEnvironmentResponseTypeDef",
-    {
-        "name": str,
-        "status": EnvironmentStatusType,
-        "environmentId": str,
-        "description": str,
-        "environmentArn": str,
-        "kmsKeyId": str,
-        "creationTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKxUserResponseTypeDef = TypedDict(
-    "CreateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKxConnectionStringResponseTypeDef = TypedDict(
-    "GetKxConnectionStringResponseTypeDef",
-    {
-        "signedConnectionString": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKxDatabaseResponseTypeDef = TypedDict(
-    "GetKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "lastCompletedChangesetId": str,
-        "numBytes": int,
-        "numChangesets": int,
-        "numFiles": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKxUserResponseTypeDef = TypedDict(
-    "GetKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
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
-UpdateKxDatabaseResponseTypeDef = TypedDict(
-    "UpdateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "environmentId": str,
-        "description": str,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateKxUserResponseTypeDef = TypedDict(
-    "UpdateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
@@ -977,15 +954,15 @@
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1001,15 +978,15 @@
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KxEnvironmentTypeDef = TypedDict(
     "KxEnvironmentTypeDef",
     {
         "name": str,
@@ -1045,22 +1022,20 @@
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
     _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
     _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateKxEnvironmentNetworkResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1072,15 +1047,15 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateKxEnvironmentResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1095,33 +1070,33 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxChangesetsResponseTypeDef = TypedDict(
     "ListKxChangesetsResponseTypeDef",
     {
         "kxChangesets": List[KxChangesetListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxClustersResponseTypeDef = TypedDict(
     "ListKxClustersResponseTypeDef",
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
@@ -1132,87 +1107,77 @@
     {
         "cacheConfigurations": Sequence[KxDatabaseCacheConfigurationTypeDef],
         "changesetId": str,
     },
     total=False,
 )
 
-
 class KxDatabaseConfigurationTypeDef(
     _RequiredKxDatabaseConfigurationTypeDef, _OptionalKxDatabaseConfigurationTypeDef
 ):
     pass
 
-
 ListKxDatabasesResponseTypeDef = TypedDict(
     "ListKxDatabasesResponseTypeDef",
     {
         "kxDatabases": List[KxDatabaseListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxClusterNodesResponseTypeDef = TypedDict(
     "ListKxClusterNodesResponseTypeDef",
     {
         "nodes": List[KxNodeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxUsersResponseTypeDef = TypedDict(
     "ListKxUsersResponseTypeDef",
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxEnvironmentsResponseTypeDef = TypedDict(
     "ListKxEnvironmentsResponseTypeDef",
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -1239,21 +1204,19 @@
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "availabilityZoneId": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateKxClusterRequestRequestTypeDef(
     _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
 ):
     pass
 
-
 CreateKxClusterResponseTypeDef = TypedDict(
     "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
@@ -1270,15 +1233,15 @@
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxClusterResponseTypeDef = TypedDict(
     "GetKxClusterResponseTypeDef",
     {
         "status": KxClusterStatusType,
@@ -1297,15 +1260,15 @@
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -1317,13 +1280,12 @@
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateKxClusterDatabasesRequestRequestTypeDef(
     _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef,
     _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/type_defs.pyi` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,92 +33,93 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AutoScalingConfigurationTypeDef",
     "CapacityConfigurationTypeDef",
     "ChangeRequestTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
+    "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
+    "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
+    "CreateKxUserResponseTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
+    "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
+    "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
     "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
+    "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
     "ListKxClustersRequestRequestTypeDef",
     "ListKxDatabasesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
+    "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
+    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
     "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "CreateKxDatabaseResponseTypeDef",
-    "CreateKxEnvironmentResponseTypeDef",
-    "CreateKxUserResponseTypeDef",
-    "GetKxConnectionStringResponseTypeDef",
-    "GetKxDatabaseResponseTypeDef",
-    "GetKxUserResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateKxDatabaseResponseTypeDef",
-    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
     "CreateKxClusterRequestRequestTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
@@ -158,17 +159,19 @@
     "_OptionalChangeRequestTypeDef",
     {
         "s3Path": str,
     },
     total=False,
 )
 
+
 class ChangeRequestTypeDef(_RequiredChangeRequestTypeDef, _OptionalChangeRequestTypeDef):
     pass
 
+
 CodeConfigurationTypeDef = TypedDict(
     "CodeConfigurationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "s3ObjectVersion": str,
     },
@@ -193,22 +196,21 @@
     {
         "emailAddress": str,
         "firstName": str,
         "lastName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "environmentId": str,
+        "environmentArn": str,
+        "environmentUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "errorMessage": str,
@@ -266,19 +268,34 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateKxDatabaseRequestRequestTypeDef(
     _RequiredCreateKxDatabaseRequestRequestTypeDef, _OptionalCreateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
+
+CreateKxDatabaseResponseTypeDef = TypedDict(
+    "CreateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxEnvironmentRequestRequestTypeDef",
     {
         "name": str,
         "kmsKeyId": str,
     },
 )
@@ -288,20 +305,36 @@
         "description": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateKxEnvironmentRequestRequestTypeDef(
     _RequiredCreateKxEnvironmentRequestRequestTypeDef,
     _OptionalCreateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
+
+CreateKxEnvironmentResponseTypeDef = TypedDict(
+    "CreateKxEnvironmentResponseTypeDef",
+    {
+        "name": str,
+        "status": EnvironmentStatusType,
+        "environmentId": str,
+        "description": str,
+        "environmentArn": str,
+        "kmsKeyId": str,
+        "creationTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -311,19 +344,32 @@
     {
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateKxUserRequestRequestTypeDef(
     _RequiredCreateKxUserRequestRequestTypeDef, _OptionalCreateKxUserRequestRequestTypeDef
 ):
     pass
 
+
+CreateKxUserResponseTypeDef = TypedDict(
+    "CreateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -346,19 +392,21 @@
     "_OptionalDeleteKxClusterRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteKxClusterRequestRequestTypeDef(
     _RequiredDeleteKxClusterRequestRequestTypeDef, _OptionalDeleteKxClusterRequestRequestTypeDef
 ):
     pass
 
+
 DeleteKxDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "clientToken": str,
     },
@@ -408,22 +456,47 @@
     {
         "userArn": str,
         "environmentId": str,
         "clusterName": str,
     },
 )
 
+GetKxConnectionStringResponseTypeDef = TypedDict(
+    "GetKxConnectionStringResponseTypeDef",
+    {
+        "signedConnectionString": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetKxDatabaseRequestRequestTypeDef = TypedDict(
     "GetKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
     },
 )
 
+GetKxDatabaseResponseTypeDef = TypedDict(
+    "GetKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "lastCompletedChangesetId": str,
+        "numBytes": int,
+        "numChangesets": int,
+        "numFiles": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
@@ -439,14 +512,25 @@
     "GetKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
+GetKxUserResponseTypeDef = TypedDict(
+    "GetKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KxChangesetListEntryTypeDef = TypedDict(
     "KxChangesetListEntryTypeDef",
     {
         "changesetId": str,
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
@@ -535,19 +619,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListKxChangesetsRequestRequestTypeDef(
     _RequiredListKxChangesetsRequestRequestTypeDef, _OptionalListKxChangesetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListKxClusterNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListKxClusterNodesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
     },
 )
@@ -556,20 +642,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListKxClusterNodesRequestRequestTypeDef(
     _RequiredListKxClusterNodesRequestRequestTypeDef,
     _OptionalListKxClusterNodesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListKxClustersRequestRequestTypeDef = TypedDict(
     "_RequiredListKxClustersRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalListKxClustersRequestRequestTypeDef = TypedDict(
@@ -578,19 +666,21 @@
         "clusterType": KxClusterTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListKxClustersRequestRequestTypeDef(
     _RequiredListKxClustersRequestRequestTypeDef, _OptionalListKxClustersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListKxDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListKxDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalListKxDatabasesRequestRequestTypeDef = TypedDict(
@@ -598,25 +688,25 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListKxDatabasesRequestRequestTypeDef(
     _RequiredListKxDatabasesRequestRequestTypeDef, _OptionalListKxDatabasesRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListKxEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListKxEnvironmentsRequestRequestTypeDef",
     {
@@ -637,26 +727,57 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListKxUsersRequestRequestTypeDef(
     _RequiredListKxUsersRequestRequestTypeDef, _OptionalListKxUsersRequestRequestTypeDef
 ):
     pass
 
+
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -681,19 +802,32 @@
     "_OptionalUpdateKxDatabaseRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateKxDatabaseRequestRequestTypeDef(
     _RequiredUpdateKxDatabaseRequestRequestTypeDef, _OptionalUpdateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
+
+UpdateKxDatabaseResponseTypeDef = TypedDict(
+    "UpdateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "environmentId": str,
+        "description": str,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
@@ -702,20 +836,22 @@
         "name": str,
         "description": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateKxEnvironmentRequestRequestTypeDef(
     _RequiredUpdateKxEnvironmentRequestRequestTypeDef,
     _OptionalUpdateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -724,19 +860,32 @@
     "_OptionalUpdateKxUserRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateKxUserRequestRequestTypeDef(
     _RequiredUpdateKxUserRequestRequestTypeDef, _OptionalUpdateKxUserRequestRequestTypeDef
 ):
     pass
 
+
+UpdateKxUserResponseTypeDef = TypedDict(
+    "UpdateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateKxChangesetRequestRequestTypeDef = TypedDict(
     "CreateKxChangesetRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
@@ -775,19 +924,21 @@
         "description": str,
         "federationMode": FederationModeType,
         "federationParameters": FederationParametersTypeDef,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -800,145 +951,33 @@
         "federationParameters": FederationParametersTypeDef,
         "superuserParameters": SuperuserParametersTypeDef,
         "dataBundles": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "environmentArn": str,
-        "environmentUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKxDatabaseResponseTypeDef = TypedDict(
-    "CreateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKxEnvironmentResponseTypeDef = TypedDict(
-    "CreateKxEnvironmentResponseTypeDef",
-    {
-        "name": str,
-        "status": EnvironmentStatusType,
-        "environmentId": str,
-        "description": str,
-        "environmentArn": str,
-        "kmsKeyId": str,
-        "creationTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKxUserResponseTypeDef = TypedDict(
-    "CreateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKxConnectionStringResponseTypeDef = TypedDict(
-    "GetKxConnectionStringResponseTypeDef",
-    {
-        "signedConnectionString": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKxDatabaseResponseTypeDef = TypedDict(
-    "GetKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "lastCompletedChangesetId": str,
-        "numBytes": int,
-        "numChangesets": int,
-        "numFiles": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetKxUserResponseTypeDef = TypedDict(
-    "GetKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
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
-UpdateKxDatabaseResponseTypeDef = TypedDict(
-    "UpdateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "environmentId": str,
-        "description": str,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateKxUserResponseTypeDef = TypedDict(
-    "UpdateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
@@ -946,15 +985,15 @@
         "environmentId": str,
         "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -970,15 +1009,15 @@
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KxEnvironmentTypeDef = TypedDict(
     "KxEnvironmentTypeDef",
     {
         "name": str,
@@ -1014,20 +1053,22 @@
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
     _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
     _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateKxEnvironmentNetworkResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1039,15 +1080,15 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateKxEnvironmentResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1062,33 +1103,33 @@
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
         "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
         "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxChangesetsResponseTypeDef = TypedDict(
     "ListKxChangesetsResponseTypeDef",
     {
         "kxChangesets": List[KxChangesetListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxClustersResponseTypeDef = TypedDict(
     "ListKxClustersResponseTypeDef",
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredKxDatabaseConfigurationTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationTypeDef",
     {
         "databaseName": str,
@@ -1099,85 +1140,79 @@
     {
         "cacheConfigurations": Sequence[KxDatabaseCacheConfigurationTypeDef],
         "changesetId": str,
     },
     total=False,
 )
 
+
 class KxDatabaseConfigurationTypeDef(
     _RequiredKxDatabaseConfigurationTypeDef, _OptionalKxDatabaseConfigurationTypeDef
 ):
     pass
 
+
 ListKxDatabasesResponseTypeDef = TypedDict(
     "ListKxDatabasesResponseTypeDef",
     {
         "kxDatabases": List[KxDatabaseListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxClusterNodesResponseTypeDef = TypedDict(
     "ListKxClusterNodesResponseTypeDef",
     {
         "nodes": List[KxNodeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxUsersResponseTypeDef = TypedDict(
     "ListKxUsersResponseTypeDef",
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKxEnvironmentsResponseTypeDef = TypedDict(
     "ListKxEnvironmentsResponseTypeDef",
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -1204,19 +1239,21 @@
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "availabilityZoneId": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateKxClusterRequestRequestTypeDef(
     _RequiredCreateKxClusterRequestRequestTypeDef, _OptionalCreateKxClusterRequestRequestTypeDef
 ):
     pass
 
+
 CreateKxClusterResponseTypeDef = TypedDict(
     "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
@@ -1233,15 +1270,15 @@
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKxClusterResponseTypeDef = TypedDict(
     "GetKxClusterResponseTypeDef",
     {
         "status": KxClusterStatusType,
@@ -1260,15 +1297,15 @@
         "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
         "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -1280,12 +1317,13 @@
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateKxClusterDatabasesRequestRequestTypeDef(
     _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef,
     _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/PKG-INFO` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.26.147
-Summary: Type annotations for boto3.finspace 1.26.147 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.finspace 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.26.147](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,85 +339,85 @@
 from mypy_boto3_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
+    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
+    CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
+    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
+    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
     TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
+    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
     EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    CreateKxDatabaseResponseTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
-    CreateKxUserResponseTypeDef,
-    GetKxConnectionStringResponseTypeDef,
-    GetKxDatabaseResponseTypeDef,
-    GetKxUserResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
```

### Comparing `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.26.147/setup.py` & `mypy-boto3-finspace-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.26.147",
+    version="1.27.0",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.finspace 1.26.147 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.finspace 1.27.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


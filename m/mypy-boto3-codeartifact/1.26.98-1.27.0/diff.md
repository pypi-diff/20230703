# Comparing `tmp/mypy-boto3-codeartifact-1.26.98.tar.gz` & `tmp/mypy-boto3-codeartifact-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeartifact-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-codeartifact-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-codeartifact-1.26.98.tar` & `mypy-boto3-codeartifact-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.395626 mypy-boto3-codeartifact-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18322 2023-03-23 19:33:04.391626 mypy-boto3-codeartifact-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.391626 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46848 2023-03-23 19:32:09.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46769 2023-03-23 19:32:09.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.391626 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18322 2023-03-23 19:33:04.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-23 19:33:04.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-23 19:33:04.000000 mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.395626 mypy-boto3-codeartifact-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-23 19:32:07.000000 mypy-boto3-codeartifact-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.762984 mypy-boto3-codeartifact-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-03 19:50:31.758984 mypy-boto3-codeartifact-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.754984 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-03 19:34:06.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-03 19:34:06.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-03 19:34:06.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-03 19:34:06.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-03 19:34:06.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46932 2023-07-03 19:34:07.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46853 2023-07-03 19:34:06.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.758984 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-03 19:50:31.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:31.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:31.000000 mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.762984 mypy-boto3-codeartifact-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:34:05.000000 mypy-boto3-codeartifact-1.27.0/setup.py
```

### Comparing `mypy-boto3-codeartifact-1.26.98/LICENSE` & `mypy-boto3-codeartifact-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.26.98/PKG-INFO` & `mypy-boto3-codeartifact-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.26.98
-Summary: Type annotations for boto3.CodeArtifact 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeArtifact 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,15 +354,14 @@
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -377,43 +376,50 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
+    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PackageOriginRestrictionsTypeDef,
+    PaginatorConfigTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
-    GetPackageVersionAssetResultTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
@@ -428,20 +434,14 @@
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.26.98/README.md` & `mypy-boto3-codeartifact-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,15 +322,14 @@
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -345,43 +344,50 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
+    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PackageOriginRestrictionsTypeDef,
+    PaginatorConfigTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
-    GetPackageVersionAssetResultTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
@@ -396,20 +402,14 @@
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/__init__.py` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/__init__.pyi` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/__main__.py` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeArtifact 1.26.98\nVersion:         1.26.98\nBuilder"
-        " version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.CodeArtifact 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.98")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/client.py` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/client.pyi` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/literals.py` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
     "ListDomainsPaginatorName",
@@ -39,15 +38,14 @@
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
 ListDomainsPaginatorName = Literal["list_domains"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
@@ -81,14 +79,15 @@
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
@@ -128,14 +127,15 @@
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
@@ -277,14 +277,15 @@
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
@@ -303,16 +304,19 @@
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
@@ -396,15 +400,17 @@
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
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/literals.pyi` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AllowPublishType",
     "AllowUpstreamType",
     "DomainStatusType",
     "ExternalConnectionStatusType",
     "HashAlgorithmType",
     "ListDomainsPaginatorName",
@@ -38,14 +39,15 @@
     "CodeArtifactServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AllowPublishType = Literal["ALLOW", "BLOCK"]
 AllowUpstreamType = Literal["ALLOW", "BLOCK"]
 DomainStatusType = Literal["Active", "Deleted"]
 ExternalConnectionStatusType = Literal["Available"]
 HashAlgorithmType = Literal["MD5", "SHA-1", "SHA-256", "SHA-512"]
 ListDomainsPaginatorName = Literal["list_domains"]
 ListPackageVersionAssetsPaginatorName = Literal["list_package_version_assets"]
@@ -79,14 +81,15 @@
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
@@ -126,14 +129,15 @@
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
@@ -275,14 +279,15 @@
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
@@ -301,16 +306,19 @@
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
@@ -394,15 +402,17 @@
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
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/paginator.py` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,50 +52,45 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDomainsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
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
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
         """
 
-
 class ListPackageVersionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
     """
 
     def paginate(
@@ -104,22 +99,21 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
-
 class ListPackageVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
     """
 
     def paginate(
@@ -130,22 +124,21 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
         """
 
-
 class ListPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
     """
 
     def paginate(
@@ -155,49 +148,47 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
         """
 
-
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, repositoryPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, repositoryPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
         """
 
-
 class ListRepositoriesInDomainPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
     """
 
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/paginator.pyi` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,45 +52,50 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListDomainsPaginator",
     "ListPackageVersionAssetsPaginator",
     "ListPackageVersionsPaginator",
     "ListPackagesPaginator",
     "ListRepositoriesPaginator",
     "ListRepositoriesInDomainPaginator",
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
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
         """
 
+
 class ListPackageVersionAssetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
     """
 
     def paginate(
@@ -99,21 +104,22 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
+
 class ListPackageVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
     """
 
     def paginate(
@@ -124,21 +130,22 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
         """
 
+
 class ListPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
     """
 
     def paginate(
@@ -148,47 +155,49 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
         """
 
+
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, repositoryPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, repositoryPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
         """
 
+
 class ListRepositoriesInDomainPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
     """
 
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/type_defs.py` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -60,43 +59,50 @@
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
+    "GetAuthorizationTokenResultTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
+    "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
+    "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
+    "GetRepositoryEndpointResultTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
+    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PackageOriginRestrictionsTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
-    "GetAuthorizationTokenResultTypeDef",
-    "GetPackageVersionAssetResultTypeDef",
-    "GetPackageVersionReadmeResultTypeDef",
-    "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
@@ -111,20 +117,14 @@
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
-    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
@@ -185,25 +185,14 @@
 class AssociateExternalConnectionRequestRequestTypeDef(
     _RequiredAssociateExternalConnectionRequestRequestTypeDef,
     _OptionalAssociateExternalConnectionRequestRequestTypeDef,
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
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -623,14 +612,23 @@
 class GetAuthorizationTokenRequestRequestTypeDef(
     _RequiredGetAuthorizationTokenRequestRequestTypeDef,
     _OptionalGetAuthorizationTokenRequestRequestTypeDef,
 ):
     pass
 
 
+GetAuthorizationTokenResultTypeDef = TypedDict(
+    "GetAuthorizationTokenResultTypeDef",
+    {
+        "authorizationToken": str,
+        "expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
@@ -674,14 +672,25 @@
 class GetPackageVersionAssetRequestRequestTypeDef(
     _RequiredGetPackageVersionAssetRequestRequestTypeDef,
     _OptionalGetPackageVersionAssetRequestRequestTypeDef,
 ):
     pass
 
 
+GetPackageVersionAssetResultTypeDef = TypedDict(
+    "GetPackageVersionAssetResultTypeDef",
+    {
+        "asset": StreamingBody,
+        "assetName": str,
+        "packageVersion": str,
+        "packageVersionRevision": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetPackageVersionReadmeRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionReadmeRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -701,14 +710,27 @@
 class GetPackageVersionReadmeRequestRequestTypeDef(
     _RequiredGetPackageVersionReadmeRequestRequestTypeDef,
     _OptionalGetPackageVersionReadmeRequestRequestTypeDef,
 ):
     pass
 
 
+GetPackageVersionReadmeResultTypeDef = TypedDict(
+    "GetPackageVersionReadmeResultTypeDef",
+    {
+        "format": PackageFormatType,
+        "namespace": str,
+        "package": str,
+        "version": str,
+        "versionRevision": str,
+        "readme": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRepositoryEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
     },
@@ -725,14 +747,22 @@
 class GetRepositoryEndpointRequestRequestTypeDef(
     _RequiredGetRepositoryEndpointRequestRequestTypeDef,
     _OptionalGetRepositoryEndpointRequestRequestTypeDef,
 ):
     pass
 
 
+GetRepositoryEndpointResultTypeDef = TypedDict(
+    "GetRepositoryEndpointResultTypeDef",
+    {
+        "repositoryEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -757,33 +787,59 @@
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+    },
+)
+_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
+    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -844,14 +900,44 @@
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
     total=False,
 )
 
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "status": PackageVersionStatusType,
+        "sortBy": Literal["PUBLISHED_TIME"],
+        "originType": PackageVersionOriginTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -875,14 +961,43 @@
 class ListPackageVersionsRequestRequestTypeDef(
     _RequiredListPackageVersionsRequestRequestTypeDef,
     _OptionalListPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+    },
+)
+_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "format": PackageFormatType,
+        "namespace": str,
+        "packagePrefix": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPackagesRequestListPackagesPaginateTypeDef(
+    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
+    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPackagesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -904,14 +1019,39 @@
 
 class ListPackagesRequestRequestTypeDef(
     _RequiredListPackagesRequestRequestTypeDef, _OptionalListPackagesRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "administratorAccount": str,
+        "repositoryPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
+    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesInDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
@@ -944,14 +1084,23 @@
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
     total=False,
 )
 
+ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    {
+        "repositoryPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -969,14 +1118,24 @@
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
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
 _RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishPackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -1067,14 +1226,25 @@
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
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
@@ -1105,116 +1275,75 @@
 class UpdatePackageVersionsStatusRequestRequestTypeDef(
     _RequiredUpdatePackageVersionsStatusRequestRequestTypeDef,
     _OptionalUpdatePackageVersionsStatusRequestRequestTypeDef,
 ):
     pass
 
 
-GetAuthorizationTokenResultTypeDef = TypedDict(
-    "GetAuthorizationTokenResultTypeDef",
-    {
-        "authorizationToken": str,
-        "expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPackageVersionAssetResultTypeDef = TypedDict(
-    "GetPackageVersionAssetResultTypeDef",
-    {
-        "asset": StreamingBody,
-        "assetName": str,
-        "packageVersion": str,
-        "packageVersionRevision": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPackageVersionReadmeResultTypeDef = TypedDict(
-    "GetPackageVersionReadmeResultTypeDef",
-    {
-        "format": PackageFormatType,
-        "namespace": str,
-        "package": str,
-        "version": str,
-        "versionRevision": str,
-        "readme": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRepositoryEndpointResultTypeDef = TypedDict(
-    "GetRepositoryEndpointResultTypeDef",
-    {
-        "repositoryEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "assets": List[AssetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishPackageVersionResultTypeDef = TypedDict(
     "PublishPackageVersionResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageVersionsResultTypeDef = TypedDict(
     "DeletePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisposePackageVersionsResultTypeDef = TypedDict(
     "DisposePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePackageVersionsStatusResultTypeDef = TypedDict(
     "UpdatePackageVersionsStatusResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domain": str,
@@ -1236,15 +1365,15 @@
     pass
 
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1252,31 +1381,31 @@
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainResultTypeDef = TypedDict(
     "DescribeDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
@@ -1325,55 +1454,55 @@
     pass
 
 
 DeleteDomainPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainPermissionsPolicyResultTypeDef = TypedDict(
     "GetDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "GetRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDomainPermissionsPolicyResultTypeDef = TypedDict(
     "PutDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "PutRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
@@ -1383,176 +1512,47 @@
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-    },
-)
-_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
-    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "status": PackageVersionStatusType,
-        "sortBy": Literal["PUBLISHED_TIME"],
-        "originType": PackageVersionOriginTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-    },
-)
-_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "format": PackageFormatType,
-        "namespace": str,
-        "packagePrefix": str,
-        "publish": AllowPublishType,
-        "upstream": AllowUpstreamType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPackagesRequestListPackagesPaginateTypeDef(
-    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
-    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domain": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "administratorAccount": str,
-        "repositoryPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
-    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-):
-    pass
-
-
-ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
-    {
-        "repositoryPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "dependencies": List[PackageDependencyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositoriesInDomainResultTypeDef = TypedDict(
     "ListRepositoriesInDomainResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositoriesResultTypeDef = TypedDict(
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
         "restrictions": PackageOriginRestrictionsTypeDef,
@@ -1668,104 +1668,104 @@
     total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateExternalConnectionResultTypeDef = TypedDict(
     "AssociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryResultTypeDef = TypedDict(
     "CreateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryResultTypeDef = TypedDict(
     "DeleteRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoryResultTypeDef = TypedDict(
     "DescribeRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateExternalConnectionResultTypeDef = TypedDict(
     "DisassociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRepositoryResultTypeDef = TypedDict(
     "UpdateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackageVersionResultTypeDef = TypedDict(
     "DescribePackageVersionResultTypeDef",
     {
         "packageVersion": PackageVersionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackageVersionsResultTypeDef = TypedDict(
     "ListPackageVersionsResultTypeDef",
     {
         "defaultDisplayVersion": str,
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageResultTypeDef = TypedDict(
     "DeletePackageResultTypeDef",
     {
         "deletedPackage": PackageSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesResultTypeDef = TypedDict(
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact/type_defs.pyi` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -59,43 +58,50 @@
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
+    "GetAuthorizationTokenResultTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
+    "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
+    "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
+    "GetRepositoryEndpointResultTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
+    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PackageOriginRestrictionsTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
-    "GetAuthorizationTokenResultTypeDef",
-    "GetPackageVersionAssetResultTypeDef",
-    "GetPackageVersionReadmeResultTypeDef",
-    "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
@@ -110,20 +116,14 @@
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
-    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
@@ -180,25 +180,14 @@
 
 class AssociateExternalConnectionRequestRequestTypeDef(
     _RequiredAssociateExternalConnectionRequestRequestTypeDef,
     _OptionalAssociateExternalConnectionRequestRequestTypeDef,
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
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -590,14 +579,23 @@
 
 class GetAuthorizationTokenRequestRequestTypeDef(
     _RequiredGetAuthorizationTokenRequestRequestTypeDef,
     _OptionalGetAuthorizationTokenRequestRequestTypeDef,
 ):
     pass
 
+GetAuthorizationTokenResultTypeDef = TypedDict(
+    "GetAuthorizationTokenResultTypeDef",
+    {
+        "authorizationToken": str,
+        "expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
@@ -637,14 +635,25 @@
 
 class GetPackageVersionAssetRequestRequestTypeDef(
     _RequiredGetPackageVersionAssetRequestRequestTypeDef,
     _OptionalGetPackageVersionAssetRequestRequestTypeDef,
 ):
     pass
 
+GetPackageVersionAssetResultTypeDef = TypedDict(
+    "GetPackageVersionAssetResultTypeDef",
+    {
+        "asset": StreamingBody,
+        "assetName": str,
+        "packageVersion": str,
+        "packageVersionRevision": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetPackageVersionReadmeRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionReadmeRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -662,14 +671,27 @@
 
 class GetPackageVersionReadmeRequestRequestTypeDef(
     _RequiredGetPackageVersionReadmeRequestRequestTypeDef,
     _OptionalGetPackageVersionReadmeRequestRequestTypeDef,
 ):
     pass
 
+GetPackageVersionReadmeResultTypeDef = TypedDict(
+    "GetPackageVersionReadmeResultTypeDef",
+    {
+        "format": PackageFormatType,
+        "namespace": str,
+        "package": str,
+        "version": str,
+        "versionRevision": str,
+        "readme": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRepositoryEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
     },
@@ -684,14 +706,22 @@
 
 class GetRepositoryEndpointRequestRequestTypeDef(
     _RequiredGetRepositoryEndpointRequestRequestTypeDef,
     _OptionalGetRepositoryEndpointRequestRequestTypeDef,
 ):
     pass
 
+GetRepositoryEndpointResultTypeDef = TypedDict(
+    "GetRepositoryEndpointResultTypeDef",
+    {
+        "repositoryEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -714,33 +744,57 @@
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+    },
+)
+_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
+    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -797,14 +851,42 @@
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
     total=False,
 )
 
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "status": PackageVersionStatusType,
+        "sortBy": Literal["PUBLISHED_TIME"],
+        "originType": PackageVersionOriginTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -826,14 +908,41 @@
 
 class ListPackageVersionsRequestRequestTypeDef(
     _RequiredListPackageVersionsRequestRequestTypeDef,
     _OptionalListPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+    },
+)
+_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "format": PackageFormatType,
+        "namespace": str,
+        "packagePrefix": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPackagesRequestListPackagesPaginateTypeDef(
+    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
+    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
+):
+    pass
+
 _RequiredListPackagesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -853,14 +962,37 @@
 )
 
 class ListPackagesRequestRequestTypeDef(
     _RequiredListPackagesRequestRequestTypeDef, _OptionalListPackagesRequestRequestTypeDef
 ):
     pass
 
+_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "administratorAccount": str,
+        "repositoryPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
+    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+):
+    pass
+
 _RequiredListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesInDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
@@ -891,14 +1023,23 @@
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
     total=False,
 )
 
+ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    {
+        "repositoryPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -916,14 +1057,24 @@
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
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
 _RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishPackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -1008,14 +1159,25 @@
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
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
@@ -1044,116 +1206,75 @@
 
 class UpdatePackageVersionsStatusRequestRequestTypeDef(
     _RequiredUpdatePackageVersionsStatusRequestRequestTypeDef,
     _OptionalUpdatePackageVersionsStatusRequestRequestTypeDef,
 ):
     pass
 
-GetAuthorizationTokenResultTypeDef = TypedDict(
-    "GetAuthorizationTokenResultTypeDef",
-    {
-        "authorizationToken": str,
-        "expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPackageVersionAssetResultTypeDef = TypedDict(
-    "GetPackageVersionAssetResultTypeDef",
-    {
-        "asset": StreamingBody,
-        "assetName": str,
-        "packageVersion": str,
-        "packageVersionRevision": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPackageVersionReadmeResultTypeDef = TypedDict(
-    "GetPackageVersionReadmeResultTypeDef",
-    {
-        "format": PackageFormatType,
-        "namespace": str,
-        "package": str,
-        "version": str,
-        "versionRevision": str,
-        "readme": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRepositoryEndpointResultTypeDef = TypedDict(
-    "GetRepositoryEndpointResultTypeDef",
-    {
-        "repositoryEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "assets": List[AssetSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishPackageVersionResultTypeDef = TypedDict(
     "PublishPackageVersionResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageVersionsResultTypeDef = TypedDict(
     "DeletePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisposePackageVersionsResultTypeDef = TypedDict(
     "DisposePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePackageVersionsStatusResultTypeDef = TypedDict(
     "UpdatePackageVersionsStatusResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domain": str,
@@ -1173,15 +1294,15 @@
 ):
     pass
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1189,31 +1310,31 @@
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDomainResultTypeDef = TypedDict(
     "DescribeDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
@@ -1258,55 +1379,55 @@
 ):
     pass
 
 DeleteDomainPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainPermissionsPolicyResultTypeDef = TypedDict(
     "GetDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "GetRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDomainPermissionsPolicyResultTypeDef = TypedDict(
     "PutDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "PutRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
@@ -1316,168 +1437,47 @@
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-    },
-)
-_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
-    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "status": PackageVersionStatusType,
-        "sortBy": Literal["PUBLISHED_TIME"],
-        "originType": PackageVersionOriginTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-    },
-)
-_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "format": PackageFormatType,
-        "namespace": str,
-        "packagePrefix": str,
-        "publish": AllowPublishType,
-        "upstream": AllowUpstreamType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPackagesRequestListPackagesPaginateTypeDef(
-    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
-    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
-):
-    pass
-
-_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "administratorAccount": str,
-        "repositoryPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
-    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-):
-    pass
-
-ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
-    {
-        "repositoryPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "dependencies": List[PackageDependencyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositoriesInDomainResultTypeDef = TypedDict(
     "ListRepositoriesInDomainResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRepositoriesResultTypeDef = TypedDict(
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
         "restrictions": PackageOriginRestrictionsTypeDef,
@@ -1589,104 +1589,104 @@
     total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateExternalConnectionResultTypeDef = TypedDict(
     "AssociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryResultTypeDef = TypedDict(
     "CreateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryResultTypeDef = TypedDict(
     "DeleteRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoryResultTypeDef = TypedDict(
     "DescribeRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateExternalConnectionResultTypeDef = TypedDict(
     "DisassociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRepositoryResultTypeDef = TypedDict(
     "UpdateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackageVersionResultTypeDef = TypedDict(
     "DescribePackageVersionResultTypeDef",
     {
         "packageVersion": PackageVersionDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackageVersionsResultTypeDef = TypedDict(
     "ListPackageVersionsResultTypeDef",
     {
         "defaultDisplayVersion": str,
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeletePackageResultTypeDef = TypedDict(
     "DeletePackageResultTypeDef",
     {
         "deletedPackage": PackageSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesResultTypeDef = TypedDict(
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/PKG-INFO` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.26.98
-Summary: Type annotations for boto3.CodeArtifact 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeArtifact 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,15 +354,14 @@
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -377,43 +376,50 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
+    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PackageOriginRestrictionsTypeDef,
+    PaginatorConfigTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
-    GetPackageVersionAssetResultTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
@@ -428,20 +434,14 @@
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.26.98/mypy_boto3_codeartifact.egg-info/SOURCES.txt` & `mypy-boto3-codeartifact-1.27.0/mypy_boto3_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.26.98/setup.py` & `mypy-boto3-codeartifact-1.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeartifact",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeArtifact 1.26.98 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.CodeArtifact 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


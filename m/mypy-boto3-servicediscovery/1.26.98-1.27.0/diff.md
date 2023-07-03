# Comparing `tmp/mypy-boto3-servicediscovery-1.26.98.tar.gz` & `tmp/mypy-boto3-servicediscovery-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicediscovery-1.26.98.tar", last modified: Thu Mar 23 19:33:06 2023, max compression
+gzip compressed data, was "mypy-boto3-servicediscovery-1.27.0.tar", last modified: Mon Jul  3 19:51:27 2023, max compression
```

## Comparing `mypy-boto3-servicediscovery-1.26.98.tar` & `mypy-boto3-servicediscovery-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.899668 mypy-boto3-servicediscovery-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-03-23 19:33:06.895668 mypy-boto3-servicediscovery-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.895668 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28418 2023-03-23 19:32:50.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28382 2023-03-23 19:32:50.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.895668 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-03-23 19:33:06.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-23 19:33:06.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:06.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-23 19:33:06.000000 mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:06.899668 mypy-boto3-servicediscovery-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-23 19:32:49.000000 mypy-boto3-servicediscovery-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.527999 mypy-boto3-servicediscovery-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-03 19:51:27.519999 mypy-boto3-servicediscovery-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.519999 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28472 2023-07-03 19:48:04.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:27.519999 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-03 19:51:27.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:51:27.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:27.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:27.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:27.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:27.000000 mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:27.527999 mypy-boto3-servicediscovery-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 19:48:03.000000 mypy-boto3-servicediscovery-1.27.0/setup.py
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/LICENSE` & `mypy-boto3-servicediscovery-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.26.98/PKG-INFO` & `mypy-boto3-servicediscovery-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.26.98
-Summary: Type annotations for boto3.ServiceDiscovery 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ServiceDiscovery 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-servicediscovery"></a>
 
 # mypy-boto3-servicediscovery
 
 [![PyPI - mypy-boto3-servicediscovery](https://img.shields.io/pypi/v/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicediscovery?color=blue)](https://pypistats.org/packages/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,71 +348,71 @@
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
+    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
+    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
     SOATypeDef,
+    EmptyResponseMetadataTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SOAChangeTypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DeregisterInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdateHttpNamespaceResponseTypeDef,
+    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
     DnsConfigTypeDef,
     DnsPropertiesTypeDef,
     PrivateDnsPropertiesMutableTypeDef,
     PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/README.md` & `mypy-boto3-servicediscovery-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-servicediscovery"></a>
 
 # mypy-boto3-servicediscovery
 
 [![PyPI - mypy-boto3-servicediscovery](https://img.shields.io/pypi/v/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicediscovery?color=blue)](https://pypistats.org/packages/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,71 +316,71 @@
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
+    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
+    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
     SOATypeDef,
+    EmptyResponseMetadataTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SOAChangeTypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DeregisterInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdateHttpNamespaceResponseTypeDef,
+    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
     DnsConfigTypeDef,
     DnsPropertiesTypeDef,
     PrivateDnsPropertiesMutableTypeDef,
     PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/__init__.py` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/__init__.pyi` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/__main__.py` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceDiscovery 1.26.98\nVersion:         1.26.98\nBuilder"
-        " version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.ServiceDiscovery 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/client.py` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/client.pyi` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/literals.py` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,15 @@
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
@@ -134,14 +135,15 @@
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
@@ -283,14 +285,15 @@
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
@@ -309,16 +312,19 @@
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
@@ -402,15 +408,17 @@
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

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/literals.pyi` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,15 @@
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
@@ -132,14 +133,15 @@
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
@@ -281,14 +283,15 @@
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
@@ -307,16 +310,19 @@
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
@@ -400,15 +406,17 @@
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

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/paginator.py` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, ServiceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServiceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
         """
 
 
@@ -79,15 +79,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 
@@ -97,15 +97,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
         """
 
 
@@ -115,13 +115,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/paginator.pyi` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, ServiceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServiceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listinstancespaginator)
         """
 
 class ListNamespacesPaginator(Paginator):
@@ -75,15 +75,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 class ListOperationsPaginator(Paginator):
@@ -92,15 +92,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listoperationspaginator)
         """
 
 class ListServicesPaginator(Paginator):
@@ -109,13 +109,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/type_defs.py` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,71 +40,71 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateHttpNamespaceResponseTypeDef",
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    "CreatePublicDnsNamespaceResponseTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
+    "DeleteNamespaceResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
+    "DeregisterInstanceResponseTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
     "SOATypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
+    "GetInstancesHealthStatusResponseTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "SOAChangeTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
-    "CreateHttpNamespaceRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateHttpNamespaceResponseTypeDef",
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    "CreatePublicDnsNamespaceResponseTypeDef",
-    "DeleteNamespaceResponseTypeDef",
-    "DeregisterInstanceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetInstancesHealthStatusResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegisterInstanceResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdateHttpNamespaceResponseTypeDef",
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
+    "CreateHttpNamespaceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
     "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
     "PrivateDnsPropertiesMutableTypeDef",
     "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
@@ -139,22 +139,35 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateHttpNamespaceResponseTypeDef = TypedDict(
+    "CreateHttpNamespaceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePublicDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -187,14 +200,22 @@
 DeleteNamespaceRequestRequestTypeDef = TypedDict(
     "DeleteNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -202,14 +223,22 @@
     "DeregisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
 
+DeregisterInstanceResponseTypeDef = TypedDict(
+    "DeregisterInstanceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDiscoverInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDiscoverInstancesRequestRequestTypeDef",
     {
         "NamespaceName": str,
         "ServiceName": str,
     },
 )
@@ -254,14 +283,21 @@
 SOATypeDef = TypedDict(
     "SOATypeDef",
     {
         "TTL": int,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
@@ -306,14 +342,23 @@
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
 
+GetInstancesHealthStatusResponseTypeDef = TypedDict(
+    "GetInstancesHealthStatusResponseTypeDef",
+    {
+        "Status": Dict[str, HealthStatusType],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -366,24 +411,36 @@
     {
         "Id": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceId": str,
+    },
+)
+_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListInstancesRequestListInstancesPaginateTypeDef(
+    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
+    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstancesRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalListInstancesRequestRequestTypeDef = TypedDict(
@@ -474,14 +531,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
@@ -504,172 +571,127 @@
 
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+RegisterInstanceResponseTypeDef = TypedDict(
+    "RegisterInstanceResponseTypeDef",
     {
-        "ServiceId": str,
-        "InstanceId": str,
-        "Status": CustomHealthStatusType,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CreatorRequestId": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class CreateHttpNamespaceRequestRequestTypeDef(
-    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
-    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
-):
-    pass
-
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "TagKeys": Sequence[str],
     },
 )
 
-CreateHttpNamespaceResponseTypeDef = TypedDict(
-    "CreateHttpNamespaceResponseTypeDef",
+UpdateHttpNamespaceResponseTypeDef = TypedDict(
+    "UpdateHttpNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePrivateDnsNamespaceResponseTypeDef",
+UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ServiceId": str,
+        "InstanceId": str,
+        "Status": CustomHealthStatusType,
     },
 )
 
-CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePublicDnsNamespaceResponseTypeDef",
+UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePrivateDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
+UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePublicDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeregisterInstanceResponseTypeDef = TypedDict(
-    "DeregisterInstanceResponseTypeDef",
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetInstancesHealthStatusResponseTypeDef = TypedDict(
-    "GetInstancesHealthStatusResponseTypeDef",
+_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
     {
-        "Status": Dict[str, HealthStatusType],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreatorRequestId": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-RegisterInstanceResponseTypeDef = TypedDict(
-    "RegisterInstanceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateHttpNamespaceResponseTypeDef = TypedDict(
-    "UpdateHttpNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class CreateHttpNamespaceRequestRequestTypeDef(
+    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
+    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
+):
+    pass
 
-UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePrivateDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePublicDnsNamespaceResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 DiscoverInstancesResponseTypeDef = TypedDict(
     "DiscoverInstancesResponseTypeDef",
     {
         "Instances": List[HttpInstanceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
@@ -719,23 +741,23 @@
     },
 )
 
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationResponseTypeDef = TypedDict(
     "GetOperationResponseTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateHttpNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -759,45 +781,23 @@
 
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "ServiceId": str,
-    },
-)
-_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListInstancesRequestListInstancesPaginateTypeDef(
-    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
-    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
-):
-    pass
-
-
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
@@ -808,15 +808,15 @@
     total=False,
 )
 
 ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsRequestListOperationsPaginateTypeDef",
     {
         "Filters": Sequence[OperationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
@@ -828,23 +828,23 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "Filters": Sequence[ServiceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
@@ -989,31 +989,31 @@
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "Services": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NamespaceSummaryTypeDef = TypedDict(
     "NamespaceSummaryTypeDef",
     {
         "Id": str,
@@ -1114,23 +1114,23 @@
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "Namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery/type_defs.pyi` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,71 +39,71 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateHttpNamespaceResponseTypeDef",
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    "CreatePublicDnsNamespaceResponseTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
+    "DeleteNamespaceResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
+    "DeregisterInstanceResponseTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
     "SOATypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
+    "GetInstancesHealthStatusResponseTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "SOAChangeTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
-    "CreateHttpNamespaceRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateHttpNamespaceResponseTypeDef",
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    "CreatePublicDnsNamespaceResponseTypeDef",
-    "DeleteNamespaceResponseTypeDef",
-    "DeregisterInstanceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetInstancesHealthStatusResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegisterInstanceResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdateHttpNamespaceResponseTypeDef",
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
+    "CreateHttpNamespaceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
     "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
     "PrivateDnsPropertiesMutableTypeDef",
     "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
@@ -138,22 +138,35 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateHttpNamespaceResponseTypeDef = TypedDict(
+    "CreateHttpNamespaceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePublicDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -184,14 +197,22 @@
 DeleteNamespaceRequestRequestTypeDef = TypedDict(
     "DeleteNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -199,14 +220,22 @@
     "DeregisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
 
+DeregisterInstanceResponseTypeDef = TypedDict(
+    "DeregisterInstanceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDiscoverInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDiscoverInstancesRequestRequestTypeDef",
     {
         "NamespaceName": str,
         "ServiceName": str,
     },
 )
@@ -249,14 +278,21 @@
 SOATypeDef = TypedDict(
     "SOATypeDef",
     {
         "TTL": int,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
@@ -297,14 +333,23 @@
 
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
+GetInstancesHealthStatusResponseTypeDef = TypedDict(
+    "GetInstancesHealthStatusResponseTypeDef",
+    {
+        "Status": Dict[str, HealthStatusType],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -357,24 +402,34 @@
     {
         "Id": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceId": str,
+    },
+)
+_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListInstancesRequestListInstancesPaginateTypeDef(
+    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
+    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
+):
+    pass
+
 _RequiredListInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstancesRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalListInstancesRequestRequestTypeDef = TypedDict(
@@ -457,14 +512,24 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
@@ -485,170 +550,125 @@
 )
 
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+RegisterInstanceResponseTypeDef = TypedDict(
+    "RegisterInstanceResponseTypeDef",
     {
-        "ServiceId": str,
-        "InstanceId": str,
-        "Status": CustomHealthStatusType,
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CreatorRequestId": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class CreateHttpNamespaceRequestRequestTypeDef(
-    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
-    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
-):
-    pass
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "TagKeys": Sequence[str],
     },
 )
 
-CreateHttpNamespaceResponseTypeDef = TypedDict(
-    "CreateHttpNamespaceResponseTypeDef",
+UpdateHttpNamespaceResponseTypeDef = TypedDict(
+    "UpdateHttpNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePrivateDnsNamespaceResponseTypeDef",
+UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ServiceId": str,
+        "InstanceId": str,
+        "Status": CustomHealthStatusType,
     },
 )
 
-CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePublicDnsNamespaceResponseTypeDef",
+UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePrivateDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
+UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePublicDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeregisterInstanceResponseTypeDef = TypedDict(
-    "DeregisterInstanceResponseTypeDef",
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
     },
 )
-
-GetInstancesHealthStatusResponseTypeDef = TypedDict(
-    "GetInstancesHealthStatusResponseTypeDef",
+_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
     {
-        "Status": Dict[str, HealthStatusType],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreatorRequestId": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+class CreateHttpNamespaceRequestRequestTypeDef(
+    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
+    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
+):
+    pass
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterInstanceResponseTypeDef = TypedDict(
-    "RegisterInstanceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateHttpNamespaceResponseTypeDef = TypedDict(
-    "UpdateHttpNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePrivateDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePublicDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 DiscoverInstancesResponseTypeDef = TypedDict(
     "DiscoverInstancesResponseTypeDef",
     {
         "Instances": List[HttpInstanceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
@@ -696,23 +716,23 @@
     },
 )
 
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOperationResponseTypeDef = TypedDict(
     "GetOperationResponseTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateHttpNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -734,43 +754,23 @@
     pass
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "ServiceId": str,
-    },
-)
-_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListInstancesRequestListInstancesPaginateTypeDef(
-    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
-    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
-):
-    pass
-
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
@@ -781,15 +781,15 @@
     total=False,
 )
 
 ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsRequestListOperationsPaginateTypeDef",
     {
         "Filters": Sequence[OperationFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
@@ -801,23 +801,23 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "Filters": Sequence[ServiceFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
@@ -960,31 +960,31 @@
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "Services": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NamespaceSummaryTypeDef = TypedDict(
     "NamespaceSummaryTypeDef",
     {
         "Id": str,
@@ -1081,23 +1081,23 @@
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "Namespace": NamespaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/PKG-INFO` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.26.98
-Summary: Type annotations for boto3.ServiceDiscovery 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ServiceDiscovery 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-servicediscovery"></a>
 
 # mypy-boto3-servicediscovery
 
 [![PyPI - mypy-boto3-servicediscovery](https://img.shields.io/pypi/v/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicediscovery?color=blue)](https://pypistats.org/packages/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,71 +348,71 @@
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
+    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
+    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
     SOATypeDef,
+    EmptyResponseMetadataTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SOAChangeTypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
-    DeleteNamespaceResponseTypeDef,
-    DeregisterInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdateHttpNamespaceResponseTypeDef,
+    UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
     DnsConfigTypeDef,
     DnsPropertiesTypeDef,
     PrivateDnsPropertiesMutableTypeDef,
     PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-servicediscovery-1.26.98/mypy_boto3_servicediscovery.egg-info/SOURCES.txt` & `mypy-boto3-servicediscovery-1.27.0/mypy_boto3_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.26.98/setup.py` & `mypy-boto3-servicediscovery-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicediscovery",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceDiscovery 1.26.98 service generated with"
-        " mypy-boto3-builder 7.14.2"
+        "Type annotations for boto3.ServiceDiscovery 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


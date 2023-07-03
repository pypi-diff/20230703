# Comparing `tmp/mypy-boto3-appmesh-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-appmesh-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appmesh-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:05 2022, max compression
+gzip compressed data, was "mypy-boto3-appmesh-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-appmesh-1.26.0.post1.tar` & `mypy-boto3-appmesh-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:05.748831 mypy-boto3-appmesh-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22409 2022-11-01 21:43:05.748831 mypy-boto3-appmesh-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20968 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:05.748831 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30229 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    30176 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10330 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10328 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9467 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9457 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    80398 2022-11-01 21:30:36.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    80247 2022-11-01 21:30:35.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:05.748831 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22409 2022-11-01 21:43:05.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-11-01 21:43:05.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:05.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:05.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:05.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-01 21:43:05.000000 mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:05.748831 mypy-boto3-appmesh-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-11-01 21:30:34.000000 mypy-boto3-appmesh-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.598823 mypy-boto3-appmesh-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-07-03 19:50:22.590823 mypy-boto3-appmesh-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20946 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.586823 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80486 2023-07-03 19:32:38.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80335 2023-07-03 19:32:38.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.590823 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22431 2023-07-03 19:50:22.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:50:22.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:22.000000 mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.598823 mypy-boto3-appmesh-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:32:36.000000 mypy-boto3-appmesh-1.27.0/setup.py
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/LICENSE` & `mypy-boto3-appmesh-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-appmesh-1.26.0.post1/PKG-INFO` & `mypy-boto3-appmesh-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.AppMesh 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AppMesh 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
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
 
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appmesh?color=blue)](https://pypistats.org/packages/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,15 +375,14 @@
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
-    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
@@ -406,35 +406,44 @@
     WeightedTargetTypeDef,
     HealthCheckPolicyTypeDef,
     HttpPathMatchTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
     QueryParameterMatchTypeDef,
     JsonFormatRefTypeDef,
-    PaginatorConfigTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
     ListenerTlsAcmCertificateTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
     PortMappingTypeDef,
     MeshStatusTypeDef,
     MeshServiceDiscoveryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
     TcpRouteMatchTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
@@ -455,16 +464,16 @@
     VirtualNodeStatusTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
     ClientTlsCertificateTypeDef,
-    TagResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TagResourceInputRequestTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
@@ -475,22 +484,14 @@
     HeaderMatchMethodTypeDef,
     GrpcRouteActionTypeDef,
     HttpRouteActionTypeDef,
     TcpRouteActionTypeDef,
     HttpGatewayRouteRewriteTypeDef,
     HttpQueryParameterTypeDef,
     LoggingFormatTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     ListenerTlsCertificateTypeDef,
@@ -610,42 +611,42 @@
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

### Comparing `mypy-boto3-appmesh-1.26.0.post1/README.md` & `mypy-boto3-appmesh-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appmesh?color=blue)](https://pypistats.org/packages/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,15 +343,14 @@
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
-    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
@@ -375,35 +374,44 @@
     WeightedTargetTypeDef,
     HealthCheckPolicyTypeDef,
     HttpPathMatchTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
     QueryParameterMatchTypeDef,
     JsonFormatRefTypeDef,
-    PaginatorConfigTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
     ListenerTlsAcmCertificateTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
     PortMappingTypeDef,
     MeshStatusTypeDef,
     MeshServiceDiscoveryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
     TcpRouteMatchTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
@@ -424,16 +432,16 @@
     VirtualNodeStatusTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
     ClientTlsCertificateTypeDef,
-    TagResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TagResourceInputRequestTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
@@ -444,22 +452,14 @@
     HeaderMatchMethodTypeDef,
     GrpcRouteActionTypeDef,
     HttpRouteActionTypeDef,
     TcpRouteActionTypeDef,
     HttpGatewayRouteRewriteTypeDef,
     HttpQueryParameterTypeDef,
     LoggingFormatTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     ListenerTlsCertificateTypeDef,
@@ -579,42 +579,42 @@
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

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/__init__.py` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/__init__.pyi` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/__main__.py` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppMesh 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.AppMesh 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/client.py` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/client.pyi` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/literals.py` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,23 +100,25 @@
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
@@ -126,30 +128,35 @@
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
@@ -175,14 +182,15 @@
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
@@ -227,51 +235,57 @@
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
@@ -284,14 +298,15 @@
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
@@ -303,28 +318,35 @@
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
@@ -333,14 +355,15 @@
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
@@ -351,55 +374,64 @@
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
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/literals.pyi` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -98,23 +98,25 @@
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
@@ -124,30 +126,35 @@
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
@@ -173,14 +180,15 @@
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
@@ -225,51 +233,57 @@
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
@@ -282,14 +296,15 @@
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
@@ -301,28 +316,35 @@
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
@@ -331,14 +353,15 @@
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
@@ -349,55 +372,64 @@
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
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/paginator.py` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -56,146 +56,152 @@
     "ListTagsForResourcePaginator",
     "ListVirtualGatewaysPaginator",
     "ListVirtualNodesPaginator",
     "ListVirtualRoutersPaginator",
     "ListVirtualServicesPaginator",
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
 class ListGatewayRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
         """
 
-
 class ListMeshesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMeshesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
         """
 
-
 class ListRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
         """
 
-
 class ListVirtualGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
         """
 
-
 class ListVirtualNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualNodesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
         """
 
-
 class ListVirtualRoutersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualRoutersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
         """
 
-
 class ListVirtualServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
         """
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/paginator.pyi` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,136 +56,162 @@
     "ListTagsForResourcePaginator",
     "ListVirtualGatewaysPaginator",
     "ListVirtualNodesPaginator",
     "ListVirtualRoutersPaginator",
     "ListVirtualServicesPaginator",
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
 class ListGatewayRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
         """
 
+
 class ListMeshesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMeshesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
         """
 
+
 class ListRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
         """
 
+
 class ListVirtualGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
         """
 
+
 class ListVirtualNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualNodesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
         """
 
+
 class ListVirtualRoutersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualRoutersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
         """
 
+
 class ListVirtualServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
     """
 
     def paginate(
-        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        meshName: str,
+        meshOwner: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
         """
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/type_defs.py` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 
 __all__ = (
     "AwsCloudMapInstanceAttributeTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
     "DeleteVirtualNodeInputRequestTypeDef",
     "DeleteVirtualRouterInputRequestTypeDef",
     "DeleteVirtualServiceInputRequestTypeDef",
@@ -80,35 +79,44 @@
     "WeightedTargetTypeDef",
     "HealthCheckPolicyTypeDef",
     "HttpPathMatchTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
     "QueryParameterMatchTypeDef",
     "JsonFormatRefTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
+    "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
+    "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
+    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
+    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
+    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
     "PortMappingTypeDef",
     "MeshStatusTypeDef",
     "MeshServiceDiscoveryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
     "TcpRouteMatchTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
@@ -129,16 +137,16 @@
     "VirtualNodeStatusTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
     "ClientTlsCertificateTypeDef",
-    "TagResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "TagResourceInputRequestTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
@@ -149,22 +157,14 @@
     "HeaderMatchMethodTypeDef",
     "GrpcRouteActionTypeDef",
     "HttpRouteActionTypeDef",
     "TcpRouteActionTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
     "HttpQueryParameterTypeDef",
     "LoggingFormatTypeDef",
-    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    "ListRoutesInputListRoutesPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
     "ListenerTlsCertificateTypeDef",
@@ -303,25 +303,14 @@
     "TagRefTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredDeleteGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDeleteGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -809,24 +798,38 @@
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "meshName": str,
+        "virtualGatewayName": str,
+    },
+)
+_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
+    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -843,14 +846,22 @@
 
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
 
+ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMeshesInputRequestTypeDef = TypedDict(
     "ListMeshesInputRequestTypeDef",
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
@@ -865,14 +876,38 @@
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
     },
 )
 
+_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualRouterName": str,
+    },
+)
+_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRoutesInputListRoutesPaginateTypeDef(
+    _RequiredListRoutesInputListRoutesPaginateTypeDef,
+    _OptionalListRoutesInputListRoutesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -904,14 +939,36 @@
         "resourceOwner": str,
         "routeName": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
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
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -926,14 +983,37 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
+    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualGatewaysInputRequestTypeDef = TypedDict(
@@ -963,14 +1043,37 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
+_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
+    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -1000,14 +1103,37 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualNodeName": str,
     },
 )
 
+_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
+    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -1037,14 +1163,37 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
+_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
+    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1119,14 +1268,35 @@
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
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
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
@@ -1385,28 +1555,28 @@
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagRefTypeDef],
-    },
-)
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagRefTypeDef],
     },
 )
 
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
@@ -1494,15 +1664,15 @@
 )
 
 ListGatewayRoutesOutputTypeDef = TypedDict(
     "ListGatewayRoutesOutputTypeDef",
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
@@ -1616,235 +1786,65 @@
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
-_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualGatewayName": str,
-    },
-)
-_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
-    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-):
-    pass
-
-
-ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualRouterName": str,
-    },
-)
-_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRoutesInputListRoutesPaginateTypeDef(
-    _RequiredListRoutesInputListRoutesPaginateTypeDef,
-    _OptionalListRoutesInputListRoutesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
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
-_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
-    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
-    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
-    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
-    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-):
-    pass
-
-
 ListMeshesOutputTypeDef = TypedDict(
     "ListMeshesOutputTypeDef",
     {
         "meshes": List[MeshRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoutesOutputTypeDef = TypedDict(
     "ListRoutesOutputTypeDef",
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualNodesOutputTypeDef = TypedDict(
     "ListVirtualNodesOutputTypeDef",
     {
         "nextToken": str,
         "virtualNodes": List[VirtualNodeRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualRoutersOutputTypeDef = TypedDict(
     "ListVirtualRoutersOutputTypeDef",
     {
         "nextToken": str,
         "virtualRouters": List[VirtualRouterRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualServicesOutputTypeDef = TypedDict(
     "ListVirtualServicesOutputTypeDef",
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
@@ -2455,39 +2455,39 @@
     },
 )
 
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMeshOutputTypeDef = TypedDict(
     "DeleteMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMeshOutputTypeDef = TypedDict(
     "DescribeMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMeshOutputTypeDef = TypedDict(
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
@@ -2709,39 +2709,39 @@
     total=False,
 )
 
 CreateVirtualRouterOutputTypeDef = TypedDict(
     "CreateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualRouterOutputTypeDef = TypedDict(
     "DeleteVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualRouterOutputTypeDef = TypedDict(
     "DescribeVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualRouterOutputTypeDef = TypedDict(
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
@@ -2803,39 +2803,39 @@
     total=False,
 )
 
 CreateVirtualServiceOutputTypeDef = TypedDict(
     "CreateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualServiceOutputTypeDef = TypedDict(
     "DeleteVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualServiceOutputTypeDef = TypedDict(
     "DescribeVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualServiceOutputTypeDef = TypedDict(
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
@@ -3051,71 +3051,71 @@
     pass
 
 
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGatewayRouteOutputTypeDef = TypedDict(
     "DeleteGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGatewayRouteOutputTypeDef = TypedDict(
     "DescribeGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGatewayRouteOutputTypeDef = TypedDict(
     "UpdateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRouteOutputTypeDef = TypedDict(
     "CreateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRouteOutputTypeDef = TypedDict(
     "DeleteRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRouteOutputTypeDef = TypedDict(
     "DescribeRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRouteOutputTypeDef = TypedDict(
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
@@ -3249,66 +3249,66 @@
     },
 )
 
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualGatewayOutputTypeDef = TypedDict(
     "DeleteVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualGatewayOutputTypeDef = TypedDict(
     "DescribeVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualGatewayOutputTypeDef = TypedDict(
     "UpdateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVirtualNodeOutputTypeDef = TypedDict(
     "CreateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualNodeOutputTypeDef = TypedDict(
     "DeleteVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualNodeOutputTypeDef = TypedDict(
     "DescribeVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualNodeOutputTypeDef = TypedDict(
     "UpdateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh/type_defs.pyi` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AwsCloudMapInstanceAttributeTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
     "DeleteVirtualNodeInputRequestTypeDef",
     "DeleteVirtualRouterInputRequestTypeDef",
     "DeleteVirtualServiceInputRequestTypeDef",
@@ -79,35 +78,44 @@
     "WeightedTargetTypeDef",
     "HealthCheckPolicyTypeDef",
     "HttpPathMatchTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
     "QueryParameterMatchTypeDef",
     "JsonFormatRefTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
+    "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
+    "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
+    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
+    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
+    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
     "PortMappingTypeDef",
     "MeshStatusTypeDef",
     "MeshServiceDiscoveryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
     "TcpRouteMatchTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
@@ -128,16 +136,16 @@
     "VirtualNodeStatusTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
     "ClientTlsCertificateTypeDef",
-    "TagResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "TagResourceInputRequestTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
@@ -148,22 +156,14 @@
     "HeaderMatchMethodTypeDef",
     "GrpcRouteActionTypeDef",
     "HttpRouteActionTypeDef",
     "TcpRouteActionTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
     "HttpQueryParameterTypeDef",
     "LoggingFormatTypeDef",
-    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    "ListRoutesInputListRoutesPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
     "ListenerTlsCertificateTypeDef",
@@ -302,25 +302,14 @@
     "TagRefTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredDeleteGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDeleteGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -776,24 +765,36 @@
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "meshName": str,
+        "virtualGatewayName": str,
+    },
+)
+_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
+    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+):
+    pass
+
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -808,14 +809,22 @@
 )
 
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
+ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMeshesInputRequestTypeDef = TypedDict(
     "ListMeshesInputRequestTypeDef",
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
@@ -830,14 +839,36 @@
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
     },
 )
 
+_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualRouterName": str,
+    },
+)
+_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRoutesInputListRoutesPaginateTypeDef(
+    _RequiredListRoutesInputListRoutesPaginateTypeDef,
+    _OptionalListRoutesInputListRoutesPaginateTypeDef,
+):
+    pass
+
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -867,14 +898,34 @@
         "resourceOwner": str,
         "routeName": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
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
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -887,14 +938,35 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
+    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+):
+    pass
+
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualGatewaysInputRequestTypeDef = TypedDict(
@@ -922,14 +994,35 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
+_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
+    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+):
+    pass
+
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -957,14 +1050,35 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualNodeName": str,
     },
 )
 
+_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
+    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+):
+    pass
+
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -992,14 +1106,35 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
+_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
+    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+):
+    pass
+
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1072,14 +1207,35 @@
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
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
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
@@ -1330,28 +1486,28 @@
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagRefTypeDef],
-    },
-)
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagRefTypeDef],
     },
 )
 
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
@@ -1435,15 +1591,15 @@
 )
 
 ListGatewayRoutesOutputTypeDef = TypedDict(
     "ListGatewayRoutesOutputTypeDef",
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
@@ -1553,221 +1709,65 @@
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
-_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualGatewayName": str,
-    },
-)
-_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
-    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-):
-    pass
-
-ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualRouterName": str,
-    },
-)
-_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRoutesInputListRoutesPaginateTypeDef(
-    _RequiredListRoutesInputListRoutesPaginateTypeDef,
-    _OptionalListRoutesInputListRoutesPaginateTypeDef,
-):
-    pass
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
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
-_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
-    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-):
-    pass
-
-_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
-    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-):
-    pass
-
-_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
-    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-):
-    pass
-
-_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
-    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-):
-    pass
-
 ListMeshesOutputTypeDef = TypedDict(
     "ListMeshesOutputTypeDef",
     {
         "meshes": List[MeshRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoutesOutputTypeDef = TypedDict(
     "ListRoutesOutputTypeDef",
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualNodesOutputTypeDef = TypedDict(
     "ListVirtualNodesOutputTypeDef",
     {
         "nextToken": str,
         "virtualNodes": List[VirtualNodeRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualRoutersOutputTypeDef = TypedDict(
     "ListVirtualRoutersOutputTypeDef",
     {
         "nextToken": str,
         "virtualRouters": List[VirtualRouterRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualServicesOutputTypeDef = TypedDict(
     "ListVirtualServicesOutputTypeDef",
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
@@ -2344,39 +2344,39 @@
     },
 )
 
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMeshOutputTypeDef = TypedDict(
     "DeleteMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMeshOutputTypeDef = TypedDict(
     "DescribeMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMeshOutputTypeDef = TypedDict(
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
@@ -2582,39 +2582,39 @@
     total=False,
 )
 
 CreateVirtualRouterOutputTypeDef = TypedDict(
     "CreateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualRouterOutputTypeDef = TypedDict(
     "DeleteVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualRouterOutputTypeDef = TypedDict(
     "DescribeVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualRouterOutputTypeDef = TypedDict(
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
@@ -2672,39 +2672,39 @@
     total=False,
 )
 
 CreateVirtualServiceOutputTypeDef = TypedDict(
     "CreateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualServiceOutputTypeDef = TypedDict(
     "DeleteVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualServiceOutputTypeDef = TypedDict(
     "DescribeVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualServiceOutputTypeDef = TypedDict(
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
@@ -2908,71 +2908,71 @@
 ):
     pass
 
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteGatewayRouteOutputTypeDef = TypedDict(
     "DeleteGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGatewayRouteOutputTypeDef = TypedDict(
     "DescribeGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGatewayRouteOutputTypeDef = TypedDict(
     "UpdateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRouteOutputTypeDef = TypedDict(
     "CreateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRouteOutputTypeDef = TypedDict(
     "DeleteRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRouteOutputTypeDef = TypedDict(
     "DescribeRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRouteOutputTypeDef = TypedDict(
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
@@ -3098,66 +3098,66 @@
     },
 )
 
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualGatewayOutputTypeDef = TypedDict(
     "DeleteVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualGatewayOutputTypeDef = TypedDict(
     "DescribeVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualGatewayOutputTypeDef = TypedDict(
     "UpdateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVirtualNodeOutputTypeDef = TypedDict(
     "CreateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVirtualNodeOutputTypeDef = TypedDict(
     "DeleteVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVirtualNodeOutputTypeDef = TypedDict(
     "DescribeVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVirtualNodeOutputTypeDef = TypedDict(
     "UpdateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/PKG-INFO` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.AppMesh 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AppMesh 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
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
 
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appmesh?color=blue)](https://pypistats.org/packages/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,15 +375,14 @@
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
-    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
@@ -406,35 +406,44 @@
     WeightedTargetTypeDef,
     HealthCheckPolicyTypeDef,
     HttpPathMatchTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
     QueryParameterMatchTypeDef,
     JsonFormatRefTypeDef,
-    PaginatorConfigTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
     ListenerTlsAcmCertificateTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
     PortMappingTypeDef,
     MeshStatusTypeDef,
     MeshServiceDiscoveryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
     TcpRouteMatchTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
@@ -455,16 +464,16 @@
     VirtualNodeStatusTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
     ClientTlsCertificateTypeDef,
-    TagResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TagResourceInputRequestTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
@@ -475,22 +484,14 @@
     HeaderMatchMethodTypeDef,
     GrpcRouteActionTypeDef,
     HttpRouteActionTypeDef,
     TcpRouteActionTypeDef,
     HttpGatewayRouteRewriteTypeDef,
     HttpQueryParameterTypeDef,
     LoggingFormatTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     ListenerTlsCertificateTypeDef,
@@ -610,42 +611,42 @@
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

### Comparing `mypy-boto3-appmesh-1.26.0.post1/mypy_boto3_appmesh.egg-info/SOURCES.txt` & `mypy-boto3-appmesh-1.27.0/mypy_boto3_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.26.0.post1/setup.py` & `mypy-boto3-appmesh-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
 Setup script for mypy-boto3-appmesh.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appmesh",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppMesh 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.AppMesh 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_appmesh": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_appmesh": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/",
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


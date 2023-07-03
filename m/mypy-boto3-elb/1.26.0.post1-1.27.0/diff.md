# Comparing `tmp/mypy-boto3-elb-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-elb-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elb-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:24 2022, max compression
+gzip compressed data, was "mypy-boto3-elb-1.27.0.tar", last modified: Mon Jul  3 19:50:44 2023, max compression
```

## Comparing `mypy-boto3-elb-1.26.0.post1.tar` & `mypy-boto3-elb-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:24.456827 mypy-boto3-elb-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16979 2022-11-01 21:43:24.448827 mypy-boto3-elb-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15537 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:24.448827 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24944 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    24903 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8084 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8082 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    24555 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    24532 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-11-01 21:34:22.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:24.448827 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16979 2022-11-01 21:43:24.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-01 21:43:24.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:24.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:24.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:24.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:24.000000 mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:24.456827 mypy-boto3-elb-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-11-01 21:34:21.000000 mypy-boto3-elb-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:44.839221 mypy-boto3-elb-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-07-03 19:50:44.831221 mypy-boto3-elb-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:44.831221 mypy-boto3-elb-1.27.0/mypy_boto3_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24903 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-03 19:37:22.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-07-03 19:37:23.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-07-03 19:37:22.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:44.831221 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-07-03 19:50:44.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:44.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:44.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:44.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:44.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:44.000000 mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:44.839221 mypy-boto3-elb-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:37:21.000000 mypy-boto3-elb-1.27.0/setup.py
```

### Comparing `mypy-boto3-elb-1.26.0.post1/LICENSE` & `mypy-boto3-elb-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-elb-1.26.0.post1/PKG-INFO` & `mypy-boto3-elb-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
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
 
 <a id="mypy-boto3-elb"></a>
 
 # mypy-boto3-elb
 
 [![PyPI - mypy-boto3-elb](https://img.shields.io/pypi/v/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elb?color=blue)](https://pypistats.org/packages/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,75 +359,75 @@
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
     TagTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
     ConnectionDrainingTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
+    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
     SourceSecurityGroupTypeDef,
+    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
+    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
-    CreateAccessPointOutputTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
     ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
     DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
     RegisterEndPointsOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
     PolicyDescriptionTypeDef,
@@ -450,42 +451,42 @@
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

### Comparing `mypy-boto3-elb-1.26.0.post1/README.md` & `mypy-boto3-elb-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elb"></a>
 
 # mypy-boto3-elb
 
 [![PyPI - mypy-boto3-elb](https://img.shields.io/pypi/v/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elb?color=blue)](https://pypistats.org/packages/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,75 +327,75 @@
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
     TagTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
     ConnectionDrainingTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
+    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
     SourceSecurityGroupTypeDef,
+    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
+    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
-    CreateAccessPointOutputTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
     ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
     DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
     RegisterEndPointsOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
     PolicyDescriptionTypeDef,
@@ -419,42 +419,42 @@
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

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/__init__.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/__init__.pyi` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/__main__.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancing 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancing 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
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

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/client.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/client.pyi` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/literals.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,23 +51,25 @@
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
@@ -77,30 +79,35 @@
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
@@ -126,14 +133,15 @@
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
@@ -178,51 +186,57 @@
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
@@ -235,14 +249,15 @@
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
@@ -254,28 +269,35 @@
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
@@ -284,14 +306,15 @@
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
@@ -302,55 +325,64 @@
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
@@ -377,21 +409,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/literals.pyi` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,25 @@
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
@@ -75,30 +77,35 @@
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
@@ -124,14 +131,15 @@
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
@@ -176,51 +184,57 @@
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
@@ -233,14 +247,15 @@
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
@@ -252,28 +267,35 @@
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
@@ -282,14 +304,15 @@
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
@@ -300,55 +323,64 @@
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
@@ -375,21 +407,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/paginator.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -65,13 +65,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/paginator.pyi` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeLoadBalancersPaginator(Paginator):
@@ -61,13 +61,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
         self,
         *,
         LoadBalancerNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccessPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/paginators/#describeloadbalancerspaginator)
         """
```

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/type_defs.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,75 +20,75 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddAvailabilityZonesOutputTypeDef",
     "TagTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
     "ConnectionDrainingTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
+    "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
     "SourceSecurityGroupTypeDef",
+    "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
+    "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
+    "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
-    "AddAvailabilityZonesOutputTypeDef",
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    "CreateAccessPointOutputTypeDef",
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    "RemoveAvailabilityZonesOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
     "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
     "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
     "RegisterEndPointsOutputTypeDef",
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
     "PolicyDescriptionTypeDef",
@@ -129,22 +129,19 @@
     "AddAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddAvailabilityZonesOutputTypeDef = TypedDict(
+    "AddAvailabilityZonesOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
@@ -185,22 +182,38 @@
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
+ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttachLoadBalancerToSubnetsInputRequestTypeDef = TypedDict(
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
+AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BackendServerDescriptionTypeDef = TypedDict(
     "BackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
     total=False,
@@ -263,14 +276,22 @@
 )
 
 
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
 
+CreateAccessPointOutputTypeDef = TypedDict(
+    "CreateAccessPointOutputTypeDef",
+    {
+        "DNSName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateAppCookieStickinessPolicyInputRequestTypeDef = TypedDict(
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "CookieName": str,
     },
@@ -342,34 +363,41 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "LoadBalancerNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccessPointsInputRequestTypeDef = TypedDict(
     "DescribeAccessPointsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
@@ -439,14 +467,22 @@
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
+DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LBCookieStickinessPolicyTypeDef = TypedDict(
     "LBCookieStickinessPolicyTypeDef",
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
@@ -457,14 +493,24 @@
     {
         "OwnerAlias": str,
         "GroupName": str,
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
 PolicyAttributeDescriptionTypeDef = TypedDict(
     "PolicyAttributeDescriptionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -486,22 +532,41 @@
     "RemoveAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
+RemoveAvailabilityZonesOutputTypeDef = TypedDict(
+    "RemoveAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagKeyOnlyTypeDef = TypedDict(
     "TagKeyOnlyTypeDef",
     {
         "Key": str,
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
 SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = TypedDict(
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "SSLCertificateId": str,
     },
@@ -521,62 +586,14 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
-AddAvailabilityZonesOutputTypeDef = TypedDict(
-    "AddAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAccessPointOutputTypeDef = TypedDict(
-    "CreateAccessPointOutputTypeDef",
-    {
-        "DNSName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveAvailabilityZonesOutputTypeDef = TypedDict(
-    "RemoveAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -598,15 +615,15 @@
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -693,15 +710,15 @@
     },
 )
 
 DeregisterEndPointsOutputTypeDef = TypedDict(
     "DeregisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -731,41 +748,24 @@
     },
 )
 
 RegisterEndPointsOutputTypeDef = TypedDict(
     "RegisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
@@ -834,15 +834,15 @@
     pass
 
 
 DescribeEndPointStateOutputTypeDef = TypedDict(
     "DescribeEndPointStateOutputTypeDef",
     {
         "InstanceStates": List[InstanceStateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PoliciesTypeDef = TypedDict(
     "PoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
@@ -880,23 +880,23 @@
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -905,15 +905,15 @@
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
@@ -936,27 +936,27 @@
     total=False,
 )
 
 DescribeLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     {
         "PolicyDescriptions": List[PolicyDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerPolicyTypesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/type_defs.pyi` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,75 +19,75 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogTypeDef",
     "AddAvailabilityZonesInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddAvailabilityZonesOutputTypeDef",
     "TagTypeDef",
     "AdditionalAttributeTypeDef",
     "AppCookieStickinessPolicyTypeDef",
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
     "BackendServerDescriptionTypeDef",
     "HealthCheckTypeDef",
     "ConnectionDrainingTypeDef",
     "ConnectionSettingsTypeDef",
     "ListenerTypeDef",
+    "CreateAccessPointOutputTypeDef",
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     "CreateLBCookieStickinessPolicyInputRequestTypeDef",
     "PolicyAttributeTypeDef",
     "CrossZoneLoadBalancingTypeDef",
     "DeleteAccessPointInputRequestTypeDef",
     "DeleteLoadBalancerListenerInputRequestTypeDef",
     "DeleteLoadBalancerPolicyInputRequestTypeDef",
     "InstanceTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     "DescribeAccessPointsInputRequestTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
     "WaiterConfigTypeDef",
     "InstanceStateTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "DescribeLoadBalancerPoliciesInputRequestTypeDef",
     "DescribeLoadBalancerPolicyTypesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
     "LBCookieStickinessPolicyTypeDef",
     "SourceSecurityGroupTypeDef",
+    "PaginatorConfigTypeDef",
     "PolicyAttributeDescriptionTypeDef",
     "PolicyAttributeTypeDescriptionTypeDef",
     "RemoveAvailabilityZonesInputRequestTypeDef",
+    "RemoveAvailabilityZonesOutputTypeDef",
     "TagKeyOnlyTypeDef",
+    "ResponseMetadataTypeDef",
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     "SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef",
     "SetLoadBalancerPoliciesOfListenerInputRequestTypeDef",
-    "AddAvailabilityZonesOutputTypeDef",
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    "CreateAccessPointOutputTypeDef",
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    "RemoveAvailabilityZonesOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
     "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
     "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
     "RegisterEndPointsOutputTypeDef",
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef",
     "DescribeEndPointStateInputInstanceInServiceWaitTypeDef",
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
     "PolicyDescriptionTypeDef",
@@ -126,22 +126,19 @@
     "AddAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddAvailabilityZonesOutputTypeDef = TypedDict(
+    "AddAvailabilityZonesOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
@@ -180,22 +177,38 @@
     "ApplySecurityGroupsToLoadBalancerInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
+ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
+    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttachLoadBalancerToSubnetsInputRequestTypeDef = TypedDict(
     "AttachLoadBalancerToSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
+AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
+    "AttachLoadBalancerToSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BackendServerDescriptionTypeDef = TypedDict(
     "BackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
     total=False,
@@ -254,14 +267,22 @@
     },
     total=False,
 )
 
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
+CreateAccessPointOutputTypeDef = TypedDict(
+    "CreateAccessPointOutputTypeDef",
+    {
+        "DNSName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateAppCookieStickinessPolicyInputRequestTypeDef = TypedDict(
     "CreateAppCookieStickinessPolicyInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "PolicyName": str,
         "CookieName": str,
     },
@@ -331,34 +352,41 @@
     "InstanceTypeDef",
     {
         "InstanceId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "LoadBalancerNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccessPointsInputRequestTypeDef = TypedDict(
     "DescribeAccessPointsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
@@ -428,14 +456,22 @@
     "DetachLoadBalancerFromSubnetsInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "Subnets": Sequence[str],
     },
 )
 
+DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
+    "DetachLoadBalancerFromSubnetsOutputTypeDef",
+    {
+        "Subnets": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LBCookieStickinessPolicyTypeDef = TypedDict(
     "LBCookieStickinessPolicyTypeDef",
     {
         "PolicyName": str,
         "CookieExpirationPeriod": int,
     },
     total=False,
@@ -446,14 +482,24 @@
     {
         "OwnerAlias": str,
         "GroupName": str,
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
 PolicyAttributeDescriptionTypeDef = TypedDict(
     "PolicyAttributeDescriptionTypeDef",
     {
         "AttributeName": str,
         "AttributeValue": str,
     },
     total=False,
@@ -475,22 +521,41 @@
     "RemoveAvailabilityZonesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "AvailabilityZones": Sequence[str],
     },
 )
 
+RemoveAvailabilityZonesOutputTypeDef = TypedDict(
+    "RemoveAvailabilityZonesOutputTypeDef",
+    {
+        "AvailabilityZones": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagKeyOnlyTypeDef = TypedDict(
     "TagKeyOnlyTypeDef",
     {
         "Key": str,
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
 SetLoadBalancerListenerSSLCertificateInputRequestTypeDef = TypedDict(
     "SetLoadBalancerListenerSSLCertificateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "SSLCertificateId": str,
     },
@@ -510,62 +575,14 @@
     {
         "LoadBalancerName": str,
         "LoadBalancerPort": int,
         "PolicyNames": Sequence[str],
     },
 )
 
-AddAvailabilityZonesOutputTypeDef = TypedDict(
-    "AddAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ApplySecurityGroupsToLoadBalancerOutputTypeDef = TypedDict(
-    "ApplySecurityGroupsToLoadBalancerOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachLoadBalancerToSubnetsOutputTypeDef = TypedDict(
-    "AttachLoadBalancerToSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAccessPointOutputTypeDef = TypedDict(
-    "CreateAccessPointOutputTypeDef",
-    {
-        "DNSName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachLoadBalancerFromSubnetsOutputTypeDef = TypedDict(
-    "DetachLoadBalancerFromSubnetsOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveAvailabilityZonesOutputTypeDef = TypedDict(
-    "RemoveAvailabilityZonesOutputTypeDef",
-    {
-        "AvailabilityZones": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "LoadBalancerNames": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -587,15 +604,15 @@
     },
 )
 
 ConfigureHealthCheckOutputTypeDef = TypedDict(
     "ConfigureHealthCheckOutputTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAccessPointInputRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -678,15 +695,15 @@
     },
 )
 
 DeregisterEndPointsOutputTypeDef = TypedDict(
     "DeregisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEndPointStateInputRequestTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -714,41 +731,24 @@
     },
 )
 
 RegisterEndPointsOutputTypeDef = TypedDict(
     "RegisterEndPointsOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeAccountLimitsOutputTypeDef = TypedDict(
     "DescribeAccountLimitsOutputTypeDef",
     {
         "Limits": List[LimitTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef",
     {
         "LoadBalancerName": str,
@@ -811,15 +811,15 @@
 ):
     pass
 
 DescribeEndPointStateOutputTypeDef = TypedDict(
     "DescribeEndPointStateOutputTypeDef",
     {
         "InstanceStates": List[InstanceStateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PoliciesTypeDef = TypedDict(
     "PoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": List[AppCookieStickinessPolicyTypeDef],
@@ -857,23 +857,23 @@
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
@@ -882,15 +882,15 @@
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
@@ -913,27 +913,27 @@
     total=False,
 )
 
 DescribeLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     {
         "PolicyDescriptions": List[PolicyDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancerPolicyTypesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     {
         "PolicyTypeDescriptions": List[PolicyTypeDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAccessPointsOutputTypeDef = TypedDict(
     "DescribeAccessPointsOutputTypeDef",
     {
         "LoadBalancerDescriptions": List[LoadBalancerDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/waiter.py` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb/waiter.pyi` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/PKG-INFO` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ElasticLoadBalancing 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticLoadBalancing 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/
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
 
 <a id="mypy-boto3-elb"></a>
 
 # mypy-boto3-elb
 
 [![PyPI - mypy-boto3-elb](https://img.shields.io/pypi/v/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elb.svg?color=blue)](https://pypi.org/project/mypy-boto3-elb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elb?color=blue)](https://pypistats.org/packages/mypy-boto3-elb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancing 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
+[boto3.ElasticLoadBalancing 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing)
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
 [mypy-boto3-elb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,75 +359,75 @@
 `mypy_boto3_elb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_elb.type_defs import (
     AccessLogTypeDef,
     AddAvailabilityZonesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddAvailabilityZonesOutputTypeDef,
     TagTypeDef,
     AdditionalAttributeTypeDef,
     AppCookieStickinessPolicyTypeDef,
     ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
+    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
     AttachLoadBalancerToSubnetsInputRequestTypeDef,
+    AttachLoadBalancerToSubnetsOutputTypeDef,
     BackendServerDescriptionTypeDef,
     HealthCheckTypeDef,
     ConnectionDrainingTypeDef,
     ConnectionSettingsTypeDef,
     ListenerTypeDef,
+    CreateAccessPointOutputTypeDef,
     CreateAppCookieStickinessPolicyInputRequestTypeDef,
     CreateLBCookieStickinessPolicyInputRequestTypeDef,
     PolicyAttributeTypeDef,
     CrossZoneLoadBalancingTypeDef,
     DeleteAccessPointInputRequestTypeDef,
     DeleteLoadBalancerListenerInputRequestTypeDef,
     DeleteLoadBalancerPolicyInputRequestTypeDef,
     InstanceTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
     DescribeAccessPointsInputRequestTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
     WaiterConfigTypeDef,
     InstanceStateTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     DescribeLoadBalancerPoliciesInputRequestTypeDef,
     DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DetachLoadBalancerFromSubnetsInputRequestTypeDef,
+    DetachLoadBalancerFromSubnetsOutputTypeDef,
     LBCookieStickinessPolicyTypeDef,
     SourceSecurityGroupTypeDef,
+    PaginatorConfigTypeDef,
     PolicyAttributeDescriptionTypeDef,
     PolicyAttributeTypeDescriptionTypeDef,
     RemoveAvailabilityZonesInputRequestTypeDef,
+    RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
+    ResponseMetadataTypeDef,
     SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
     SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
     SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
-    CreateAccessPointOutputTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     ConfigureHealthCheckInputRequestTypeDef,
     ConfigureHealthCheckOutputTypeDef,
     CreateAccessPointInputRequestTypeDef,
     CreateLoadBalancerListenerInputRequestTypeDef,
     ListenerDescriptionTypeDef,
     CreateLoadBalancerPolicyInputRequestTypeDef,
     LoadBalancerAttributesTypeDef,
     DeregisterEndPointsInputRequestTypeDef,
     DeregisterEndPointsOutputTypeDef,
     DescribeEndPointStateInputRequestTypeDef,
     RegisterEndPointsInputRequestTypeDef,
     RegisterEndPointsOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
     DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
     DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
     DescribeEndPointStateOutputTypeDef,
     PoliciesTypeDef,
     PolicyDescriptionTypeDef,
@@ -450,42 +451,42 @@
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

### Comparing `mypy-boto3-elb-1.26.0.post1/mypy_boto3_elb.egg-info/SOURCES.txt` & `mypy-boto3-elb-1.27.0/mypy_boto3_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elb-1.26.0.post1/setup.py` & `mypy-boto3-elb-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-elb.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elb",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancing 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ElasticLoadBalancing 1.27.0 service generated with"
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
     keywords="boto3 elb type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_elb": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_elb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elb/",
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


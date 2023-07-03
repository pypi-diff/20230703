# Comparing `tmp/mypy-boto3-elbv2-1.26.63.tar.gz` & `tmp/mypy-boto3-elbv2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elbv2-1.26.63.tar", last modified: Thu Feb  2 20:49:28 2023, max compression
+gzip compressed data, was "mypy-boto3-elbv2-1.27.0.tar", last modified: Mon Jul  3 19:50:44 2023, max compression
```

## Comparing `mypy-boto3-elbv2-1.26.63.tar` & `mypy-boto3-elbv2-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:28.134371 mypy-boto3-elbv2-1.26.63/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-02-02 20:49:28.134371 mypy-boto3-elbv2-1.26.63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18409 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:28.130371 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-02-02 20:47:47.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-02-02 20:47:47.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-02-02 20:47:47.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38563 2023-02-02 20:47:47.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 20:49:28.130371 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-02-02 20:49:27.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-02 20:49:27.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:49:27.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 20:49:27.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 20:49:27.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-02 20:49:27.000000 mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 20:49:28.134371 mypy-boto3-elbv2-1.26.63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-02-02 20:47:46.000000 mypy-boto3-elbv2-1.26.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:44.855222 mypy-boto3-elbv2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-03 19:50:44.855222 mypy-boto3-elbv2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:44.851221 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33888 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33835 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-03 19:37:25.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-07-03 19:37:25.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-07-03 19:37:25.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:44.855222 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-03 19:50:44.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-03 19:50:44.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:44.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:44.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:44.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:50:44.000000 mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:44.855222 mypy-boto3-elbv2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-03 19:37:24.000000 mypy-boto3-elbv2-1.27.0/setup.py
```

### Comparing `mypy-boto3-elbv2-1.26.63/LICENSE` & `mypy-boto3-elbv2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-elbv2-1.26.63/PKG-INFO` & `mypy-boto3-elbv2-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.26.63
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.26.63 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-elbv2"></a>
 
 # mypy-boto3-elbv2
 
 [![PyPI - mypy-boto3-elbv2](https://img.shields.io/pypi/v/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elbv2?color=blue)](https://pypistats.org/packages/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,79 +409,79 @@
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigTypeDef,
     AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
     CertificateTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerAttributeTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
     TargetGroupAttributeTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
     HostHeaderConditionConfigTypeDef,
     HttpHeaderConditionConfigTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
     LoadBalancerStateTypeDef,
+    PaginatorConfigTypeDef,
     PathPatternConditionConfigTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
+    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    SetIpAddressTypeOutputTypeDef,
-    SetSecurityGroupsOutputTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
     TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
@@ -529,42 +529,42 @@
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

### Comparing `mypy-boto3-elbv2-1.26.63/README.md` & `mypy-boto3-elbv2-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elbv2"></a>
 
 # mypy-boto3-elbv2
 
 [![PyPI - mypy-boto3-elbv2](https://img.shields.io/pypi/v/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elbv2?color=blue)](https://pypistats.org/packages/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,79 +377,79 @@
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigTypeDef,
     AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
     CertificateTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerAttributeTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
     TargetGroupAttributeTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
     HostHeaderConditionConfigTypeDef,
     HttpHeaderConditionConfigTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
     LoadBalancerStateTypeDef,
+    PaginatorConfigTypeDef,
     PathPatternConditionConfigTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
+    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    SetIpAddressTypeOutputTypeDef,
-    SetSecurityGroupsOutputTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
     TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
@@ -497,42 +497,42 @@
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

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/__init__.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/__init__.pyi` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/__main__.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.26.63\nVersion:        "
-        " 1.26.63\nBuilder version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.63")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/client.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/client.pyi` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/literals.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,14 +243,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -259,14 +262,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -302,14 +306,15 @@
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
@@ -328,16 +333,19 @@
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
@@ -417,18 +425,21 @@
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

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/literals.pyi` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,14 +241,15 @@
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
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -257,14 +260,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -300,14 +304,15 @@
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
@@ -326,16 +331,19 @@
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
@@ -415,18 +423,21 @@
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

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/paginator.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,30 +71,30 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
         """
 
 
 class DescribeListenerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeListenerCertificatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
         """
 
 
@@ -105,15 +105,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeListenersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenerspaginator)
         """
 
 
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
 
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describerulespaginator)
         """
 
 
@@ -162,15 +162,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describesslpoliciespaginator)
         """
 
 
@@ -182,13 +182,13 @@
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/paginator.pyi` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -68,29 +68,29 @@
 class DescribeAccountLimitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeAccountLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeListenerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeListenerCertificatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListenerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenercertificatespaginator)
         """
 
 class DescribeListenersPaginator(Paginator):
@@ -100,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         ListenerArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeListenersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describelistenerspaginator)
         """
 
 class DescribeLoadBalancersPaginator(Paginator):
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         LoadBalancerArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLoadBalancersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describeloadbalancerspaginator)
         """
 
 class DescribeRulesPaginator(Paginator):
@@ -136,15 +136,15 @@
     """
 
     def paginate(
         self,
         *,
         ListenerArn: str = ...,
         RuleArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describerulespaginator)
         """
 
 class DescribeSSLPoliciesPaginator(Paginator):
@@ -154,15 +154,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         LoadBalancerType: LoadBalancerTypeEnumType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSSLPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeSSLPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describesslpoliciespaginator)
         """
 
 class DescribeTargetGroupsPaginator(Paginator):
@@ -173,13 +173,13 @@
 
     def paginate(
         self,
         *,
         LoadBalancerArn: str = ...,
         TargetGroupArns: Sequence[str] = ...,
         Names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTargetGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2.Paginator.DescribeTargetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/paginators/#describetargetgroupspaginator)
         """
```

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/type_defs.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,86 +32,85 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
     "CertificateTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
     "DeleteRuleInputRequestTypeDef",
     "DeleteTargetGroupInputRequestTypeDef",
     "TargetDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
+    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerAttributeTypeDef",
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     "TargetGroupAttributeTypeDef",
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
     "HostHeaderConditionConfigTypeDef",
     "HttpHeaderConditionConfigTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
     "LoadBalancerStateTypeDef",
+    "PaginatorConfigTypeDef",
     "PathPatternConditionConfigTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
+    "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
+    "SetSecurityGroupsOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
-    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
-    "SetIpAddressTypeOutputTypeDef",
-    "SetSecurityGroupsOutputTypeDef",
+    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
     "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
@@ -167,21 +166,19 @@
         "SessionTimeout": int,
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
-
 class AuthenticateCognitoActionConfigTypeDef(
     _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
 ):
     pass
 
-
 _RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateOidcActionConfigTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
@@ -198,21 +195,19 @@
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
-
 class AuthenticateOidcActionConfigTypeDef(
     _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
-
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
     },
 )
 _OptionalFixedResponseActionConfigTypeDef = TypedDict(
@@ -220,21 +215,19 @@
     {
         "MessageBody": str,
         "ContentType": str,
     },
     total=False,
 )
 
-
 class FixedResponseActionConfigTypeDef(
     _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
 ):
     pass
 
-
 _RequiredRedirectActionConfigTypeDef = TypedDict(
     "_RequiredRedirectActionConfigTypeDef",
     {
         "StatusCode": RedirectActionStatusCodeEnumType,
     },
 )
 _OptionalRedirectActionConfigTypeDef = TypedDict(
@@ -245,60 +238,45 @@
         "Host": str,
         "Path": str,
         "Query": str,
     },
     total=False,
 )
 
-
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
-
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
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
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 LoadBalancerAddressTypeDef = TypedDict(
     "LoadBalancerAddressTypeDef",
     {
         "IpAddress": str,
         "AllocationId": str,
         "PrivateIPv4Address": str,
         "IPv6Address": str,
@@ -374,27 +352,23 @@
     {
         "Port": int,
         "AvailabilityZone": str,
     },
     total=False,
 )
 
-
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -409,14 +383,34 @@
     {
         "Name": str,
         "Max": str,
     },
     total=False,
 )
 
+_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
+    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -424,21 +418,29 @@
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
+DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "ListenerArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeListenersInputRequestTypeDef = TypedDict(
     "DescribeListenersInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "Marker": str,
@@ -459,14 +461,24 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -479,25 +491,45 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+        "RuleArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRulesInputRequestTypeDef = TypedDict(
     "DescribeRulesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "RuleArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "LoadBalancerType": LoadBalancerTypeEnumType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSSLPoliciesInputRequestTypeDef = TypedDict(
     "DescribeSSLPoliciesInputRequestTypeDef",
     {
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
         "LoadBalancerType": LoadBalancerTypeEnumType,
@@ -524,14 +556,25 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "TargetGroupArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeTargetGroupsInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "TargetGroupArns": Sequence[str],
         "Names": Sequence[str],
         "Marker": str,
@@ -588,14 +631,24 @@
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
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
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -613,14 +666,25 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
     },
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
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -638,22 +702,38 @@
     "SetIpAddressTypeInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "IpAddressType": IpAddressTypeType,
     },
 )
 
+SetIpAddressTypeOutputTypeDef = TypedDict(
+    "SetIpAddressTypeOutputTypeDef",
+    {
+        "IpAddressType": IpAddressTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetSecurityGroupsInputRequestTypeDef = TypedDict(
     "SetSecurityGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
+SetSecurityGroupsOutputTypeDef = TypedDict(
+    "SetSecurityGroupsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -664,52 +744,36 @@
     "AddListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
-RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
-    "RemoveListenerCertificatesInputRequestTypeDef",
-    {
-        "ListenerArn": str,
-        "Certificates": Sequence[CertificateTypeDef],
-    },
-)
-
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SetIpAddressTypeOutputTypeDef = TypedDict(
-    "SetIpAddressTypeOutputTypeDef",
-    {
-        "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetSecurityGroupsOutputTypeDef = TypedDict(
-    "SetSecurityGroupsOutputTypeDef",
+RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
+    "RemoveListenerCertificatesInputRequestTypeDef",
     {
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ListenerArn": str,
+        "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
@@ -765,21 +829,19 @@
         "Type": LoadBalancerTypeEnumType,
         "IpAddressType": IpAddressTypeType,
         "CustomerOwnedIpv4Pool": str,
     },
     total=False,
 )
 
-
 class CreateLoadBalancerInputRequestTypeDef(
     _RequiredCreateLoadBalancerInputRequestTypeDef, _OptionalCreateLoadBalancerInputRequestTypeDef
 ):
     pass
 
-
 _RequiredSetSubnetsInputRequestTypeDef = TypedDict(
     "_RequiredSetSubnetsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 _OptionalSetSubnetsInputRequestTypeDef = TypedDict(
@@ -788,21 +850,19 @@
         "Subnets": Sequence[str],
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
         "IpAddressType": IpAddressTypeType,
     },
     total=False,
 )
 
-
 class SetSubnetsInputRequestTypeDef(
     _RequiredSetSubnetsInputRequestTypeDef, _OptionalSetSubnetsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTargetGroupInputRequestTypeDef = TypedDict(
@@ -824,21 +884,19 @@
         "TargetType": TargetTypeEnumType,
         "Tags": Sequence[TagTypeDef],
         "IpAddressType": TargetGroupIpAddressTypeEnumType,
     },
     total=False,
 )
 
-
 class CreateTargetGroupInputRequestTypeDef(
     _RequiredCreateTargetGroupInputRequestTypeDef, _OptionalCreateTargetGroupInputRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredModifyTargetGroupInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalModifyTargetGroupInputRequestTypeDef = TypedDict(
@@ -853,21 +911,19 @@
         "HealthyThresholdCount": int,
         "UnhealthyThresholdCount": int,
         "Matcher": MatcherTypeDef,
     },
     total=False,
 )
 
-
 class ModifyTargetGroupInputRequestTypeDef(
     _RequiredModifyTargetGroupInputRequestTypeDef, _OptionalModifyTargetGroupInputRequestTypeDef
 ):
     pass
 
-
 TargetGroupTypeDef = TypedDict(
     "TargetGroupTypeDef",
     {
         "TargetGroupArn": str,
         "TargetGroupName": str,
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -907,125 +963,42 @@
     "_OptionalDescribeTargetHealthInputRequestTypeDef",
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
     total=False,
 )
 
-
 class DescribeTargetHealthInputRequestTypeDef(
     _RequiredDescribeTargetHealthInputRequestTypeDef,
     _OptionalDescribeTargetHealthInputRequestTypeDef,
 ):
     pass
 
-
 RegisterTargetsInputRequestTypeDef = TypedDict(
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
-    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-):
-    pass
-
-
-DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "ListenerArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-        "RuleArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "LoadBalancerType": LoadBalancerTypeEnumType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "TargetGroupArns": Sequence[str],
-        "Names": Sequence[str],
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
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1033,15 +1006,15 @@
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
         "LoadBalancerArns": Sequence[str],
@@ -1088,22 +1061,20 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTargetHealthInputTargetDeregisteredWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
@@ -1111,27 +1082,25 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTargetHealthInputTargetInServiceWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef,
 ):
     pass
 
-
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
@@ -1139,15 +1108,15 @@
     },
 )
 
 ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
@@ -1181,15 +1150,15 @@
     total=False,
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1210,49 +1179,49 @@
 )
 
 SetSubnetsOutputTypeDef = TypedDict(
     "SetSubnetsOutputTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSSLPoliciesOutputTypeDef = TypedDict(
     "DescribeSSLPoliciesOutputTypeDef",
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTargetGroupOutputTypeDef = TypedDict(
     "CreateTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTargetGroupsOutputTypeDef = TypedDict(
     "DescribeTargetGroupsOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyTargetGroupOutputTypeDef = TypedDict(
     "ModifyTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
@@ -1268,19 +1237,17 @@
         "RedirectConfig": RedirectActionConfigTypeDef,
         "FixedResponseConfig": FixedResponseActionConfigTypeDef,
         "ForwardConfig": ForwardActionConfigTypeDef,
     },
     total=False,
 )
 
-
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
-
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1292,32 +1259,32 @@
     total=False,
 )
 
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoadBalancerOutputTypeDef = TypedDict(
     "CreateLoadBalancerOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersOutputTypeDef = TypedDict(
     "DescribeLoadBalancersOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1333,21 +1300,19 @@
         "Certificates": Sequence[CertificateTypeDef],
         "AlpnPolicy": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
-
 ListenerTypeDef = TypedDict(
     "ListenerTypeDef",
     {
         "ListenerArn": str,
         "LoadBalancerArn": str,
         "Port": int,
         "Protocol": ProtocolEnumType,
@@ -1374,21 +1339,19 @@
         "Certificates": Sequence[CertificateTypeDef],
         "DefaultActions": Sequence[ActionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Conditions": Sequence[RuleConditionTypeDef],
         "Priority": int,
         "Actions": Sequence[ActionTypeDef],
@@ -1398,21 +1361,19 @@
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRuleInputRequestTypeDef(
     _RequiredCreateRuleInputRequestTypeDef, _OptionalCreateRuleInputRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyRuleInputRequestTypeDef = TypedDict(
     "_RequiredModifyRuleInputRequestTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
@@ -1420,21 +1381,19 @@
     {
         "Conditions": Sequence[RuleConditionTypeDef],
         "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
 
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "RuleArn": str,
         "Priority": str,
         "Conditions": List[RuleConditionTypeDef],
         "Actions": List[ActionTypeDef],
@@ -1443,60 +1402,60 @@
     total=False,
 )
 
 CreateListenerOutputTypeDef = TypedDict(
     "CreateListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenersOutputTypeDef = TypedDict(
     "DescribeListenersOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyListenerOutputTypeDef = TypedDict(
     "ModifyListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleOutputTypeDef = TypedDict(
     "CreateRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRulesOutputTypeDef = TypedDict(
     "DescribeRulesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyRuleOutputTypeDef = TypedDict(
     "ModifyRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetRulePrioritiesOutputTypeDef = TypedDict(
     "SetRulePrioritiesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/type_defs.pyi` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,85 +32,86 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AuthenticateCognitoActionConfigTypeDef",
     "AuthenticateOidcActionConfigTypeDef",
     "FixedResponseActionConfigTypeDef",
     "RedirectActionConfigTypeDef",
     "CertificateTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "LoadBalancerAddressTypeDef",
     "CipherTypeDef",
     "SubnetMappingTypeDef",
     "MatcherTypeDef",
     "DeleteListenerInputRequestTypeDef",
     "DeleteLoadBalancerInputRequestTypeDef",
     "DeleteRuleInputRequestTypeDef",
     "DeleteTargetGroupInputRequestTypeDef",
     "TargetDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "LimitTypeDef",
+    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
     "DescribeListenerCertificatesInputRequestTypeDef",
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
     "DescribeListenersInputRequestTypeDef",
     "DescribeLoadBalancerAttributesInputRequestTypeDef",
     "LoadBalancerAttributeTypeDef",
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
     "WaiterConfigTypeDef",
     "DescribeLoadBalancersInputRequestTypeDef",
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
     "DescribeRulesInputRequestTypeDef",
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
     "DescribeSSLPoliciesInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "DescribeTargetGroupAttributesInputRequestTypeDef",
     "TargetGroupAttributeTypeDef",
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeTargetGroupsInputRequestTypeDef",
     "TargetGroupStickinessConfigTypeDef",
     "TargetGroupTupleTypeDef",
     "HostHeaderConditionConfigTypeDef",
     "HttpHeaderConditionConfigTypeDef",
     "HttpRequestMethodConditionConfigTypeDef",
     "LoadBalancerStateTypeDef",
+    "PaginatorConfigTypeDef",
     "PathPatternConditionConfigTypeDef",
     "QueryStringKeyValuePairTypeDef",
     "RemoveTagsInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SourceIpConditionConfigTypeDef",
     "RulePriorityPairTypeDef",
     "SetIpAddressTypeInputRequestTypeDef",
+    "SetIpAddressTypeOutputTypeDef",
     "SetSecurityGroupsInputRequestTypeDef",
+    "SetSecurityGroupsOutputTypeDef",
     "TargetHealthTypeDef",
     "AddListenerCertificatesInputRequestTypeDef",
-    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddListenerCertificatesOutputTypeDef",
     "DescribeListenerCertificatesOutputTypeDef",
-    "SetIpAddressTypeOutputTypeDef",
-    "SetSecurityGroupsOutputTypeDef",
+    "RemoveListenerCertificatesInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "TagDescriptionTypeDef",
     "AvailabilityZoneTypeDef",
     "SslPolicyTypeDef",
     "CreateLoadBalancerInputRequestTypeDef",
     "SetSubnetsInputRequestTypeDef",
     "CreateTargetGroupInputRequestTypeDef",
     "ModifyTargetGroupInputRequestTypeDef",
     "TargetGroupTypeDef",
     "DeregisterTargetsInputRequestTypeDef",
     "DescribeTargetHealthInputRequestTypeDef",
     "RegisterTargetsInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    "DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
     "DescribeAccountLimitsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     "ModifyLoadBalancerAttributesOutputTypeDef",
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef",
     "DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef",
@@ -166,19 +167,21 @@
         "SessionTimeout": int,
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateCognitoActionConditionalBehaviorEnumType,
     },
     total=False,
 )
 
+
 class AuthenticateCognitoActionConfigTypeDef(
     _RequiredAuthenticateCognitoActionConfigTypeDef, _OptionalAuthenticateCognitoActionConfigTypeDef
 ):
     pass
 
+
 _RequiredAuthenticateOidcActionConfigTypeDef = TypedDict(
     "_RequiredAuthenticateOidcActionConfigTypeDef",
     {
         "Issuer": str,
         "AuthorizationEndpoint": str,
         "TokenEndpoint": str,
         "UserInfoEndpoint": str,
@@ -195,19 +198,21 @@
         "AuthenticationRequestExtraParams": Mapping[str, str],
         "OnUnauthenticatedRequest": AuthenticateOidcActionConditionalBehaviorEnumType,
         "UseExistingClientSecret": bool,
     },
     total=False,
 )
 
+
 class AuthenticateOidcActionConfigTypeDef(
     _RequiredAuthenticateOidcActionConfigTypeDef, _OptionalAuthenticateOidcActionConfigTypeDef
 ):
     pass
 
+
 _RequiredFixedResponseActionConfigTypeDef = TypedDict(
     "_RequiredFixedResponseActionConfigTypeDef",
     {
         "StatusCode": str,
     },
 )
 _OptionalFixedResponseActionConfigTypeDef = TypedDict(
@@ -215,19 +220,21 @@
     {
         "MessageBody": str,
         "ContentType": str,
     },
     total=False,
 )
 
+
 class FixedResponseActionConfigTypeDef(
     _RequiredFixedResponseActionConfigTypeDef, _OptionalFixedResponseActionConfigTypeDef
 ):
     pass
 
+
 _RequiredRedirectActionConfigTypeDef = TypedDict(
     "_RequiredRedirectActionConfigTypeDef",
     {
         "StatusCode": RedirectActionStatusCodeEnumType,
     },
 )
 _OptionalRedirectActionConfigTypeDef = TypedDict(
@@ -238,56 +245,49 @@
         "Host": str,
         "Path": str,
         "Query": str,
     },
     total=False,
 )
 
+
 class RedirectActionConfigTypeDef(
     _RequiredRedirectActionConfigTypeDef, _OptionalRedirectActionConfigTypeDef
 ):
     pass
 
+
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateArn": str,
         "IsDefault": bool,
     },
     total=False,
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
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 LoadBalancerAddressTypeDef = TypedDict(
     "LoadBalancerAddressTypeDef",
     {
         "IpAddress": str,
         "AllocationId": str,
         "PrivateIPv4Address": str,
         "IPv6Address": str,
@@ -363,25 +363,25 @@
     {
         "Port": int,
         "AvailabilityZone": str,
     },
     total=False,
 )
 
+
 class TargetDescriptionTypeDef(
     _RequiredTargetDescriptionTypeDef, _OptionalTargetDescriptionTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -396,14 +396,36 @@
     {
         "Name": str,
         "Max": str,
     },
     total=False,
 )
 
+_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
+    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalDescribeListenerCertificatesInputRequestTypeDef = TypedDict(
@@ -411,20 +433,32 @@
     {
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class DescribeListenerCertificatesInputRequestTypeDef(
     _RequiredDescribeListenerCertificatesInputRequestTypeDef,
     _OptionalDescribeListenerCertificatesInputRequestTypeDef,
 ):
     pass
 
+
+DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
+    "DescribeListenersInputDescribeListenersPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "ListenerArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeListenersInputRequestTypeDef = TypedDict(
     "DescribeListenersInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "ListenerArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
@@ -444,14 +478,24 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
+    {
+        "LoadBalancerArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -464,25 +508,45 @@
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
+    "DescribeRulesInputDescribeRulesPaginateTypeDef",
+    {
+        "ListenerArn": str,
+        "RuleArns": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRulesInputRequestTypeDef = TypedDict(
     "DescribeRulesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "RuleArns": Sequence[str],
         "Marker": str,
         "PageSize": int,
     },
     total=False,
 )
 
+DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
+    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
+    {
+        "Names": Sequence[str],
+        "LoadBalancerType": LoadBalancerTypeEnumType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSSLPoliciesInputRequestTypeDef = TypedDict(
     "DescribeSSLPoliciesInputRequestTypeDef",
     {
         "Names": Sequence[str],
         "Marker": str,
         "PageSize": int,
         "LoadBalancerType": LoadBalancerTypeEnumType,
@@ -509,14 +573,25 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
+    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
+    {
+        "LoadBalancerArn": str,
+        "TargetGroupArns": Sequence[str],
+        "Names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeTargetGroupsInputRequestTypeDef = TypedDict(
     "DescribeTargetGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "TargetGroupArns": Sequence[str],
         "Names": Sequence[str],
         "Marker": str,
@@ -573,14 +648,24 @@
     {
         "Code": LoadBalancerStateEnumType,
         "Reason": str,
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
 PathPatternConditionConfigTypeDef = TypedDict(
     "PathPatternConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -598,14 +683,25 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
         "TagKeys": Sequence[str],
     },
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
 SourceIpConditionConfigTypeDef = TypedDict(
     "SourceIpConditionConfigTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
@@ -623,22 +719,38 @@
     "SetIpAddressTypeInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "IpAddressType": IpAddressTypeType,
     },
 )
 
+SetIpAddressTypeOutputTypeDef = TypedDict(
+    "SetIpAddressTypeOutputTypeDef",
+    {
+        "IpAddressType": IpAddressTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetSecurityGroupsInputRequestTypeDef = TypedDict(
     "SetSecurityGroupsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
         "SecurityGroups": Sequence[str],
     },
 )
 
+SetSecurityGroupsOutputTypeDef = TypedDict(
+    "SetSecurityGroupsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TargetHealthTypeDef = TypedDict(
     "TargetHealthTypeDef",
     {
         "State": TargetHealthStateEnumType,
         "Reason": TargetHealthReasonEnumType,
         "Description": str,
     },
@@ -649,52 +761,36 @@
     "AddListenerCertificatesInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
-RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
-    "RemoveListenerCertificatesInputRequestTypeDef",
-    {
-        "ListenerArn": str,
-        "Certificates": Sequence[CertificateTypeDef],
-    },
-)
-
 AddListenerCertificatesOutputTypeDef = TypedDict(
     "AddListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenerCertificatesOutputTypeDef = TypedDict(
     "DescribeListenerCertificatesOutputTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetIpAddressTypeOutputTypeDef = TypedDict(
-    "SetIpAddressTypeOutputTypeDef",
-    {
-        "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SetSecurityGroupsOutputTypeDef = TypedDict(
-    "SetSecurityGroupsOutputTypeDef",
+RemoveListenerCertificatesInputRequestTypeDef = TypedDict(
+    "RemoveListenerCertificatesInputRequestTypeDef",
     {
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ListenerArn": str,
+        "Certificates": Sequence[CertificateTypeDef],
     },
 )
 
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceArns": Sequence[str],
@@ -750,19 +846,21 @@
         "Type": LoadBalancerTypeEnumType,
         "IpAddressType": IpAddressTypeType,
         "CustomerOwnedIpv4Pool": str,
     },
     total=False,
 )
 
+
 class CreateLoadBalancerInputRequestTypeDef(
     _RequiredCreateLoadBalancerInputRequestTypeDef, _OptionalCreateLoadBalancerInputRequestTypeDef
 ):
     pass
 
+
 _RequiredSetSubnetsInputRequestTypeDef = TypedDict(
     "_RequiredSetSubnetsInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
     },
 )
 _OptionalSetSubnetsInputRequestTypeDef = TypedDict(
@@ -771,19 +869,21 @@
         "Subnets": Sequence[str],
         "SubnetMappings": Sequence[SubnetMappingTypeDef],
         "IpAddressType": IpAddressTypeType,
     },
     total=False,
 )
 
+
 class SetSubnetsInputRequestTypeDef(
     _RequiredSetSubnetsInputRequestTypeDef, _OptionalSetSubnetsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTargetGroupInputRequestTypeDef = TypedDict(
@@ -805,19 +905,21 @@
         "TargetType": TargetTypeEnumType,
         "Tags": Sequence[TagTypeDef],
         "IpAddressType": TargetGroupIpAddressTypeEnumType,
     },
     total=False,
 )
 
+
 class CreateTargetGroupInputRequestTypeDef(
     _RequiredCreateTargetGroupInputRequestTypeDef, _OptionalCreateTargetGroupInputRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyTargetGroupInputRequestTypeDef = TypedDict(
     "_RequiredModifyTargetGroupInputRequestTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalModifyTargetGroupInputRequestTypeDef = TypedDict(
@@ -832,19 +934,21 @@
         "HealthyThresholdCount": int,
         "UnhealthyThresholdCount": int,
         "Matcher": MatcherTypeDef,
     },
     total=False,
 )
 
+
 class ModifyTargetGroupInputRequestTypeDef(
     _RequiredModifyTargetGroupInputRequestTypeDef, _OptionalModifyTargetGroupInputRequestTypeDef
 ):
     pass
 
+
 TargetGroupTypeDef = TypedDict(
     "TargetGroupTypeDef",
     {
         "TargetGroupArn": str,
         "TargetGroupName": str,
         "Protocol": ProtocolEnumType,
         "Port": int,
@@ -884,121 +988,44 @@
     "_OptionalDescribeTargetHealthInputRequestTypeDef",
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
     total=False,
 )
 
+
 class DescribeTargetHealthInputRequestTypeDef(
     _RequiredDescribeTargetHealthInputRequestTypeDef,
     _OptionalDescribeTargetHealthInputRequestTypeDef,
 ):
     pass
 
+
 RegisterTargetsInputRequestTypeDef = TypedDict(
     "RegisterTargetsInputRequestTypeDef",
     {
         "TargetGroupArn": str,
         "Targets": Sequence[TargetDescriptionTypeDef],
     },
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef(
-    _RequiredDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    _OptionalDescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-):
-    pass
-
-DescribeListenersInputDescribeListenersPaginateTypeDef = TypedDict(
-    "DescribeListenersInputDescribeListenersPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "ListenerArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef",
-    {
-        "LoadBalancerArns": Sequence[str],
-        "Names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeRulesInputDescribeRulesPaginateTypeDef = TypedDict(
-    "DescribeRulesInputDescribeRulesPaginateTypeDef",
-    {
-        "ListenerArn": str,
-        "RuleArns": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef = TypedDict(
-    "DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef",
-    {
-        "Names": Sequence[str],
-        "LoadBalancerType": LoadBalancerTypeEnumType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef = TypedDict(
-    "DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef",
-    {
-        "LoadBalancerArn": str,
-        "TargetGroupArns": Sequence[str],
-        "Names": Sequence[str],
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
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1006,15 +1033,15 @@
     },
 )
 
 ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
     "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "Attributes": List[LoadBalancerAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef = TypedDict(
     "DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef",
     {
         "LoadBalancerArns": Sequence[str],
@@ -1061,20 +1088,22 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTargetHealthInputTargetDeregisteredWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetDeregisteredWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
     "_RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef",
     {
         "TargetGroupArn": str,
     },
 )
 _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef = TypedDict(
@@ -1082,25 +1111,27 @@
     {
         "Targets": Sequence[TargetDescriptionTypeDef],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTargetHealthInputTargetInServiceWaitTypeDef(
     _RequiredDescribeTargetHealthInputTargetInServiceWaitTypeDef,
     _OptionalDescribeTargetHealthInputTargetInServiceWaitTypeDef,
 ):
     pass
 
+
 DescribeTargetGroupAttributesOutputTypeDef = TypedDict(
     "DescribeTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyTargetGroupAttributesInputRequestTypeDef = TypedDict(
     "ModifyTargetGroupAttributesInputRequestTypeDef",
     {
         "TargetGroupArn": str,
@@ -1108,15 +1139,15 @@
     },
 )
 
 ModifyTargetGroupAttributesOutputTypeDef = TypedDict(
     "ModifyTargetGroupAttributesOutputTypeDef",
     {
         "Attributes": List[TargetGroupAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ForwardActionConfigTypeDef = TypedDict(
     "ForwardActionConfigTypeDef",
     {
         "TargetGroups": Sequence[TargetGroupTupleTypeDef],
@@ -1150,15 +1181,15 @@
     total=False,
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "TagDescriptions": List[TagDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoadBalancerTypeDef = TypedDict(
     "LoadBalancerTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1179,49 +1210,49 @@
 )
 
 SetSubnetsOutputTypeDef = TypedDict(
     "SetSubnetsOutputTypeDef",
     {
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "IpAddressType": IpAddressTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSSLPoliciesOutputTypeDef = TypedDict(
     "DescribeSSLPoliciesOutputTypeDef",
     {
         "SslPolicies": List[SslPolicyTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTargetGroupOutputTypeDef = TypedDict(
     "CreateTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTargetGroupsOutputTypeDef = TypedDict(
     "DescribeTargetGroupsOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyTargetGroupOutputTypeDef = TypedDict(
     "ModifyTargetGroupOutputTypeDef",
     {
         "TargetGroups": List[TargetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActionTypeDef = TypedDict(
     "_RequiredActionTypeDef",
     {
         "Type": ActionTypeEnumType,
@@ -1237,17 +1268,19 @@
         "RedirectConfig": RedirectActionConfigTypeDef,
         "FixedResponseConfig": FixedResponseActionConfigTypeDef,
         "ForwardConfig": ForwardActionConfigTypeDef,
     },
     total=False,
 )
 
+
 class ActionTypeDef(_RequiredActionTypeDef, _OptionalActionTypeDef):
     pass
 
+
 RuleConditionTypeDef = TypedDict(
     "RuleConditionTypeDef",
     {
         "Field": str,
         "Values": Sequence[str],
         "HostHeaderConfig": HostHeaderConditionConfigTypeDef,
         "PathPatternConfig": PathPatternConditionConfigTypeDef,
@@ -1259,32 +1292,32 @@
     total=False,
 )
 
 DescribeTargetHealthOutputTypeDef = TypedDict(
     "DescribeTargetHealthOutputTypeDef",
     {
         "TargetHealthDescriptions": List[TargetHealthDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateLoadBalancerOutputTypeDef = TypedDict(
     "CreateLoadBalancerOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLoadBalancersOutputTypeDef = TypedDict(
     "DescribeLoadBalancersOutputTypeDef",
     {
         "LoadBalancers": List[LoadBalancerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateListenerInputRequestTypeDef = TypedDict(
     "_RequiredCreateListenerInputRequestTypeDef",
     {
         "LoadBalancerArn": str,
@@ -1300,19 +1333,21 @@
         "Certificates": Sequence[CertificateTypeDef],
         "AlpnPolicy": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateListenerInputRequestTypeDef(
     _RequiredCreateListenerInputRequestTypeDef, _OptionalCreateListenerInputRequestTypeDef
 ):
     pass
 
+
 ListenerTypeDef = TypedDict(
     "ListenerTypeDef",
     {
         "ListenerArn": str,
         "LoadBalancerArn": str,
         "Port": int,
         "Protocol": ProtocolEnumType,
@@ -1339,19 +1374,21 @@
         "Certificates": Sequence[CertificateTypeDef],
         "DefaultActions": Sequence[ActionTypeDef],
         "AlpnPolicy": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyListenerInputRequestTypeDef(
     _RequiredModifyListenerInputRequestTypeDef, _OptionalModifyListenerInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreateRuleInputRequestTypeDef",
     {
         "ListenerArn": str,
         "Conditions": Sequence[RuleConditionTypeDef],
         "Priority": int,
         "Actions": Sequence[ActionTypeDef],
@@ -1361,19 +1398,21 @@
     "_OptionalCreateRuleInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRuleInputRequestTypeDef(
     _RequiredCreateRuleInputRequestTypeDef, _OptionalCreateRuleInputRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyRuleInputRequestTypeDef = TypedDict(
     "_RequiredModifyRuleInputRequestTypeDef",
     {
         "RuleArn": str,
     },
 )
 _OptionalModifyRuleInputRequestTypeDef = TypedDict(
@@ -1381,19 +1420,21 @@
     {
         "Conditions": Sequence[RuleConditionTypeDef],
         "Actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
+
 class ModifyRuleInputRequestTypeDef(
     _RequiredModifyRuleInputRequestTypeDef, _OptionalModifyRuleInputRequestTypeDef
 ):
     pass
 
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "RuleArn": str,
         "Priority": str,
         "Conditions": List[RuleConditionTypeDef],
         "Actions": List[ActionTypeDef],
@@ -1402,60 +1443,60 @@
     total=False,
 )
 
 CreateListenerOutputTypeDef = TypedDict(
     "CreateListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeListenersOutputTypeDef = TypedDict(
     "DescribeListenersOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyListenerOutputTypeDef = TypedDict(
     "ModifyListenerOutputTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRuleOutputTypeDef = TypedDict(
     "CreateRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRulesOutputTypeDef = TypedDict(
     "DescribeRulesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyRuleOutputTypeDef = TypedDict(
     "ModifyRuleOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetRulePrioritiesOutputTypeDef = TypedDict(
     "SetRulePrioritiesOutputTypeDef",
     {
         "Rules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/waiter.py` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2/waiter.pyi` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/PKG-INFO` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elbv2
-Version: 1.26.63
-Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.26.63 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.ElasticLoadBalancingv2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-elbv2"></a>
 
 # mypy-boto3-elbv2
 
 [![PyPI - mypy-boto3-elbv2](https://img.shields.io/pypi/v/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elbv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-elbv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elbv2?color=blue)](https://pypistats.org/packages/mypy-boto3-elbv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticLoadBalancingv2 1.26.63](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
+[boto3.ElasticLoadBalancingv2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#ElasticLoadBalancingv2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-elbv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,79 +409,79 @@
 ```python
 from mypy_boto3_elbv2.type_defs import (
     AuthenticateCognitoActionConfigTypeDef,
     AuthenticateOidcActionConfigTypeDef,
     FixedResponseActionConfigTypeDef,
     RedirectActionConfigTypeDef,
     CertificateTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     LoadBalancerAddressTypeDef,
     CipherTypeDef,
     SubnetMappingTypeDef,
     MatcherTypeDef,
     DeleteListenerInputRequestTypeDef,
     DeleteLoadBalancerInputRequestTypeDef,
     DeleteRuleInputRequestTypeDef,
     DeleteTargetGroupInputRequestTypeDef,
     TargetDescriptionTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     LimitTypeDef,
+    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
     DescribeListenerCertificatesInputRequestTypeDef,
+    DescribeListenersInputDescribeListenersPaginateTypeDef,
     DescribeListenersInputRequestTypeDef,
     DescribeLoadBalancerAttributesInputRequestTypeDef,
     LoadBalancerAttributeTypeDef,
+    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
     WaiterConfigTypeDef,
     DescribeLoadBalancersInputRequestTypeDef,
+    DescribeRulesInputDescribeRulesPaginateTypeDef,
     DescribeRulesInputRequestTypeDef,
+    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
     DescribeSSLPoliciesInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     DescribeTargetGroupAttributesInputRequestTypeDef,
     TargetGroupAttributeTypeDef,
+    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeTargetGroupsInputRequestTypeDef,
     TargetGroupStickinessConfigTypeDef,
     TargetGroupTupleTypeDef,
     HostHeaderConditionConfigTypeDef,
     HttpHeaderConditionConfigTypeDef,
     HttpRequestMethodConditionConfigTypeDef,
     LoadBalancerStateTypeDef,
+    PaginatorConfigTypeDef,
     PathPatternConditionConfigTypeDef,
     QueryStringKeyValuePairTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     SourceIpConditionConfigTypeDef,
     RulePriorityPairTypeDef,
     SetIpAddressTypeInputRequestTypeDef,
+    SetIpAddressTypeOutputTypeDef,
     SetSecurityGroupsInputRequestTypeDef,
+    SetSecurityGroupsOutputTypeDef,
     TargetHealthTypeDef,
     AddListenerCertificatesInputRequestTypeDef,
-    RemoveListenerCertificatesInputRequestTypeDef,
     AddListenerCertificatesOutputTypeDef,
     DescribeListenerCertificatesOutputTypeDef,
-    SetIpAddressTypeOutputTypeDef,
-    SetSecurityGroupsOutputTypeDef,
+    RemoveListenerCertificatesInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     TagDescriptionTypeDef,
     AvailabilityZoneTypeDef,
     SslPolicyTypeDef,
     CreateLoadBalancerInputRequestTypeDef,
     SetSubnetsInputRequestTypeDef,
     CreateTargetGroupInputRequestTypeDef,
     ModifyTargetGroupInputRequestTypeDef,
     TargetGroupTypeDef,
     DeregisterTargetsInputRequestTypeDef,
     DescribeTargetHealthInputRequestTypeDef,
     RegisterTargetsInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeListenerCertificatesInputDescribeListenerCertificatesPaginateTypeDef,
-    DescribeListenersInputDescribeListenersPaginateTypeDef,
-    DescribeLoadBalancersInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeRulesInputDescribeRulesPaginateTypeDef,
-    DescribeSSLPoliciesInputDescribeSSLPoliciesPaginateTypeDef,
-    DescribeTargetGroupsInputDescribeTargetGroupsPaginateTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeLoadBalancerAttributesOutputTypeDef,
     ModifyLoadBalancerAttributesInputRequestTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     DescribeLoadBalancersInputLoadBalancerAvailableWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancerExistsWaitTypeDef,
     DescribeLoadBalancersInputLoadBalancersDeletedWaitTypeDef,
@@ -529,42 +529,42 @@
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

### Comparing `mypy-boto3-elbv2-1.26.63/mypy_boto3_elbv2.egg-info/SOURCES.txt` & `mypy-boto3-elbv2-1.27.0/mypy_boto3_elbv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elbv2-1.26.63/setup.py` & `mypy-boto3-elbv2-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-elbv2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elbv2",
-    version="1.26.63",
+    version="1.27.0",
     packages=["mypy_boto3_elbv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticLoadBalancingv2 1.26.63 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ElasticLoadBalancingv2 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elbv2/",
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


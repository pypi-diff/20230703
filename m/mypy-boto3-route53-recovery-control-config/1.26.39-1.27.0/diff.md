# Comparing `tmp/mypy-boto3-route53-recovery-control-config-1.26.39.tar.gz` & `tmp/mypy-boto3-route53-recovery-control-config-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-control-config-1.26.39.tar", last modified: Wed Dec 28 20:24:49 2022, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-control-config-1.27.0.tar", last modified: Mon Jul  3 19:51:21 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-control-config-1.26.39.tar` & `mypy-boto3-route53-recovery-control-config-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:49.377914 mypy-boto3-route53-recovery-control-config-1.26.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18997 2022-12-28 20:24:49.373914 mypy-boto3-route53-recovery-control-config-1.26.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:49.373914 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23819 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23778 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2022-12-28 20:24:41.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2022-12-28 20:24:41.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23185 2022-12-28 20:24:41.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 20:24:49.373914 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18997 2022-12-28 20:24:49.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2022-12-28 20:24:49.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 20:24:49.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 20:24:49.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-28 20:24:49.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-28 20:24:49.000000 mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 20:24:49.377914 mypy-boto3-route53-recovery-control-config-1.26.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2022-12-28 20:24:40.000000 mypy-boto3-route53-recovery-control-config-1.26.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.711903 mypy-boto3-route53-recovery-control-config-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-07-03 19:51:21.703903 mypy-boto3-route53-recovery-control-config-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.703903 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23819 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23778 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23260 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-07-03 19:46:33.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.703903 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:21.711903 mypy-boto3-route53-recovery-control-config-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-control-config-1.27.0/setup.py
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/LICENSE` & `mypy-boto3-route53-recovery-control-config-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/PKG-INFO` & `mypy-boto3-route53-recovery-control-config-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-control-config
-Version: 1.26.39
-Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.26.39 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53-recovery-control-config"></a>
 
 # mypy-boto3-route53-recovery-control-config
 
 [![PyPI - mypy-boto3-route53-recovery-control-config](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-control-config?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryControlConfig 1.26.39](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[boto3.Route53RecoveryControlConfig 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53-recovery-control-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,66 +392,66 @@
 ```python
 from mypy_boto3_route53_recovery_control_config.type_defs import (
     RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
     RoutingControlTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteControlPanelRequestRequestTypeDef,
     DeleteRoutingControlRequestRequestTypeDef,
     DeleteSafetyRuleRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeControlPanelRequestRequestTypeDef,
     DescribeRoutingControlRequestRequestTypeDef,
     DescribeSafetyRuleRequestRequestTypeDef,
     GatingRuleUpdateTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
+    ListAssociatedRoute53HealthChecksResponseTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListControlPanelsRequestRequestTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
+    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
     NewAssertionRuleTypeDef,
     NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
     CreateRoutingControlResponseTypeDef,
     DescribeRoutingControlResponseTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlResponseTypeDef,
     DescribeClusterRequestClusterCreatedWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
     DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
     CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
@@ -467,42 +467,42 @@
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

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/README.md` & `mypy-boto3-route53-recovery-control-config-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53-recovery-control-config"></a>
 
 # mypy-boto3-route53-recovery-control-config
 
 [![PyPI - mypy-boto3-route53-recovery-control-config](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-control-config?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryControlConfig 1.26.39](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[boto3.Route53RecoveryControlConfig 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53-recovery-control-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,66 +360,66 @@
 ```python
 from mypy_boto3_route53_recovery_control_config.type_defs import (
     RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
     RoutingControlTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteControlPanelRequestRequestTypeDef,
     DeleteRoutingControlRequestRequestTypeDef,
     DeleteSafetyRuleRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeControlPanelRequestRequestTypeDef,
     DescribeRoutingControlRequestRequestTypeDef,
     DescribeSafetyRuleRequestRequestTypeDef,
     GatingRuleUpdateTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
+    ListAssociatedRoute53HealthChecksResponseTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListControlPanelsRequestRequestTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
+    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
     NewAssertionRuleTypeDef,
     NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
     CreateRoutingControlResponseTypeDef,
     DescribeRoutingControlResponseTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlResponseTypeDef,
     DescribeClusterRequestClusterCreatedWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
     DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
     CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
@@ -435,42 +435,42 @@
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

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/__init__.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/__init__.pyi` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/__main__.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryControlConfig 1.26.39\nVersion:        "
-        " 1.26.39\nBuilder version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryControlConfig 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.39")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/client.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/client.pyi` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/literals.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/literals.py`

 * *Files 2% similar despite different names*

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
@@ -94,31 +95,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -197,14 +201,15 @@
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
@@ -215,18 +220,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -257,14 +264,15 @@
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
@@ -283,16 +291,19 @@
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
@@ -372,18 +383,21 @@
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

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/literals.pyi` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/literals.pyi`

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
@@ -92,31 +93,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -195,14 +199,15 @@
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
@@ -213,18 +218,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -255,14 +262,15 @@
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
@@ -281,16 +289,19 @@
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
@@ -370,18 +381,21 @@
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

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/paginator.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 class ListAssociatedRoute53HealthChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
     """
 
     def paginate(
-        self, *, RoutingControlArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RoutingControlArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedRoute53HealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listclusterspaginator)
         """
 
 
 class ListControlPanelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListControlPanelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
         """
 
 
 class ListRoutingControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
         """
 
 
 class ListSafetyRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSafetyRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/paginator.pyi` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,69 +59,69 @@
 class ListAssociatedRoute53HealthChecksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
     """
 
     def paginate(
-        self, *, RoutingControlArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RoutingControlArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedRoute53HealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listassociatedroute53healthcheckspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listclusterspaginator)
         """
 
 class ListControlPanelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListControlPanelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListControlPanels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listcontrolpanelspaginator)
         """
 
 class ListRoutingControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listroutingcontrolspaginator)
         """
 
 class ListSafetyRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ControlPanelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSafetyRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/paginators/#listsafetyrulespaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/type_defs.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,66 +24,66 @@
 
 __all__ = (
     "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateControlPanelRequestRequestTypeDef",
     "CreateRoutingControlRequestRequestTypeDef",
     "RoutingControlTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteControlPanelRequestRequestTypeDef",
     "DeleteRoutingControlRequestRequestTypeDef",
     "DeleteSafetyRuleRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeControlPanelRequestRequestTypeDef",
     "DescribeRoutingControlRequestRequestTypeDef",
     "DescribeSafetyRuleRequestRequestTypeDef",
     "GatingRuleUpdateTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
     "ListAssociatedRoute53HealthChecksRequestRequestTypeDef",
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
     "ListControlPanelsRequestRequestTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
+    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "ListSafetyRulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateControlPanelRequestRequestTypeDef",
     "UpdateRoutingControlRequestRequestTypeDef",
     "AssertionRuleTypeDef",
     "GatingRuleTypeDef",
     "NewAssertionRuleTypeDef",
     "NewGatingRuleTypeDef",
     "ClusterTypeDef",
     "CreateControlPanelResponseTypeDef",
     "DescribeControlPanelResponseTypeDef",
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
     "ListControlPanelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateControlPanelResponseTypeDef",
     "CreateRoutingControlResponseTypeDef",
     "DescribeRoutingControlResponseTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlResponseTypeDef",
     "DescribeClusterRequestClusterCreatedWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelCreatedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelDeletedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef",
     "UpdateSafetyRuleRequestRequestTypeDef",
-    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "CreateSafetyRuleResponseTypeDef",
     "DescribeSafetyRuleResponseTypeDef",
     "RuleTypeDef",
     "UpdateSafetyRuleResponseTypeDef",
     "CreateSafetyRuleRequestRequestTypeDef",
     "CreateClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -149,25 +149,14 @@
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
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
 _RequiredCreateControlPanelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateControlPanelRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ControlPanelName": str,
     },
 )
@@ -293,24 +282,36 @@
     {
         "Name": str,
         "SafetyRuleArn": str,
         "WaitPeriodMs": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "RoutingControlArn": str,
+    },
+)
+_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
+    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
@@ -326,33 +327,81 @@
 class ListAssociatedRoute53HealthChecksRequestRequestTypeDef(
     _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef,
 ):
     pass
 
 
+ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
+    {
+        "HealthCheckIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListControlPanelsRequestRequestTypeDef = TypedDict(
     "ListControlPanelsRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
+    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRoutingControlsRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingControlsRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListRoutingControlsRequestRequestTypeDef = TypedDict(
@@ -368,14 +417,36 @@
 class ListRoutingControlsRequestRequestTypeDef(
     _RequiredListRoutingControlsRequestRequestTypeDef,
     _OptionalListRoutingControlsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
+    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSafetyRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListSafetyRulesRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListSafetyRulesRequestRequestTypeDef = TypedDict(
@@ -397,14 +468,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -494,90 +594,73 @@
     total=False,
 )
 
 CreateControlPanelResponseTypeDef = TypedDict(
     "CreateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeControlPanelResponseTypeDef = TypedDict(
     "DescribeControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
-    {
-        "HealthCheckIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlPanelsResponseTypeDef = TypedDict(
     "ListControlPanelsResponseTypeDef",
     {
         "ControlPanels": List[ControlPanelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateControlPanelResponseTypeDef = TypedDict(
     "UpdateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRoutingControlResponseTypeDef = TypedDict(
     "CreateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRoutingControlResponseTypeDef = TypedDict(
     "DescribeRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "NextToken": str,
         "RoutingControls": List[RoutingControlTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRoutingControlResponseTypeDef = TypedDict(
     "UpdateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeClusterRequestClusterCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterCreatedWaitTypeDef",
     {
         "ClusterArn": str,
@@ -714,112 +797,29 @@
     {
         "AssertionRuleUpdate": AssertionRuleUpdateTypeDef,
         "GatingRuleUpdate": GatingRuleUpdateTypeDef,
     },
     total=False,
 )
 
-_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    {
-        "RoutingControlArn": str,
-    },
-)
-_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
-    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
-    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
-    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-):
-    pass
-
-
 CreateSafetyRuleResponseTypeDef = TypedDict(
     "CreateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSafetyRuleResponseTypeDef = TypedDict(
     "DescribeSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "ASSERTION": AssertionRuleTypeDef,
@@ -829,15 +829,15 @@
 )
 
 UpdateSafetyRuleResponseTypeDef = TypedDict(
     "UpdateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSafetyRuleRequestRequestTypeDef = TypedDict(
     "CreateSafetyRuleRequestRequestTypeDef",
     {
         "AssertionRule": NewAssertionRuleTypeDef,
@@ -848,36 +848,36 @@
     total=False,
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSafetyRulesResponseTypeDef = TypedDict(
     "ListSafetyRulesResponseTypeDef",
     {
         "NextToken": str,
         "SafetyRules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/type_defs.pyi` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,66 +23,66 @@
 
 __all__ = (
     "RuleConfigTypeDef",
     "AssertionRuleUpdateTypeDef",
     "ClusterEndpointTypeDef",
     "ControlPanelTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateControlPanelRequestRequestTypeDef",
     "CreateRoutingControlRequestRequestTypeDef",
     "RoutingControlTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteControlPanelRequestRequestTypeDef",
     "DeleteRoutingControlRequestRequestTypeDef",
     "DeleteSafetyRuleRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeControlPanelRequestRequestTypeDef",
     "DescribeRoutingControlRequestRequestTypeDef",
     "DescribeSafetyRuleRequestRequestTypeDef",
     "GatingRuleUpdateTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
     "ListAssociatedRoute53HealthChecksRequestRequestTypeDef",
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
     "ListControlPanelsRequestRequestTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
+    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "ListSafetyRulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateControlPanelRequestRequestTypeDef",
     "UpdateRoutingControlRequestRequestTypeDef",
     "AssertionRuleTypeDef",
     "GatingRuleTypeDef",
     "NewAssertionRuleTypeDef",
     "NewGatingRuleTypeDef",
     "ClusterTypeDef",
     "CreateControlPanelResponseTypeDef",
     "DescribeControlPanelResponseTypeDef",
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
     "ListControlPanelsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdateControlPanelResponseTypeDef",
     "CreateRoutingControlResponseTypeDef",
     "DescribeRoutingControlResponseTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlResponseTypeDef",
     "DescribeClusterRequestClusterCreatedWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelCreatedWaitTypeDef",
     "DescribeControlPanelRequestControlPanelDeletedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef",
     "DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef",
     "UpdateSafetyRuleRequestRequestTypeDef",
-    "ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    "ListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
     "CreateSafetyRuleResponseTypeDef",
     "DescribeSafetyRuleResponseTypeDef",
     "RuleTypeDef",
     "UpdateSafetyRuleResponseTypeDef",
     "CreateSafetyRuleRequestRequestTypeDef",
     "CreateClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -146,25 +146,14 @@
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
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
 _RequiredCreateControlPanelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateControlPanelRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ControlPanelName": str,
     },
 )
@@ -286,24 +275,34 @@
     {
         "Name": str,
         "SafetyRuleArn": str,
         "WaitPeriodMs": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "RoutingControlArn": str,
+    },
+)
+_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
+    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef = TypedDict(
@@ -317,33 +316,79 @@
 
 class ListAssociatedRoute53HealthChecksRequestRequestTypeDef(
     _RequiredListAssociatedRoute53HealthChecksRequestRequestTypeDef,
     _OptionalListAssociatedRoute53HealthChecksRequestRequestTypeDef,
 ):
     pass
 
+ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
+    "ListAssociatedRoute53HealthChecksResponseTypeDef",
+    {
+        "HealthCheckIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
+    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListControlPanelsRequestRequestTypeDef = TypedDict(
     "ListControlPanelsRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
+    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRoutingControlsRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutingControlsRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListRoutingControlsRequestRequestTypeDef = TypedDict(
@@ -357,14 +402,34 @@
 
 class ListRoutingControlsRequestRequestTypeDef(
     _RequiredListRoutingControlsRequestRequestTypeDef,
     _OptionalListRoutingControlsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+    },
+)
+_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
+    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
+    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
+):
+    pass
+
 _RequiredListSafetyRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListSafetyRulesRequestRequestTypeDef",
     {
         "ControlPanelArn": str,
     },
 )
 _OptionalListSafetyRulesRequestRequestTypeDef = TypedDict(
@@ -384,14 +449,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -481,90 +575,73 @@
     total=False,
 )
 
 CreateControlPanelResponseTypeDef = TypedDict(
     "CreateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeControlPanelResponseTypeDef = TypedDict(
     "DescribeControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssociatedRoute53HealthChecksResponseTypeDef = TypedDict(
-    "ListAssociatedRoute53HealthChecksResponseTypeDef",
-    {
-        "HealthCheckIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListControlPanelsResponseTypeDef = TypedDict(
     "ListControlPanelsResponseTypeDef",
     {
         "ControlPanels": List[ControlPanelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateControlPanelResponseTypeDef = TypedDict(
     "UpdateControlPanelResponseTypeDef",
     {
         "ControlPanel": ControlPanelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRoutingControlResponseTypeDef = TypedDict(
     "CreateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRoutingControlResponseTypeDef = TypedDict(
     "DescribeRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "NextToken": str,
         "RoutingControls": List[RoutingControlTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRoutingControlResponseTypeDef = TypedDict(
     "UpdateRoutingControlResponseTypeDef",
     {
         "RoutingControl": RoutingControlTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeClusterRequestClusterCreatedWaitTypeDef = TypedDict(
     "_RequiredDescribeClusterRequestClusterCreatedWaitTypeDef",
     {
         "ClusterArn": str,
@@ -689,106 +766,29 @@
     {
         "AssertionRuleUpdate": AssertionRuleUpdateTypeDef,
         "GatingRuleUpdate": GatingRuleUpdateTypeDef,
     },
     total=False,
 )
 
-_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    {
-        "RoutingControlArn": str,
-    },
-)
-_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef(
-    _RequiredListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    _OptionalListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListControlPanelsRequestListControlPanelsPaginateTypeDef = TypedDict(
-    "ListControlPanelsRequestListControlPanelsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "_OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRoutingControlsRequestListRoutingControlsPaginateTypeDef(
-    _RequiredListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    _OptionalListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-):
-    pass
-
-_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-    },
-)
-_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef = TypedDict(
-    "_OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSafetyRulesRequestListSafetyRulesPaginateTypeDef(
-    _RequiredListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    _OptionalListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-):
-    pass
-
 CreateSafetyRuleResponseTypeDef = TypedDict(
     "CreateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSafetyRuleResponseTypeDef = TypedDict(
     "DescribeSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "ASSERTION": AssertionRuleTypeDef,
@@ -798,15 +798,15 @@
 )
 
 UpdateSafetyRuleResponseTypeDef = TypedDict(
     "UpdateSafetyRuleResponseTypeDef",
     {
         "AssertionRule": AssertionRuleTypeDef,
         "GatingRule": GatingRuleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSafetyRuleRequestRequestTypeDef = TypedDict(
     "CreateSafetyRuleRequestRequestTypeDef",
     {
         "AssertionRule": NewAssertionRuleTypeDef,
@@ -817,36 +817,36 @@
     total=False,
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSafetyRulesResponseTypeDef = TypedDict(
     "ListSafetyRulesResponseTypeDef",
     {
         "NextToken": str,
         "SafetyRules": List[RuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/waiter.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config/waiter.pyi` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-control-config
-Version: 1.26.39
-Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.26.39 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53RecoveryControlConfig 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53-recovery-control-config"></a>
 
 # mypy-boto3-route53-recovery-control-config
 
 [![PyPI - mypy-boto3-route53-recovery-control-config](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-control-config)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-control-config?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-control-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryControlConfig 1.26.39](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
+[boto3.Route53RecoveryControlConfig 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53-recovery-control-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,66 +392,66 @@
 ```python
 from mypy_boto3_route53_recovery_control_config.type_defs import (
     RuleConfigTypeDef,
     AssertionRuleUpdateTypeDef,
     ClusterEndpointTypeDef,
     ControlPanelTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateControlPanelRequestRequestTypeDef,
     CreateRoutingControlRequestRequestTypeDef,
     RoutingControlTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteControlPanelRequestRequestTypeDef,
     DeleteRoutingControlRequestRequestTypeDef,
     DeleteSafetyRuleRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeControlPanelRequestRequestTypeDef,
     DescribeRoutingControlRequestRequestTypeDef,
     DescribeSafetyRuleRequestRequestTypeDef,
     GatingRuleUpdateTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
     ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
+    ListAssociatedRoute53HealthChecksResponseTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
     ListControlPanelsRequestRequestTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
+    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     ListSafetyRulesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateControlPanelRequestRequestTypeDef,
     UpdateRoutingControlRequestRequestTypeDef,
     AssertionRuleTypeDef,
     GatingRuleTypeDef,
     NewAssertionRuleTypeDef,
     NewGatingRuleTypeDef,
     ClusterTypeDef,
     CreateControlPanelResponseTypeDef,
     DescribeControlPanelResponseTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
     ListControlPanelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdateControlPanelResponseTypeDef,
     CreateRoutingControlResponseTypeDef,
     DescribeRoutingControlResponseTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlResponseTypeDef,
     DescribeClusterRequestClusterCreatedWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
     DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
     DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
     UpdateSafetyRuleRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
     CreateSafetyRuleResponseTypeDef,
     DescribeSafetyRuleResponseTypeDef,
     RuleTypeDef,
     UpdateSafetyRuleResponseTypeDef,
     CreateSafetyRuleRequestRequestTypeDef,
     CreateClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
@@ -467,42 +467,42 @@
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

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-control-config-1.27.0/mypy_boto3_route53_recovery_control_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-control-config-1.26.39/setup.py` & `mypy-boto3-route53-recovery-control-config-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-route53-recovery-control-config.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-control-config",
-    version="1.26.39",
+    version="1.27.0",
     packages=["mypy_boto3_route53_recovery_control_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryControlConfig 1.26.39 service generated with"
-        " mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.Route53RecoveryControlConfig 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -50,11 +50,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_control_config/"
         ),
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


# Comparing `tmp/mypy-boto3-kafkaconnect-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-kafkaconnect-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafkaconnect-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:36 2022, max compression
+gzip compressed data, was "mypy-boto3-kafkaconnect-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
```

## Comparing `mypy-boto3-kafkaconnect-1.26.0.post1.tar` & `mypy-boto3-kafkaconnect-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:36.564831 mypy-boto3-kafkaconnect-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16403 2022-11-01 21:43:36.556831 mypy-boto3-kafkaconnect-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14942 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:36.544831 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12818 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12796 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8194 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8192 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4176 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    25514 2022-11-01 21:36:34.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    25493 2022-11-01 21:36:34.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:36.556831 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16403 2022-11-01 21:43:36.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-01 21:43:36.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:36.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:36.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:36.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:36.000000 mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:36.564831 mypy-boto3-kafkaconnect-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:36:33.000000 mypy-boto3-kafkaconnect-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.247481 mypy-boto3-kafkaconnect-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-03 19:50:57.247481 mypy-boto3-kafkaconnect-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.247481 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25544 2023-07-03 19:40:10.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25523 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.247481 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-03 19:50:57.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:57.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:57.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:57.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:57.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:57.000000 mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:57.247481 mypy-boto3-kafkaconnect-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:40:09.000000 mypy-boto3-kafkaconnect-1.27.0/setup.py
```

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/LICENSE` & `mypy-boto3-kafkaconnect-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/PKG-INFO` & `mypy-boto3-kafkaconnect-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafkaconnect
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.KafkaConnect 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.KafkaConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/
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
 
 <a id="mypy-boto3-kafkaconnect"></a>
 
 # mypy-boto3-kafkaconnect
 
 [![PyPI - mypy-boto3-kafkaconnect](https://img.shields.io/pypi/v/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafkaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KafkaConnect 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[boto3.KafkaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [mypy-boto3-kafkaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,57 +355,57 @@
     CloudWatchLogsLogDeliveryTypeDef,
     KafkaClusterClientAuthenticationDescriptionTypeDef,
     KafkaClusterEncryptionInTransitDescriptionTypeDef,
     WorkerConfigurationDescriptionTypeDef,
     KafkaClusterClientAuthenticationTypeDef,
     KafkaClusterEncryptionInTransitTypeDef,
     WorkerConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateCustomPluginResponseTypeDef,
     CreateWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionSummaryTypeDef,
     CustomPluginDescriptionTypeDef,
     CustomPluginFileDescriptionTypeDef,
     S3LocationDescriptionTypeDef,
     S3LocationTypeDef,
     CustomPluginTypeDef,
     DeleteConnectorRequestRequestTypeDef,
+    DeleteConnectorResponseTypeDef,
     DeleteCustomPluginRequestRequestTypeDef,
+    DeleteCustomPluginResponseTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     StateDescriptionTypeDef,
     DescribeCustomPluginRequestRequestTypeDef,
     DescribeWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionDescriptionTypeDef,
     FirehoseLogDeliveryDescriptionTypeDef,
     FirehoseLogDeliveryTypeDef,
-    PaginatorConfigTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
+    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
     ListCustomPluginsRequestRequestTypeDef,
+    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     ListWorkerConfigurationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     S3LogDeliveryDescriptionTypeDef,
     S3LogDeliveryTypeDef,
+    UpdateConnectorResponseTypeDef,
     ApacheKafkaClusterDescriptionTypeDef,
     ApacheKafkaClusterTypeDef,
     AutoScalingDescriptionTypeDef,
     AutoScalingTypeDef,
     AutoScalingUpdateTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
-    DeleteConnectorResponseTypeDef,
-    DeleteCustomPluginResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     CreateWorkerConfigurationResponseTypeDef,
     WorkerConfigurationSummaryTypeDef,
     PluginDescriptionTypeDef,
     CustomPluginLocationDescriptionTypeDef,
     CustomPluginLocationTypeDef,
     PluginTypeDef,
     DescribeWorkerConfigurationResponseTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     WorkerLogDeliveryDescriptionTypeDef,
     WorkerLogDeliveryTypeDef,
     KafkaClusterDescriptionTypeDef,
     KafkaClusterTypeDef,
     CapacityDescriptionTypeDef,
     CapacityTypeDef,
     CapacityUpdateTypeDef,
@@ -431,42 +432,42 @@
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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/README.md` & `mypy-boto3-kafkaconnect-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kafkaconnect"></a>
 
 # mypy-boto3-kafkaconnect
 
 [![PyPI - mypy-boto3-kafkaconnect](https://img.shields.io/pypi/v/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafkaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KafkaConnect 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[boto3.KafkaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [mypy-boto3-kafkaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,57 +323,57 @@
     CloudWatchLogsLogDeliveryTypeDef,
     KafkaClusterClientAuthenticationDescriptionTypeDef,
     KafkaClusterEncryptionInTransitDescriptionTypeDef,
     WorkerConfigurationDescriptionTypeDef,
     KafkaClusterClientAuthenticationTypeDef,
     KafkaClusterEncryptionInTransitTypeDef,
     WorkerConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateCustomPluginResponseTypeDef,
     CreateWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionSummaryTypeDef,
     CustomPluginDescriptionTypeDef,
     CustomPluginFileDescriptionTypeDef,
     S3LocationDescriptionTypeDef,
     S3LocationTypeDef,
     CustomPluginTypeDef,
     DeleteConnectorRequestRequestTypeDef,
+    DeleteConnectorResponseTypeDef,
     DeleteCustomPluginRequestRequestTypeDef,
+    DeleteCustomPluginResponseTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     StateDescriptionTypeDef,
     DescribeCustomPluginRequestRequestTypeDef,
     DescribeWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionDescriptionTypeDef,
     FirehoseLogDeliveryDescriptionTypeDef,
     FirehoseLogDeliveryTypeDef,
-    PaginatorConfigTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
+    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
     ListCustomPluginsRequestRequestTypeDef,
+    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     ListWorkerConfigurationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     S3LogDeliveryDescriptionTypeDef,
     S3LogDeliveryTypeDef,
+    UpdateConnectorResponseTypeDef,
     ApacheKafkaClusterDescriptionTypeDef,
     ApacheKafkaClusterTypeDef,
     AutoScalingDescriptionTypeDef,
     AutoScalingTypeDef,
     AutoScalingUpdateTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
-    DeleteConnectorResponseTypeDef,
-    DeleteCustomPluginResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     CreateWorkerConfigurationResponseTypeDef,
     WorkerConfigurationSummaryTypeDef,
     PluginDescriptionTypeDef,
     CustomPluginLocationDescriptionTypeDef,
     CustomPluginLocationTypeDef,
     PluginTypeDef,
     DescribeWorkerConfigurationResponseTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     WorkerLogDeliveryDescriptionTypeDef,
     WorkerLogDeliveryTypeDef,
     KafkaClusterDescriptionTypeDef,
     KafkaClusterTypeDef,
     CapacityDescriptionTypeDef,
     CapacityTypeDef,
     CapacityUpdateTypeDef,
@@ -400,42 +400,42 @@
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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/__init__.py` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/__init__.pyi` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/__main__.py` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KafkaConnect 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.KafkaConnect 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect\nOther"
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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/client.py` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/client.pyi` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/literals.py` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,23 +58,25 @@
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
@@ -84,30 +86,35 @@
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
@@ -133,14 +140,15 @@
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
@@ -185,51 +193,57 @@
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
@@ -242,14 +256,15 @@
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
@@ -261,28 +276,35 @@
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
@@ -291,14 +313,15 @@
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
@@ -309,55 +332,64 @@
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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/literals.pyi` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -56,23 +56,25 @@
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
@@ -82,30 +84,35 @@
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
@@ -131,14 +138,15 @@
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
@@ -183,51 +191,57 @@
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
@@ -240,14 +254,15 @@
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
@@ -259,28 +274,35 @@
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
@@ -289,14 +311,15 @@
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
@@ -307,55 +330,64 @@
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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/paginator.py` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,43 +54,43 @@
 class ListConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, connectorNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, connectorNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
         """
 
 
 class ListCustomPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
         """
 
 
 class ListWorkerConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkerConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/paginator.pyi` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,41 +51,41 @@
 class ListConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, connectorNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, connectorNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listconnectorspaginator)
         """
 
 class ListCustomPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListCustomPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listcustompluginspaginator)
         """
 
 class ListWorkerConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkerConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect.Paginator.ListWorkerConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/paginators/#listworkerconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/type_defs.py` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,57 +45,57 @@
     "CloudWatchLogsLogDeliveryTypeDef",
     "KafkaClusterClientAuthenticationDescriptionTypeDef",
     "KafkaClusterEncryptionInTransitDescriptionTypeDef",
     "WorkerConfigurationDescriptionTypeDef",
     "KafkaClusterClientAuthenticationTypeDef",
     "KafkaClusterEncryptionInTransitTypeDef",
     "WorkerConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateCustomPluginResponseTypeDef",
     "CreateWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionSummaryTypeDef",
     "CustomPluginDescriptionTypeDef",
     "CustomPluginFileDescriptionTypeDef",
     "S3LocationDescriptionTypeDef",
     "S3LocationTypeDef",
     "CustomPluginTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
+    "DeleteConnectorResponseTypeDef",
     "DeleteCustomPluginRequestRequestTypeDef",
+    "DeleteCustomPluginResponseTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "StateDescriptionTypeDef",
     "DescribeCustomPluginRequestRequestTypeDef",
     "DescribeWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionDescriptionTypeDef",
     "FirehoseLogDeliveryDescriptionTypeDef",
     "FirehoseLogDeliveryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListConnectorsRequestRequestTypeDef",
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
     "ListCustomPluginsRequestRequestTypeDef",
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "ListWorkerConfigurationsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "S3LogDeliveryDescriptionTypeDef",
     "S3LogDeliveryTypeDef",
+    "UpdateConnectorResponseTypeDef",
     "ApacheKafkaClusterDescriptionTypeDef",
     "ApacheKafkaClusterTypeDef",
     "AutoScalingDescriptionTypeDef",
     "AutoScalingTypeDef",
     "AutoScalingUpdateTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateCustomPluginResponseTypeDef",
-    "DeleteConnectorResponseTypeDef",
-    "DeleteCustomPluginResponseTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "CreateWorkerConfigurationResponseTypeDef",
     "WorkerConfigurationSummaryTypeDef",
     "PluginDescriptionTypeDef",
     "CustomPluginLocationDescriptionTypeDef",
     "CustomPluginLocationTypeDef",
     "PluginTypeDef",
     "DescribeWorkerConfigurationResponseTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "WorkerLogDeliveryDescriptionTypeDef",
     "WorkerLogDeliveryTypeDef",
     "KafkaClusterDescriptionTypeDef",
     "KafkaClusterTypeDef",
     "CapacityDescriptionTypeDef",
     "CapacityTypeDef",
     "CapacityUpdateTypeDef",
@@ -284,22 +284,32 @@
     "WorkerConfigurationTypeDef",
     {
         "revision": int,
         "workerConfigurationArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "connectorArn": str,
+        "connectorName": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomPluginResponseTypeDef = TypedDict(
+    "CreateCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "name": str,
+        "revision": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerConfigurationRequestRequestTypeDef",
     {
         "name": str,
@@ -405,21 +415,39 @@
 
 class DeleteConnectorRequestRequestTypeDef(
     _RequiredDeleteConnectorRequestRequestTypeDef, _OptionalDeleteConnectorRequestRequestTypeDef
 ):
     pass
 
 
+DeleteConnectorResponseTypeDef = TypedDict(
+    "DeleteConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCustomPluginRequestRequestTypeDef = TypedDict(
     "DeleteCustomPluginRequestRequestTypeDef",
     {
         "customPluginArn": str,
     },
 )
 
+DeleteCustomPluginResponseTypeDef = TypedDict(
+    "DeleteCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeConnectorRequestRequestTypeDef = TypedDict(
     "DescribeConnectorRequestRequestTypeDef",
     {
         "connectorArn": str,
     },
 )
 
@@ -483,52 +511,88 @@
 
 class FirehoseLogDeliveryTypeDef(
     _RequiredFirehoseLogDeliveryTypeDef, _OptionalFirehoseLogDeliveryTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "connectorNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "connectorNamePrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCustomPluginsRequestRequestTypeDef = TypedDict(
     "ListCustomPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorkerConfigurationsRequestRequestTypeDef = TypedDict(
     "ListWorkerConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
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
 S3LogDeliveryDescriptionTypeDef = TypedDict(
     "S3LogDeliveryDescriptionTypeDef",
     {
         "bucket": str,
         "enabled": bool,
         "prefix": str,
     },
@@ -551,14 +615,23 @@
 )
 
 
 class S3LogDeliveryTypeDef(_RequiredS3LogDeliveryTypeDef, _OptionalS3LogDeliveryTypeDef):
     pass
 
 
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ApacheKafkaClusterDescriptionTypeDef = TypedDict(
     "ApacheKafkaClusterDescriptionTypeDef",
     {
         "bootstrapServers": str,
         "vpc": VpcDescriptionTypeDef,
     },
     total=False,
@@ -613,70 +686,22 @@
         "mcuCount": int,
         "minWorkerCount": int,
         "scaleInPolicy": ScaleInPolicyUpdateTypeDef,
         "scaleOutPolicy": ScaleOutPolicyUpdateTypeDef,
     },
 )
 
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorName": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomPluginResponseTypeDef = TypedDict(
-    "CreateCustomPluginResponseTypeDef",
-    {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "name": str,
-        "revision": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteConnectorResponseTypeDef = TypedDict(
-    "DeleteConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomPluginResponseTypeDef = TypedDict(
-    "DeleteCustomPluginResponseTypeDef",
-    {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWorkerConfigurationResponseTypeDef = TypedDict(
     "CreateWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "latestRevision": WorkerConfigurationRevisionSummaryTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkerConfigurationSummaryTypeDef = TypedDict(
     "WorkerConfigurationSummaryTypeDef",
     {
         "creationTime": datetime,
@@ -722,43 +747,18 @@
     "DescribeWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "description": str,
         "latestRevision": WorkerConfigurationRevisionDescriptionTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    {
-        "connectorNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 WorkerLogDeliveryDescriptionTypeDef = TypedDict(
     "WorkerLogDeliveryDescriptionTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsLogDeliveryDescriptionTypeDef,
         "firehose": FirehoseLogDeliveryDescriptionTypeDef,
         "s3": S3LogDeliveryDescriptionTypeDef,
     },
@@ -818,15 +818,15 @@
 )
 
 ListWorkerConfigurationsResponseTypeDef = TypedDict(
     "ListWorkerConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "workerConfigurations": List[WorkerConfigurationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomPluginRevisionSummaryTypeDef = TypedDict(
     "CustomPluginRevisionSummaryTypeDef",
     {
         "contentType": CustomPluginContentTypeType,
@@ -906,15 +906,15 @@
         "creationTime": datetime,
         "customPluginArn": str,
         "customPluginState": CustomPluginStateType,
         "description": str,
         "latestRevision": CustomPluginRevisionSummaryTypeDef,
         "name": str,
         "stateDescription": StateDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectorSummaryTypeDef = TypedDict(
     "ConnectorSummaryTypeDef",
     {
         "capacity": CapacityDescriptionTypeDef,
@@ -952,15 +952,15 @@
         "kafkaClusterEncryptionInTransit": KafkaClusterEncryptionInTransitDescriptionTypeDef,
         "kafkaConnectVersion": str,
         "logDelivery": LogDeliveryDescriptionTypeDef,
         "plugins": List[PluginDescriptionTypeDef],
         "serviceExecutionRoleArn": str,
         "stateDescription": StateDescriptionTypeDef,
         "workerConfiguration": WorkerConfigurationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorRequestRequestTypeDef",
     {
         "capacity": CapacityTypeDef,
@@ -992,19 +992,19 @@
 
 
 ListCustomPluginsResponseTypeDef = TypedDict(
     "ListCustomPluginsResponseTypeDef",
     {
         "customPlugins": List[CustomPluginSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect/type_defs.pyi` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,57 +44,57 @@
     "CloudWatchLogsLogDeliveryTypeDef",
     "KafkaClusterClientAuthenticationDescriptionTypeDef",
     "KafkaClusterEncryptionInTransitDescriptionTypeDef",
     "WorkerConfigurationDescriptionTypeDef",
     "KafkaClusterClientAuthenticationTypeDef",
     "KafkaClusterEncryptionInTransitTypeDef",
     "WorkerConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateCustomPluginResponseTypeDef",
     "CreateWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionSummaryTypeDef",
     "CustomPluginDescriptionTypeDef",
     "CustomPluginFileDescriptionTypeDef",
     "S3LocationDescriptionTypeDef",
     "S3LocationTypeDef",
     "CustomPluginTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
+    "DeleteConnectorResponseTypeDef",
     "DeleteCustomPluginRequestRequestTypeDef",
+    "DeleteCustomPluginResponseTypeDef",
     "DescribeConnectorRequestRequestTypeDef",
     "StateDescriptionTypeDef",
     "DescribeCustomPluginRequestRequestTypeDef",
     "DescribeWorkerConfigurationRequestRequestTypeDef",
     "WorkerConfigurationRevisionDescriptionTypeDef",
     "FirehoseLogDeliveryDescriptionTypeDef",
     "FirehoseLogDeliveryTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListConnectorsRequestRequestTypeDef",
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
     "ListCustomPluginsRequestRequestTypeDef",
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "ListWorkerConfigurationsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "S3LogDeliveryDescriptionTypeDef",
     "S3LogDeliveryTypeDef",
+    "UpdateConnectorResponseTypeDef",
     "ApacheKafkaClusterDescriptionTypeDef",
     "ApacheKafkaClusterTypeDef",
     "AutoScalingDescriptionTypeDef",
     "AutoScalingTypeDef",
     "AutoScalingUpdateTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateCustomPluginResponseTypeDef",
-    "DeleteConnectorResponseTypeDef",
-    "DeleteCustomPluginResponseTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "CreateWorkerConfigurationResponseTypeDef",
     "WorkerConfigurationSummaryTypeDef",
     "PluginDescriptionTypeDef",
     "CustomPluginLocationDescriptionTypeDef",
     "CustomPluginLocationTypeDef",
     "PluginTypeDef",
     "DescribeWorkerConfigurationResponseTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
     "WorkerLogDeliveryDescriptionTypeDef",
     "WorkerLogDeliveryTypeDef",
     "KafkaClusterDescriptionTypeDef",
     "KafkaClusterTypeDef",
     "CapacityDescriptionTypeDef",
     "CapacityTypeDef",
     "CapacityUpdateTypeDef",
@@ -279,22 +279,32 @@
     "WorkerConfigurationTypeDef",
     {
         "revision": int,
         "workerConfigurationArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "connectorArn": str,
+        "connectorName": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomPluginResponseTypeDef = TypedDict(
+    "CreateCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "name": str,
+        "revision": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerConfigurationRequestRequestTypeDef",
     {
         "name": str,
@@ -394,21 +404,39 @@
 )
 
 class DeleteConnectorRequestRequestTypeDef(
     _RequiredDeleteConnectorRequestRequestTypeDef, _OptionalDeleteConnectorRequestRequestTypeDef
 ):
     pass
 
+DeleteConnectorResponseTypeDef = TypedDict(
+    "DeleteConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCustomPluginRequestRequestTypeDef = TypedDict(
     "DeleteCustomPluginRequestRequestTypeDef",
     {
         "customPluginArn": str,
     },
 )
 
+DeleteCustomPluginResponseTypeDef = TypedDict(
+    "DeleteCustomPluginResponseTypeDef",
+    {
+        "customPluginArn": str,
+        "customPluginState": CustomPluginStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeConnectorRequestRequestTypeDef = TypedDict(
     "DescribeConnectorRequestRequestTypeDef",
     {
         "connectorArn": str,
     },
 )
 
@@ -470,52 +498,88 @@
 )
 
 class FirehoseLogDeliveryTypeDef(
     _RequiredFirehoseLogDeliveryTypeDef, _OptionalFirehoseLogDeliveryTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "connectorNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "connectorNamePrefix": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
+    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCustomPluginsRequestRequestTypeDef = TypedDict(
     "ListCustomPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
+    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorkerConfigurationsRequestRequestTypeDef = TypedDict(
     "ListWorkerConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
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
 S3LogDeliveryDescriptionTypeDef = TypedDict(
     "S3LogDeliveryDescriptionTypeDef",
     {
         "bucket": str,
         "enabled": bool,
         "prefix": str,
     },
@@ -536,14 +600,23 @@
     },
     total=False,
 )
 
 class S3LogDeliveryTypeDef(_RequiredS3LogDeliveryTypeDef, _OptionalS3LogDeliveryTypeDef):
     pass
 
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "connectorArn": str,
+        "connectorState": ConnectorStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ApacheKafkaClusterDescriptionTypeDef = TypedDict(
     "ApacheKafkaClusterDescriptionTypeDef",
     {
         "bootstrapServers": str,
         "vpc": VpcDescriptionTypeDef,
     },
     total=False,
@@ -596,70 +669,22 @@
         "mcuCount": int,
         "minWorkerCount": int,
         "scaleInPolicy": ScaleInPolicyUpdateTypeDef,
         "scaleOutPolicy": ScaleOutPolicyUpdateTypeDef,
     },
 )
 
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorName": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomPluginResponseTypeDef = TypedDict(
-    "CreateCustomPluginResponseTypeDef",
-    {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "name": str,
-        "revision": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteConnectorResponseTypeDef = TypedDict(
-    "DeleteConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomPluginResponseTypeDef = TypedDict(
-    "DeleteCustomPluginResponseTypeDef",
-    {
-        "customPluginArn": str,
-        "customPluginState": CustomPluginStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "connectorArn": str,
-        "connectorState": ConnectorStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWorkerConfigurationResponseTypeDef = TypedDict(
     "CreateWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "latestRevision": WorkerConfigurationRevisionSummaryTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkerConfigurationSummaryTypeDef = TypedDict(
     "WorkerConfigurationSummaryTypeDef",
     {
         "creationTime": datetime,
@@ -705,43 +730,18 @@
     "DescribeWorkerConfigurationResponseTypeDef",
     {
         "creationTime": datetime,
         "description": str,
         "latestRevision": WorkerConfigurationRevisionDescriptionTypeDef,
         "name": str,
         "workerConfigurationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    {
-        "connectorNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCustomPluginsRequestListCustomPluginsPaginateTypeDef = TypedDict(
-    "ListCustomPluginsRequestListCustomPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef = TypedDict(
-    "ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 WorkerLogDeliveryDescriptionTypeDef = TypedDict(
     "WorkerLogDeliveryDescriptionTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsLogDeliveryDescriptionTypeDef,
         "firehose": FirehoseLogDeliveryDescriptionTypeDef,
         "s3": S3LogDeliveryDescriptionTypeDef,
     },
@@ -801,15 +801,15 @@
 )
 
 ListWorkerConfigurationsResponseTypeDef = TypedDict(
     "ListWorkerConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "workerConfigurations": List[WorkerConfigurationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CustomPluginRevisionSummaryTypeDef = TypedDict(
     "CustomPluginRevisionSummaryTypeDef",
     {
         "contentType": CustomPluginContentTypeType,
@@ -887,15 +887,15 @@
         "creationTime": datetime,
         "customPluginArn": str,
         "customPluginState": CustomPluginStateType,
         "description": str,
         "latestRevision": CustomPluginRevisionSummaryTypeDef,
         "name": str,
         "stateDescription": StateDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConnectorSummaryTypeDef = TypedDict(
     "ConnectorSummaryTypeDef",
     {
         "capacity": CapacityDescriptionTypeDef,
@@ -933,15 +933,15 @@
         "kafkaClusterEncryptionInTransit": KafkaClusterEncryptionInTransitDescriptionTypeDef,
         "kafkaConnectVersion": str,
         "logDelivery": LogDeliveryDescriptionTypeDef,
         "plugins": List[PluginDescriptionTypeDef],
         "serviceExecutionRoleArn": str,
         "stateDescription": StateDescriptionTypeDef,
         "workerConfiguration": WorkerConfigurationDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectorRequestRequestTypeDef",
     {
         "capacity": CapacityTypeDef,
@@ -971,19 +971,19 @@
     pass
 
 ListCustomPluginsResponseTypeDef = TypedDict(
     "ListCustomPluginsResponseTypeDef",
     {
         "customPlugins": List[CustomPluginSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "connectors": List[ConnectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/PKG-INFO` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafkaconnect
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.KafkaConnect 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.KafkaConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/
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
 
 <a id="mypy-boto3-kafkaconnect"></a>
 
 # mypy-boto3-kafkaconnect
 
 [![PyPI - mypy-boto3-kafkaconnect](https://img.shields.io/pypi/v/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafkaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafkaconnect)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafkaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-kafkaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KafkaConnect 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
+[boto3.KafkaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
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
 [mypy-boto3-kafkaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,57 +355,57 @@
     CloudWatchLogsLogDeliveryTypeDef,
     KafkaClusterClientAuthenticationDescriptionTypeDef,
     KafkaClusterEncryptionInTransitDescriptionTypeDef,
     WorkerConfigurationDescriptionTypeDef,
     KafkaClusterClientAuthenticationTypeDef,
     KafkaClusterEncryptionInTransitTypeDef,
     WorkerConfigurationTypeDef,
-    ResponseMetadataTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateCustomPluginResponseTypeDef,
     CreateWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionSummaryTypeDef,
     CustomPluginDescriptionTypeDef,
     CustomPluginFileDescriptionTypeDef,
     S3LocationDescriptionTypeDef,
     S3LocationTypeDef,
     CustomPluginTypeDef,
     DeleteConnectorRequestRequestTypeDef,
+    DeleteConnectorResponseTypeDef,
     DeleteCustomPluginRequestRequestTypeDef,
+    DeleteCustomPluginResponseTypeDef,
     DescribeConnectorRequestRequestTypeDef,
     StateDescriptionTypeDef,
     DescribeCustomPluginRequestRequestTypeDef,
     DescribeWorkerConfigurationRequestRequestTypeDef,
     WorkerConfigurationRevisionDescriptionTypeDef,
     FirehoseLogDeliveryDescriptionTypeDef,
     FirehoseLogDeliveryTypeDef,
-    PaginatorConfigTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
+    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
     ListCustomPluginsRequestRequestTypeDef,
+    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     ListWorkerConfigurationsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     S3LogDeliveryDescriptionTypeDef,
     S3LogDeliveryTypeDef,
+    UpdateConnectorResponseTypeDef,
     ApacheKafkaClusterDescriptionTypeDef,
     ApacheKafkaClusterTypeDef,
     AutoScalingDescriptionTypeDef,
     AutoScalingTypeDef,
     AutoScalingUpdateTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateCustomPluginResponseTypeDef,
-    DeleteConnectorResponseTypeDef,
-    DeleteCustomPluginResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     CreateWorkerConfigurationResponseTypeDef,
     WorkerConfigurationSummaryTypeDef,
     PluginDescriptionTypeDef,
     CustomPluginLocationDescriptionTypeDef,
     CustomPluginLocationTypeDef,
     PluginTypeDef,
     DescribeWorkerConfigurationResponseTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
-    ListCustomPluginsRequestListCustomPluginsPaginateTypeDef,
-    ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef,
     WorkerLogDeliveryDescriptionTypeDef,
     WorkerLogDeliveryTypeDef,
     KafkaClusterDescriptionTypeDef,
     KafkaClusterTypeDef,
     CapacityDescriptionTypeDef,
     CapacityTypeDef,
     CapacityUpdateTypeDef,
@@ -431,42 +432,42 @@
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

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt` & `mypy-boto3-kafkaconnect-1.27.0/mypy_boto3_kafkaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafkaconnect-1.26.0.post1/setup.py` & `mypy-boto3-kafkaconnect-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-kafkaconnect.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafkaconnect",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_kafkaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KafkaConnect 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.KafkaConnect 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
     keywords="boto3 kafkaconnect type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_kafkaconnect": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_kafkaconnect": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafkaconnect/",
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


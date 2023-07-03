# Comparing `tmp/mypy-boto3-kinesisvideo-1.26.33.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.26.33.tar", last modified: Mon Dec 19 20:27:39 2022, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.27.0.tar", last modified: Mon Jul  3 19:50:59 2023, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.26.33.tar` & `mypy-boto3-kinesisvideo-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23103 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23065 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25175 2022-12-19 20:26:51.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2022-12-19 20:26:51.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-19 20:27:39.000000 mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 20:27:39.495972 mypy-boto3-kinesisvideo-1.26.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-19 20:26:50.000000 mypy-boto3-kinesisvideo-1.26.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:59.751526 mypy-boto3-kinesisvideo-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-07-03 19:50:59.743526 mypy-boto3-kinesisvideo-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:59.743526 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28642 2023-07-03 19:40:29.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28603 2023-07-03 19:40:29.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:59.743526 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-07-03 19:50:59.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:59.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:59.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:59.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:59.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:59.000000 mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:59.751526 mypy-boto3-kinesisvideo-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:40:28.000000 mypy-boto3-kinesisvideo-1.27.0/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/LICENSE` & `mypy-boto3-kinesisvideo-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kinesisvideo-1.26.33/PKG-INFO` & `mypy-boto3-kinesisvideo-1.27.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.26.33
-Summary: Type annotations for boto3.KinesisVideo 1.26.33 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.KinesisVideo 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kinesisvideo"></a>
 
 # mypy-boto3-kinesisvideo
 
 [![PyPI - mypy-boto3-kinesisvideo](https://img.shields.io/pypi/v/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.26.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,25 +281,29 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kinesisvideo import KinesisVideoClient
 from mypy_boto3_kinesisvideo.paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 client: KinesisVideoClient = Session().client("kinesisvideo")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = (
     client.get_paginator("describe_mapped_resource_configuration")
 )
+list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = (
+    client.get_paginator("list_edge_agent_configurations")
+)
 list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
     "list_signaling_channels"
 )
 list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
@@ -317,22 +321,25 @@
     ChannelTypeType,
     ComparisonOperatorType,
     ConfigurationStatusType,
     DescribeMappedResourceConfigurationPaginatorName,
     FormatConfigKeyType,
     FormatType,
     ImageSelectorTypeType,
+    ListEdgeAgentConfigurationsPaginatorName,
     ListSignalingChannelsPaginatorName,
     ListStreamsPaginatorName,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
     KinesisVideoServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -349,63 +356,69 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSignalingChannelOutputTypeDef,
     CreateStreamInputRequestTypeDef,
+    CreateStreamOutputTypeDef,
+    DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
     MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
+    LastRecorderStatusTypeDef,
+    LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
+    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
+    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
+    ListTagsForStreamOutputTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
+    PaginatorConfigTypeDef,
     ScheduleConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    CreateSignalingChannelOutputTypeDef,
-    CreateStreamOutputTypeDef,
-    GetDataEndpointOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
     UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
+    EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
@@ -414,58 +427,60 @@
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsEdgeConfigTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
 def get_structure() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-kinesisvideo-1.26.33/README.md` & `mypy-boto3-kinesisvideo-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kinesisvideo"></a>
 
 # mypy-boto3-kinesisvideo
 
 [![PyPI - mypy-boto3-kinesisvideo](https://img.shields.io/pypi/v/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.26.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,25 +249,29 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kinesisvideo import KinesisVideoClient
 from mypy_boto3_kinesisvideo.paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 client: KinesisVideoClient = Session().client("kinesisvideo")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = (
     client.get_paginator("describe_mapped_resource_configuration")
 )
+list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = (
+    client.get_paginator("list_edge_agent_configurations")
+)
 list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
     "list_signaling_channels"
 )
 list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
@@ -285,22 +289,25 @@
     ChannelTypeType,
     ComparisonOperatorType,
     ConfigurationStatusType,
     DescribeMappedResourceConfigurationPaginatorName,
     FormatConfigKeyType,
     FormatType,
     ImageSelectorTypeType,
+    ListEdgeAgentConfigurationsPaginatorName,
     ListSignalingChannelsPaginatorName,
     ListStreamsPaginatorName,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
     KinesisVideoServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -317,63 +324,69 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSignalingChannelOutputTypeDef,
     CreateStreamInputRequestTypeDef,
+    CreateStreamOutputTypeDef,
+    DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
     MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
+    LastRecorderStatusTypeDef,
+    LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
+    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
+    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
+    ListTagsForStreamOutputTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
+    PaginatorConfigTypeDef,
     ScheduleConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    CreateSignalingChannelOutputTypeDef,
-    CreateStreamOutputTypeDef,
-    GetDataEndpointOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
     UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
+    EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
@@ -382,58 +395,60 @@
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsEdgeConfigTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
 def get_structure() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__init__.py` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -5,36 +5,39 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_kinesisvideo import (
         Client,
         DescribeMappedResourceConfigurationPaginator,
         KinesisVideoClient,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
 
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from .client import KinesisVideoClient
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 Client = KinesisVideoClient
 
-
 __all__ = (
     "Client",
     "DescribeMappedResourceConfigurationPaginator",
     "KinesisVideoClient",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__init__.pyi` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,40 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_kinesisvideo import (
         Client,
         DescribeMappedResourceConfigurationPaginator,
         KinesisVideoClient,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
 
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from .client import KinesisVideoClient
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 Client = KinesisVideoClient
 
+
 __all__ = (
     "Client",
     "DescribeMappedResourceConfigurationPaginator",
     "KinesisVideoClient",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.26.33\nVersion:         1.26.33\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.KinesisVideo 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.33")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     ChannelNameConditionTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
@@ -35,14 +36,15 @@
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
@@ -53,26 +55,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KinesisVideoClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AccountChannelLimitExceededException: Type[BotocoreClientError]
     AccountStreamLimitExceededException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientLimitExceededException: Type[BotocoreClientError]
     DeviceStreamLimitExceededException: Type[BotocoreClientError]
@@ -83,15 +82,14 @@
     NotAuthorizedException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     StreamEdgeConfigurationNotFoundException: Type[BotocoreClientError]
     TagsPerResourceExceededLimitException: Type[BotocoreClientError]
     VersionMismatchException: Type[BotocoreClientError]
 
-
 class KinesisVideoClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/)
     """
 
     meta: ClientMeta
@@ -100,46 +98,42 @@
     def exceptions(self) -> Exceptions:
         """
         KinesisVideoClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#close)
         """
-
     def create_signaling_channel(
         self,
         *,
         ChannelName: str,
         ChannelType: ChannelTypeType = ...,
         SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalingChannelOutputTypeDef:
         """
         Creates a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#create_signaling_channel)
         """
-
     def create_stream(
         self,
         *,
         StreamName: str,
         DeviceName: str = ...,
         MediaType: str = ...,
         KmsKeyId: str = ...,
@@ -148,241 +142,240 @@
     ) -> CreateStreamOutputTypeDef:
         """
         Creates a new Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#create_stream)
         """
+    def delete_edge_configuration(
+        self, *, StreamName: str = ..., StreamARN: str = ...
+    ) -> Dict[str, Any]:
+        """
+        An asynchronous API that deletes a stream’s existing edge configuration, as well
+        as the corresponding media from the Edge Agent.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_edge_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#delete_edge_configuration)
+        """
     def delete_signaling_channel(
         self, *, ChannelARN: str, CurrentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a specified signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#delete_signaling_channel)
         """
-
     def delete_stream(self, *, StreamARN: str, CurrentVersion: str = ...) -> Dict[str, Any]:
         """
         Deletes a Kinesis video stream and the data contained in the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#delete_stream)
         """
-
     def describe_edge_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeEdgeConfigurationOutputTypeDef:
         """
         Describes a stream’s edge configuration that was set using the
-        `StartEdgeConfigurationUpdate` API.
+        `StartEdgeConfigurationUpdate` API and the latest status of the edge agent's
+        recorder and uploader jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_edge_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_edge_configuration)
         """
-
     def describe_image_generation_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeImageGenerationConfigurationOutputTypeDef:
         """
         Gets the `ImageGenerationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_image_generation_configuration)
         """
-
     def describe_mapped_resource_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMappedResourceConfigurationOutputTypeDef:
         """
         Returns the most current information about the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_mapped_resource_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_mapped_resource_configuration)
         """
-
     def describe_media_storage_configuration(
         self, *, ChannelName: str = ..., ChannelARN: str = ...
     ) -> DescribeMediaStorageConfigurationOutputTypeDef:
         """
         Returns the most current information about the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_media_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_media_storage_configuration)
         """
-
     def describe_notification_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeNotificationConfigurationOutputTypeDef:
         """
         Gets the `NotificationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_notification_configuration)
         """
-
     def describe_signaling_channel(
         self, *, ChannelName: str = ..., ChannelARN: str = ...
     ) -> DescribeSignalingChannelOutputTypeDef:
         """
         Returns the most current information about the signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_signaling_channel)
         """
-
     def describe_stream(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeStreamOutputTypeDef:
         """
         Returns the most current information about the specified stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_stream)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#generate_presigned_url)
         """
-
     def get_data_endpoint(
         self, *, APIName: APINameType, StreamName: str = ..., StreamARN: str = ...
     ) -> GetDataEndpointOutputTypeDef:
         """
         Gets an endpoint for a specified stream for either reading or writing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_data_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_data_endpoint)
         """
-
     def get_signaling_channel_endpoint(
         self,
         *,
         ChannelARN: str,
         SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...
     ) -> GetSignalingChannelEndpointOutputTypeDef:
         """
         Provides an endpoint for the specified signaling channel to send and receive
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_signaling_channel_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_signaling_channel_endpoint)
         """
+    def list_edge_agent_configurations(
+        self, *, HubDeviceArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListEdgeAgentConfigurationsOutputTypeDef:
+        """
+        Returns an array of edge configurations associated with the specified Edge
+        Agent.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_edge_agent_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_edge_agent_configurations)
+        """
     def list_signaling_channels(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...
     ) -> ListSignalingChannelsOutputTypeDef:
         """
         Returns an array of `ChannelInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_signaling_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_signaling_channels)
         """
-
     def list_streams(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         StreamNameCondition: StreamNameConditionTypeDef = ...
     ) -> ListStreamsOutputTypeDef:
         """
         Returns an array of `StreamInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_streams)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_streams)
         """
-
     def list_tags_for_resource(
         self, *, ResourceARN: str, NextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         Returns a list of tags associated with the specified signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_tags_for_resource)
         """
-
     def list_tags_for_stream(
         self, *, NextToken: str = ..., StreamARN: str = ..., StreamName: str = ...
     ) -> ListTagsForStreamOutputTypeDef:
         """
         Returns a list of tags associated with the specified stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_tags_for_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_tags_for_stream)
         """
-
     def start_edge_configuration_update(
         self, *, EdgeConfig: EdgeConfigTypeDef, StreamName: str = ..., StreamARN: str = ...
     ) -> StartEdgeConfigurationUpdateOutputTypeDef:
         """
         An asynchronous API that updates a stream’s existing edge configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.start_edge_configuration_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#start_edge_configuration_update)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#tag_resource)
         """
-
     def tag_stream(
         self, *, Tags: Mapping[str, str], StreamARN: str = ..., StreamName: str = ...
     ) -> Dict[str, Any]:
         """
         Adds one or more tags to a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.tag_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#tag_stream)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeyList: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#untag_resource)
         """
-
     def untag_stream(
         self, *, TagKeyList: Sequence[str], StreamARN: str = ..., StreamName: str = ...
     ) -> Dict[str, Any]:
         """
         Removes one or more tags from a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.untag_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#untag_stream)
         """
-
     def update_data_retention(
         self,
         *,
         CurrentVersion: str,
         Operation: UpdateDataRetentionOperationType,
         DataRetentionChangeInHours: int,
         StreamName: str = ...,
@@ -391,67 +384,62 @@
         """
         Increases or decreases the stream's data retention period by the value that you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_data_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_data_retention)
         """
-
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
-
     def update_media_storage_configuration(
         self, *, ChannelARN: str, MediaStorageConfiguration: MediaStorageConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Associates a `SignalingChannel` to a stream to store the media.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_media_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_media_storage_configuration)
         """
-
     def update_notification_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the notification information for a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_notification_configuration)
         """
-
     def update_signaling_channel(
         self,
         *,
         ChannelARN: str,
         CurrentVersion: str,
         SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the existing signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_signaling_channel)
         """
-
     def update_stream(
         self,
         *,
         CurrentVersion: str,
         StreamName: str = ...,
         StreamARN: str = ...,
         DeviceName: str = ...,
@@ -459,32 +447,37 @@
     ) -> Dict[str, Any]:
         """
         Updates stream metadata, such as the device name and media type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_stream)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_mapped_resource_configuration"]
     ) -> DescribeMappedResourceConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
-
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_edge_agent_configurations"]
+    ) -> ListEdgeAgentConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
+        """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signaling_channels"]
     ) -> ListSignalingChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_streams"]) -> ListStreamsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import APINameType, ChannelTypeType, UpdateDataRetentionOperationType
 from .paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 from .type_defs import (
     ChannelNameConditionTypeDef,
     CreateSignalingChannelOutputTypeDef,
     CreateStreamOutputTypeDef,
@@ -35,14 +36,15 @@
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
@@ -53,23 +55,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("KinesisVideoClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AccountChannelLimitExceededException: Type[BotocoreClientError]
     AccountStreamLimitExceededException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientLimitExceededException: Type[BotocoreClientError]
     DeviceStreamLimitExceededException: Type[BotocoreClientError]
@@ -80,14 +85,15 @@
     NotAuthorizedException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     StreamEdgeConfigurationNotFoundException: Type[BotocoreClientError]
     TagsPerResourceExceededLimitException: Type[BotocoreClientError]
     VersionMismatchException: Type[BotocoreClientError]
 
+
 class KinesisVideoClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/)
     """
 
     meta: ClientMeta
@@ -96,42 +102,46 @@
     def exceptions(self) -> Exceptions:
         """
         KinesisVideoClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#close)
         """
+
     def create_signaling_channel(
         self,
         *,
         ChannelName: str,
         ChannelType: ChannelTypeType = ...,
         SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalingChannelOutputTypeDef:
         """
         Creates a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#create_signaling_channel)
         """
+
     def create_stream(
         self,
         *,
         StreamName: str,
         DeviceName: str = ...,
         MediaType: str = ...,
         KmsKeyId: str = ...,
@@ -140,219 +150,264 @@
     ) -> CreateStreamOutputTypeDef:
         """
         Creates a new Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.create_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#create_stream)
         """
+
+    def delete_edge_configuration(
+        self, *, StreamName: str = ..., StreamARN: str = ...
+    ) -> Dict[str, Any]:
+        """
+        An asynchronous API that deletes a stream’s existing edge configuration, as well
+        as the corresponding media from the Edge Agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_edge_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#delete_edge_configuration)
+        """
+
     def delete_signaling_channel(
         self, *, ChannelARN: str, CurrentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a specified signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#delete_signaling_channel)
         """
+
     def delete_stream(self, *, StreamARN: str, CurrentVersion: str = ...) -> Dict[str, Any]:
         """
         Deletes a Kinesis video stream and the data contained in the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.delete_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#delete_stream)
         """
+
     def describe_edge_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeEdgeConfigurationOutputTypeDef:
         """
         Describes a stream’s edge configuration that was set using the
-        `StartEdgeConfigurationUpdate` API.
+        `StartEdgeConfigurationUpdate` API and the latest status of the edge agent's
+        recorder and uploader jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_edge_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_edge_configuration)
         """
+
     def describe_image_generation_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeImageGenerationConfigurationOutputTypeDef:
         """
         Gets the `ImageGenerationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_image_generation_configuration)
         """
+
     def describe_mapped_resource_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMappedResourceConfigurationOutputTypeDef:
         """
         Returns the most current information about the stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_mapped_resource_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_mapped_resource_configuration)
         """
+
     def describe_media_storage_configuration(
         self, *, ChannelName: str = ..., ChannelARN: str = ...
     ) -> DescribeMediaStorageConfigurationOutputTypeDef:
         """
         Returns the most current information about the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_media_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_media_storage_configuration)
         """
+
     def describe_notification_configuration(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeNotificationConfigurationOutputTypeDef:
         """
         Gets the `NotificationConfiguration` for a given Kinesis video stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_notification_configuration)
         """
+
     def describe_signaling_channel(
         self, *, ChannelName: str = ..., ChannelARN: str = ...
     ) -> DescribeSignalingChannelOutputTypeDef:
         """
         Returns the most current information about the signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_signaling_channel)
         """
+
     def describe_stream(
         self, *, StreamName: str = ..., StreamARN: str = ...
     ) -> DescribeStreamOutputTypeDef:
         """
         Returns the most current information about the specified stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.describe_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#describe_stream)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#generate_presigned_url)
         """
+
     def get_data_endpoint(
         self, *, APIName: APINameType, StreamName: str = ..., StreamARN: str = ...
     ) -> GetDataEndpointOutputTypeDef:
         """
         Gets an endpoint for a specified stream for either reading or writing.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_data_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_data_endpoint)
         """
+
     def get_signaling_channel_endpoint(
         self,
         *,
         ChannelARN: str,
         SingleMasterChannelEndpointConfiguration: SingleMasterChannelEndpointConfigurationTypeDef = ...
     ) -> GetSignalingChannelEndpointOutputTypeDef:
         """
         Provides an endpoint for the specified signaling channel to send and receive
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_signaling_channel_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_signaling_channel_endpoint)
         """
+
+    def list_edge_agent_configurations(
+        self, *, HubDeviceArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListEdgeAgentConfigurationsOutputTypeDef:
+        """
+        Returns an array of edge configurations associated with the specified Edge
+        Agent.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_edge_agent_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_edge_agent_configurations)
+        """
+
     def list_signaling_channels(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...
     ) -> ListSignalingChannelsOutputTypeDef:
         """
         Returns an array of `ChannelInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_signaling_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_signaling_channels)
         """
+
     def list_streams(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         StreamNameCondition: StreamNameConditionTypeDef = ...
     ) -> ListStreamsOutputTypeDef:
         """
         Returns an array of `StreamInfo` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_streams)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_streams)
         """
+
     def list_tags_for_resource(
         self, *, ResourceARN: str, NextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         Returns a list of tags associated with the specified signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_tags_for_resource)
         """
+
     def list_tags_for_stream(
         self, *, NextToken: str = ..., StreamARN: str = ..., StreamName: str = ...
     ) -> ListTagsForStreamOutputTypeDef:
         """
         Returns a list of tags associated with the specified stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.list_tags_for_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#list_tags_for_stream)
         """
+
     def start_edge_configuration_update(
         self, *, EdgeConfig: EdgeConfigTypeDef, StreamName: str = ..., StreamARN: str = ...
     ) -> StartEdgeConfigurationUpdateOutputTypeDef:
         """
         An asynchronous API that updates a stream’s existing edge configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.start_edge_configuration_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#start_edge_configuration_update)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#tag_resource)
         """
+
     def tag_stream(
         self, *, Tags: Mapping[str, str], StreamARN: str = ..., StreamName: str = ...
     ) -> Dict[str, Any]:
         """
         Adds one or more tags to a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.tag_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#tag_stream)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeyList: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#untag_resource)
         """
+
     def untag_stream(
         self, *, TagKeyList: Sequence[str], StreamARN: str = ..., StreamName: str = ...
     ) -> Dict[str, Any]:
         """
         Removes one or more tags from a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.untag_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#untag_stream)
         """
+
     def update_data_retention(
         self,
         *,
         CurrentVersion: str,
         Operation: UpdateDataRetentionOperationType,
         DataRetentionChangeInHours: int,
         StreamName: str = ...,
@@ -361,62 +416,67 @@
         """
         Increases or decreases the stream's data retention period by the value that you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_data_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_data_retention)
         """
+
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
+
     def update_media_storage_configuration(
         self, *, ChannelARN: str, MediaStorageConfiguration: MediaStorageConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Associates a `SignalingChannel` to a stream to store the media.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_media_storage_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_media_storage_configuration)
         """
+
     def update_notification_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the notification information for a stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_notification_configuration)
         """
+
     def update_signaling_channel(
         self,
         *,
         ChannelARN: str,
         CurrentVersion: str,
         SingleMasterConfiguration: SingleMasterConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the existing signaling channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_signaling_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_signaling_channel)
         """
+
     def update_stream(
         self,
         *,
         CurrentVersion: str,
         StreamName: str = ...,
         StreamARN: str = ...,
         DeviceName: str = ...,
@@ -424,29 +484,41 @@
     ) -> Dict[str, Any]:
         """
         Updates stream metadata, such as the device name and media type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_stream)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_mapped_resource_configuration"]
     ) -> DescribeMappedResourceConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_edge_agent_configurations"]
+    ) -> ListEdgeAgentConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
+        """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signaling_channels"]
     ) -> ListSignalingChannelsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_streams"]) -> ListStreamsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,25 @@
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
     "DescribeMappedResourceConfigurationPaginatorName",
     "FormatConfigKeyType",
     "FormatType",
     "ImageSelectorTypeType",
+    "ListEdgeAgentConfigurationsPaginatorName",
     "ListSignalingChannelsPaginatorName",
     "ListStreamsPaginatorName",
     "MediaStorageConfigurationStatusType",
     "MediaUriTypeType",
+    "RecorderStatusType",
     "StatusType",
     "StrategyOnFullSizeType",
     "SyncStatusType",
     "UpdateDataRetentionOperationType",
+    "UploaderStatusType",
     "KinesisVideoServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -61,24 +64,33 @@
 ChannelTypeType = Literal["FULL_MESH", "SINGLE_MASTER"]
 ComparisonOperatorType = Literal["BEGINS_WITH"]
 ConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 DescribeMappedResourceConfigurationPaginatorName = Literal["describe_mapped_resource_configuration"]
 FormatConfigKeyType = Literal["JPEGQuality"]
 FormatType = Literal["JPEG", "PNG"]
 ImageSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
+ListEdgeAgentConfigurationsPaginatorName = Literal["list_edge_agent_configurations"]
 ListSignalingChannelsPaginatorName = Literal["list_signaling_channels"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MediaStorageConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 MediaUriTypeType = Literal["FILE_URI", "RTSP_URI"]
+RecorderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 StatusType = Literal["ACTIVE", "CREATING", "DELETING", "UPDATING"]
 StrategyOnFullSizeType = Literal["DELETE_OLDEST_MEDIA", "DENY_NEW_MEDIA"]
 SyncStatusType = Literal[
-    "ACKNOWLEDGED", "DELETE_FAILED", "DELETING", "IN_SYNC", "SYNCING", "SYNC_FAILED"
+    "ACKNOWLEDGED",
+    "DELETE_FAILED",
+    "DELETING",
+    "DELETING_ACKNOWLEDGED",
+    "IN_SYNC",
+    "SYNCING",
+    "SYNC_FAILED",
 ]
 UpdateDataRetentionOperationType = Literal["DECREASE_DATA_RETENTION", "INCREASE_DATA_RETENTION"]
+UploaderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 KinesisVideoServiceName = Literal["kinesisvideo"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -87,14 +99,15 @@
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
@@ -115,31 +128,34 @@
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
@@ -218,14 +234,15 @@
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
@@ -236,18 +253,20 @@
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
@@ -257,14 +276,15 @@
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
@@ -277,14 +297,15 @@
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
@@ -303,16 +324,19 @@
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
@@ -392,18 +416,21 @@
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
@@ -422,15 +449,18 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "describe_mapped_resource_configuration", "list_signaling_channels", "list_streams"
+    "describe_mapped_resource_configuration",
+    "list_edge_agent_configurations",
+    "list_signaling_channels",
+    "list_streams",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,25 @@
     "ChannelTypeType",
     "ComparisonOperatorType",
     "ConfigurationStatusType",
     "DescribeMappedResourceConfigurationPaginatorName",
     "FormatConfigKeyType",
     "FormatType",
     "ImageSelectorTypeType",
+    "ListEdgeAgentConfigurationsPaginatorName",
     "ListSignalingChannelsPaginatorName",
     "ListStreamsPaginatorName",
     "MediaStorageConfigurationStatusType",
     "MediaUriTypeType",
+    "RecorderStatusType",
     "StatusType",
     "StrategyOnFullSizeType",
     "SyncStatusType",
     "UpdateDataRetentionOperationType",
+    "UploaderStatusType",
     "KinesisVideoServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -59,24 +62,33 @@
 ChannelTypeType = Literal["FULL_MESH", "SINGLE_MASTER"]
 ComparisonOperatorType = Literal["BEGINS_WITH"]
 ConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 DescribeMappedResourceConfigurationPaginatorName = Literal["describe_mapped_resource_configuration"]
 FormatConfigKeyType = Literal["JPEGQuality"]
 FormatType = Literal["JPEG", "PNG"]
 ImageSelectorTypeType = Literal["PRODUCER_TIMESTAMP", "SERVER_TIMESTAMP"]
+ListEdgeAgentConfigurationsPaginatorName = Literal["list_edge_agent_configurations"]
 ListSignalingChannelsPaginatorName = Literal["list_signaling_channels"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MediaStorageConfigurationStatusType = Literal["DISABLED", "ENABLED"]
 MediaUriTypeType = Literal["FILE_URI", "RTSP_URI"]
+RecorderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 StatusType = Literal["ACTIVE", "CREATING", "DELETING", "UPDATING"]
 StrategyOnFullSizeType = Literal["DELETE_OLDEST_MEDIA", "DENY_NEW_MEDIA"]
 SyncStatusType = Literal[
-    "ACKNOWLEDGED", "DELETE_FAILED", "DELETING", "IN_SYNC", "SYNCING", "SYNC_FAILED"
+    "ACKNOWLEDGED",
+    "DELETE_FAILED",
+    "DELETING",
+    "DELETING_ACKNOWLEDGED",
+    "IN_SYNC",
+    "SYNCING",
+    "SYNC_FAILED",
 ]
 UpdateDataRetentionOperationType = Literal["DECREASE_DATA_RETENTION", "INCREASE_DATA_RETENTION"]
+UploaderStatusType = Literal["SUCCESS", "SYSTEM_ERROR", "USER_ERROR"]
 KinesisVideoServiceName = Literal["kinesisvideo"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -85,14 +97,15 @@
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
@@ -113,31 +126,34 @@
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
@@ -216,14 +232,15 @@
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
@@ -234,18 +251,20 @@
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
@@ -255,14 +274,15 @@
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
@@ -275,14 +295,15 @@
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
@@ -301,16 +322,19 @@
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
@@ -390,18 +414,21 @@
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
@@ -420,15 +447,18 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "describe_mapped_resource_configuration", "list_signaling_channels", "list_streams"
+    "describe_mapped_resource_configuration",
+    "list_edge_agent_configurations",
+    "list_signaling_channels",
+    "list_streams",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/paginator.py` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/paginator.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,41 +7,45 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kinesisvideo.client import KinesisVideoClient
     from mypy_boto3_kinesisvideo.paginator import (
         DescribeMappedResourceConfigurationPaginator,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
 
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ChannelNameConditionTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
 )
 
 __all__ = (
     "DescribeMappedResourceConfigurationPaginator",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -60,33 +64,48 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 
+class ListEdgeAgentConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+    """
+
+    def paginate(
+        self, *, HubDeviceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEdgeAgentConfigurationsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+        """
+
+
 class ListSignalingChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 
@@ -96,13 +115,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/paginator.pyi` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/paginator.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -7,41 +7,45 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kinesisvideo.client import KinesisVideoClient
     from mypy_boto3_kinesisvideo.paginator import (
         DescribeMappedResourceConfigurationPaginator,
+        ListEdgeAgentConfigurationsPaginator,
         ListSignalingChannelsPaginator,
         ListStreamsPaginator,
     )
 
     session = Session()
     client: KinesisVideoClient = session.client("kinesisvideo")
 
     describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = client.get_paginator("describe_mapped_resource_configuration")
+    list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = client.get_paginator("list_edge_agent_configurations")
     list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
     list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ChannelNameConditionTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     PaginatorConfigTypeDef,
     StreamNameConditionTypeDef,
 )
 
 __all__ = (
     "DescribeMappedResourceConfigurationPaginator",
+    "ListEdgeAgentConfigurationsPaginator",
     "ListSignalingChannelsPaginator",
     "ListStreamsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -57,32 +61,46 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
+class ListEdgeAgentConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+    """
+
+    def paginate(
+        self, *, HubDeviceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListEdgeAgentConfigurationsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListEdgeAgentConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listedgeagentconfigurationspaginator)
+        """
+
 class ListSignalingChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 class ListStreamsPaginator(Paginator):
@@ -91,13 +109,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,20 @@
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
     FormatType,
     ImageSelectorTypeType,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -41,63 +43,69 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateSignalingChannelOutputTypeDef",
     "CreateStreamInputRequestTypeDef",
+    "CreateStreamOutputTypeDef",
+    "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
     "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
+    "LastRecorderStatusTypeDef",
+    "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
+    "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
+    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
+    "ListTagsForStreamOutputTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ScheduleConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
     "UpdateSignalingChannelInputRequestTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListSignalingChannelsInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "CreateSignalingChannelOutputTypeDef",
-    "CreateStreamOutputTypeDef",
-    "GetDataEndpointOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
+    "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
@@ -106,16 +114,18 @@
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
+    "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
 SingleMasterConfigurationTypeDef = TypedDict(
     "SingleMasterConfigurationTypeDef",
     {
         "MessageTtlSeconds": int,
     },
@@ -135,22 +145,19 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSignalingChannelOutputTypeDef = TypedDict(
+    "CreateSignalingChannelOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChannelARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
@@ -171,14 +178,31 @@
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
 
+CreateStreamOutputTypeDef = TypedDict(
+    "CreateStreamOutputTypeDef",
+    {
+        "StreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
+    "DeleteEdgeConfigurationInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredDeleteSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalDeleteSignalingChannelInputRequestTypeDef = TypedDict(
@@ -241,20 +265,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     {
@@ -344,14 +368,36 @@
         "Status": StatusType,
         "CreationTime": datetime,
         "DataRetentionInHours": int,
     },
     total=False,
 )
 
+LastRecorderStatusTypeDef = TypedDict(
+    "LastRecorderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RecorderStatus": RecorderStatusType,
+    },
+    total=False,
+)
+
+LastUploaderStatusTypeDef = TypedDict(
+    "LastUploaderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "UploaderStatus": UploaderStatusType,
+    },
+    total=False,
+)
+
 _RequiredGetDataEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetDataEndpointInputRequestTypeDef",
     {
         "APIName": APINameType,
     },
 )
 _OptionalGetDataEndpointInputRequestTypeDef = TypedDict(
@@ -366,14 +412,22 @@
 
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
 
+GetDataEndpointOutputTypeDef = TypedDict(
+    "GetDataEndpointOutputTypeDef",
+    {
+        "DataEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -392,14 +446,59 @@
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
+_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListEdgeAgentConfigurationsInputRequestTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
+):
+    pass
+
+
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -422,24 +521,42 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
@@ -447,22 +564,43 @@
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
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
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
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
 _RequiredTagStreamInputRequestTypeDef = TypedDict(
     "_RequiredTagStreamInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
 )
 _OptionalTagStreamInputRequestTypeDef = TypedDict(
@@ -592,14 +730,23 @@
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
 
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSignalingChannelsInputRequestTypeDef = TypedDict(
     "ListSignalingChannelsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ChannelNameCondition": ChannelNameConditionTypeDef,
     },
@@ -634,99 +781,38 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateSignalingChannelOutputTypeDef = TypedDict(
-    "CreateSignalingChannelOutputTypeDef",
-    {
-        "ChannelARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStreamOutputTypeDef = TypedDict(
-    "CreateStreamOutputTypeDef",
-    {
-        "StreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataEndpointOutputTypeDef = TypedDict(
-    "GetDataEndpointOutputTypeDef",
-    {
-        "DataEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
-DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationOutputTypeDef",
     {
         "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
         "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     {
         "ChannelARN": str,
@@ -734,25 +820,34 @@
     },
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EdgeAgentStatusTypeDef = TypedDict(
+    "EdgeAgentStatusTypeDef",
+    {
+        "LastRecorderStatus": LastRecorderStatusTypeDef,
+        "LastUploaderStatus": LastUploaderStatusTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
@@ -773,15 +868,15 @@
     pass
 
 
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
@@ -808,15 +903,15 @@
     pass
 
 
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
@@ -861,32 +956,32 @@
     },
 )
 
 DescribeSignalingChannelOutputTypeDef = TypedDict(
     "DescribeSignalingChannelOutputTypeDef",
     {
         "ChannelInfo": ChannelInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSignalingChannelsOutputTypeDef = TypedDict(
     "ListSignalingChannelsOutputTypeDef",
     {
         "ChannelInfoList": List[ChannelInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -896,15 +991,15 @@
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -941,18 +1036,33 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EdgeAgentStatus": EdgeAgentStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -978,10 +1088,19 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsOutputTypeDef",
+    {
+        "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -21,18 +21,20 @@
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
     FormatType,
     ImageSelectorTypeType,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -40,63 +42,69 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateSignalingChannelOutputTypeDef",
     "CreateStreamInputRequestTypeDef",
+    "CreateStreamOutputTypeDef",
+    "DeleteEdgeConfigurationInputRequestTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
     "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
+    "LastRecorderStatusTypeDef",
+    "LastUploaderStatusTypeDef",
     "GetDataEndpointInputRequestTypeDef",
+    "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
+    "ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    "ListEdgeAgentConfigurationsInputRequestTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
+    "ListTagsForStreamOutputTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ScheduleConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
     "UpdateSignalingChannelInputRequestTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListSignalingChannelsInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "CreateSignalingChannelOutputTypeDef",
-    "CreateStreamOutputTypeDef",
-    "GetDataEndpointOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
+    "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
@@ -105,16 +113,18 @@
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
+    "ListEdgeAgentConfigurationsOutputTypeDef",
 )
 
 SingleMasterConfigurationTypeDef = TypedDict(
     "SingleMasterConfigurationTypeDef",
     {
         "MessageTtlSeconds": int,
     },
@@ -134,22 +144,19 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSignalingChannelOutputTypeDef = TypedDict(
+    "CreateSignalingChannelOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChannelARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
@@ -168,14 +175,31 @@
 )
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
+CreateStreamOutputTypeDef = TypedDict(
+    "CreateStreamOutputTypeDef",
+    {
+        "StreamARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
+    "DeleteEdgeConfigurationInputRequestTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+    },
+    total=False,
+)
+
 _RequiredDeleteSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredDeleteSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalDeleteSignalingChannelInputRequestTypeDef = TypedDict(
@@ -234,20 +258,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     {
@@ -335,14 +359,36 @@
         "Status": StatusType,
         "CreationTime": datetime,
         "DataRetentionInHours": int,
     },
     total=False,
 )
 
+LastRecorderStatusTypeDef = TypedDict(
+    "LastRecorderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RecorderStatus": RecorderStatusType,
+    },
+    total=False,
+)
+
+LastUploaderStatusTypeDef = TypedDict(
+    "LastUploaderStatusTypeDef",
+    {
+        "JobStatusDetails": str,
+        "LastCollectedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "UploaderStatus": UploaderStatusType,
+    },
+    total=False,
+)
+
 _RequiredGetDataEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetDataEndpointInputRequestTypeDef",
     {
         "APIName": APINameType,
     },
 )
 _OptionalGetDataEndpointInputRequestTypeDef = TypedDict(
@@ -355,14 +401,22 @@
 )
 
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
+GetDataEndpointOutputTypeDef = TypedDict(
+    "GetDataEndpointOutputTypeDef",
+    {
+        "DataEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -381,14 +435,55 @@
     "ImageGenerationDestinationConfigTypeDef",
     {
         "Uri": str,
         "DestinationRegion": str,
     },
 )
 
+_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_RequiredListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "HubDeviceArn": str,
+    },
+)
+_OptionalListEdgeAgentConfigurationsInputRequestTypeDef = TypedDict(
+    "_OptionalListEdgeAgentConfigurationsInputRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListEdgeAgentConfigurationsInputRequestTypeDef(
+    _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
+    _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
+):
+    pass
+
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -409,24 +504,42 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
@@ -434,22 +547,43 @@
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
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
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
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
 _RequiredTagStreamInputRequestTypeDef = TypedDict(
     "_RequiredTagStreamInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
 )
 _OptionalTagStreamInputRequestTypeDef = TypedDict(
@@ -569,14 +703,23 @@
 
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSignalingChannelsInputRequestTypeDef = TypedDict(
     "ListSignalingChannelsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ChannelNameCondition": ChannelNameConditionTypeDef,
     },
@@ -609,99 +752,38 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateSignalingChannelOutputTypeDef = TypedDict(
-    "CreateSignalingChannelOutputTypeDef",
-    {
-        "ChannelARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStreamOutputTypeDef = TypedDict(
-    "CreateStreamOutputTypeDef",
-    {
-        "StreamARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataEndpointOutputTypeDef = TypedDict(
-    "GetDataEndpointOutputTypeDef",
-    {
-        "DataEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
-DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationOutputTypeDef",
     {
         "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
         "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     {
         "ChannelARN": str,
@@ -709,25 +791,34 @@
     },
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EdgeAgentStatusTypeDef = TypedDict(
+    "EdgeAgentStatusTypeDef",
+    {
+        "LastRecorderStatus": LastRecorderStatusTypeDef,
+        "LastUploaderStatus": LastUploaderStatusTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
@@ -746,15 +837,15 @@
 ):
     pass
 
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
@@ -779,15 +870,15 @@
 ):
     pass
 
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
@@ -830,32 +921,32 @@
     },
 )
 
 DescribeSignalingChannelOutputTypeDef = TypedDict(
     "DescribeSignalingChannelOutputTypeDef",
     {
         "ChannelInfo": ChannelInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSignalingChannelsOutputTypeDef = TypedDict(
     "ListSignalingChannelsOutputTypeDef",
     {
         "ChannelInfoList": List[ChannelInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -865,15 +956,15 @@
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -908,18 +999,33 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EdgeAgentStatus": EdgeAgentStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListEdgeAgentConfigurationsEdgeConfigTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+        "SyncStatus": SyncStatusType,
+        "FailedStatusDetails": str,
+        "EdgeConfig": EdgeConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
     },
 )
 _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
@@ -943,10 +1049,19 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEdgeAgentConfigurationsOutputTypeDef = TypedDict(
+    "ListEdgeAgentConfigurationsOutputTypeDef",
+    {
+        "EdgeConfigs": List[ListEdgeAgentConfigurationsEdgeConfigTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/PKG-INFO` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisvideo
-Version: 1.26.33
-Summary: Type annotations for boto3.KinesisVideo 1.26.33 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.KinesisVideo 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kinesisvideo"></a>
 
 # mypy-boto3-kinesisvideo
 
 [![PyPI - mypy-boto3-kinesisvideo](https://img.shields.io/pypi/v/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesisvideo.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesisvideo)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesisvideo?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideo 1.26.33](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
+[boto3.KinesisVideo 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesisvideo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,25 +281,29 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kinesisvideo import KinesisVideoClient
 from mypy_boto3_kinesisvideo.paginator import (
     DescribeMappedResourceConfigurationPaginator,
+    ListEdgeAgentConfigurationsPaginator,
     ListSignalingChannelsPaginator,
     ListStreamsPaginator,
 )
 
 client: KinesisVideoClient = Session().client("kinesisvideo")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_mapped_resource_configuration_paginator: DescribeMappedResourceConfigurationPaginator = (
     client.get_paginator("describe_mapped_resource_configuration")
 )
+list_edge_agent_configurations_paginator: ListEdgeAgentConfigurationsPaginator = (
+    client.get_paginator("list_edge_agent_configurations")
+)
 list_signaling_channels_paginator: ListSignalingChannelsPaginator = client.get_paginator(
     "list_signaling_channels"
 )
 list_streams_paginator: ListStreamsPaginator = client.get_paginator("list_streams")
 ```
 
 <a id="literals"></a>
@@ -317,22 +321,25 @@
     ChannelTypeType,
     ComparisonOperatorType,
     ConfigurationStatusType,
     DescribeMappedResourceConfigurationPaginatorName,
     FormatConfigKeyType,
     FormatType,
     ImageSelectorTypeType,
+    ListEdgeAgentConfigurationsPaginatorName,
     ListSignalingChannelsPaginatorName,
     ListStreamsPaginatorName,
     MediaStorageConfigurationStatusType,
     MediaUriTypeType,
+    RecorderStatusType,
     StatusType,
     StrategyOnFullSizeType,
     SyncStatusType,
     UpdateDataRetentionOperationType,
+    UploaderStatusType,
     KinesisVideoServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -349,63 +356,69 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateSignalingChannelOutputTypeDef,
     CreateStreamInputRequestTypeDef,
+    CreateStreamOutputTypeDef,
+    DeleteEdgeConfigurationInputRequestTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
     MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
+    LastRecorderStatusTypeDef,
+    LastUploaderStatusTypeDef,
     GetDataEndpointInputRequestTypeDef,
+    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
+    ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
+    ListEdgeAgentConfigurationsInputRequestTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
+    ListTagsForStreamOutputTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
+    PaginatorConfigTypeDef,
     ScheduleConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
-    CreateSignalingChannelOutputTypeDef,
-    CreateStreamOutputTypeDef,
-    GetDataEndpointOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
     UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
+    EdgeAgentStatusTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
@@ -414,58 +427,60 @@
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
+    ListEdgeAgentConfigurationsEdgeConfigTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
+    ListEdgeAgentConfigurationsOutputTypeDef,
 )
 
 
 def get_structure() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-kinesisvideo-1.26.33/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.27.0/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.26.33/setup.py` & `mypy-boto3-kinesisvideo-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-kinesisvideo.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.26.33",
+    version="1.27.0",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideo 1.26.33 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.KinesisVideo 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/",
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


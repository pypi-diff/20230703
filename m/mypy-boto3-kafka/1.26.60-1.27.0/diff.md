# Comparing `tmp/mypy-boto3-kafka-1.26.60.tar.gz` & `tmp/mypy-boto3-kafka-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafka-1.26.60.tar", last modified: Mon Jan 30 21:06:23 2023, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
```

## Comparing `mypy-boto3-kafka-1.26.60.tar` & `mypy-boto3-kafka-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.542472 mypy-boto3-kafka-1.26.60/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-01-30 21:06:23.538471 mypy-boto3-kafka-1.26.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17383 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.534471 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45275 2023-01-30 21:06:02.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.538471 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18862 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 21:06:23.000000 mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:06:23.542472 mypy-boto3-kafka-1.26.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-30 21:06:01.000000 mypy-boto3-kafka-1.26.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.107478 mypy-boto3-kafka-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-07-03 19:50:57.107478 mypy-boto3-kafka-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.103478 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34814 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55042 2023-07-03 19:40:07.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54973 2023-07-03 19:40:07.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:06.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.107478 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-07-03 19:50:56.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:50:56.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:56.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:56.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:50:56.000000 mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:57.107478 mypy-boto3-kafka-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:40:05.000000 mypy-boto3-kafka-1.27.0/setup.py
```

### Comparing `mypy-boto3-kafka-1.26.60/LICENSE` & `mypy-boto3-kafka-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kafka-1.26.60/PKG-INFO` & `mypy-boto3-kafka-1.27.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.26.60
-Summary: Type annotations for boto3.Kafka 1.26.60 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Kafka 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,28 +279,33 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 
 client: KafkaClient = Session().client("kafka")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
+    "list_client_vpc_connections"
+)
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
@@ -309,14 +314,17 @@
     "list_configurations"
 )
 list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator(
     "list_kafka_versions"
 )
 list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
 list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator(
+    "list_vpc_connections"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kafka.literals` module contains literals extracted from shapes that
@@ -327,24 +335,28 @@
     BrokerAZDistributionType,
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
+    ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
+    ListVpcConnectionsPaginatorName,
     NodeTypeType,
     StorageModeType,
+    UserIdentityTypeType,
+    VpcConnectionStateType,
     KafkaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -359,135 +371,163 @@
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
+    ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
+    CreateClusterResponseTypeDef,
+    CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
+    CreateVpcConnectionRequestRequestTypeDef,
+    CreateVpcConnectionResponseTypeDef,
+    DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
+    DeleteClusterResponseTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
+    DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionRequestRequestTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionRequestRequestTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionAtRestTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
+    GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyRequestRequestTypeDef,
+    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
     IamTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
-    PaginatorConfigTypeDef,
+    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    ListClientVpcConnectionsRequestRequestTypeDef,
+    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListClustersV2RequestRequestTypeDef,
+    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
+    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListConfigurationsRequestRequestTypeDef,
+    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
+    ListNodesRequestListNodesPaginateTypeDef,
     ListNodesRequestRequestTypeDef,
+    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
     ListScramSecretsRequestRequestTypeDef,
+    ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
+    ListVpcConnectionsRequestRequestTypeDef,
+    VpcConnectionTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
+    PaginatorConfigTypeDef,
+    PutClusterPolicyRequestRequestTypeDef,
+    PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
+    RebootBrokerResponseTypeDef,
+    RejectClientVpcConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
-    UpdateBrokerTypeRequestRequestTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
-    CreateClusterResponseTypeDef,
-    CreateClusterV2ResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DeleteConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBootstrapBrokersResponseTypeDef,
-    ListScramSecretsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
+    UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
+    UserIdentityTypeDef,
+    VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamTypeDef,
+    VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
+    ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
-    ConnectivityInfoTypeDef,
     EncryptionInfoTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
-    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListClustersV2RequestListClustersV2PaginateTypeDef,
-    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
-    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
-    ListNodesRequestListNodesPaginateTypeDef,
-    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
     SaslTypeDef,
+    VpcConnectionInfoTypeDef,
+    VpcConnectivitySaslTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
-    UpdateConnectivityRequestRequestTypeDef,
     ServerlessClientAuthenticationTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationTypeDef,
-    BrokerNodeGroupInfoTypeDef,
+    VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
-    MutableClusterInfoTypeDef,
     UpdateSecurityRequestRequestTypeDef,
+    VpcConnectivityTypeDef,
+    ConnectivityInfoTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    MutableClusterInfoTypeDef,
+    UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
@@ -507,42 +547,42 @@
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

### Comparing `mypy-boto3-kafka-1.26.60/README.md` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kafka
+Version: 1.27.0
+Summary: Type annotations for boto3.Kafka 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -247,28 +279,33 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 
 client: KafkaClient = Session().client("kafka")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
+    "list_client_vpc_connections"
+)
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
@@ -277,14 +314,17 @@
     "list_configurations"
 )
 list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator(
     "list_kafka_versions"
 )
 list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
 list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator(
+    "list_vpc_connections"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kafka.literals` module contains literals extracted from shapes that
@@ -295,24 +335,28 @@
     BrokerAZDistributionType,
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
+    ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
+    ListVpcConnectionsPaginatorName,
     NodeTypeType,
     StorageModeType,
+    UserIdentityTypeType,
+    VpcConnectionStateType,
     KafkaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -327,135 +371,163 @@
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
+    ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
+    CreateClusterResponseTypeDef,
+    CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
+    CreateVpcConnectionRequestRequestTypeDef,
+    CreateVpcConnectionResponseTypeDef,
+    DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
+    DeleteClusterResponseTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
+    DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionRequestRequestTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionRequestRequestTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionAtRestTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
+    GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyRequestRequestTypeDef,
+    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
     IamTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
-    PaginatorConfigTypeDef,
+    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    ListClientVpcConnectionsRequestRequestTypeDef,
+    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListClustersV2RequestRequestTypeDef,
+    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
+    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListConfigurationsRequestRequestTypeDef,
+    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
+    ListNodesRequestListNodesPaginateTypeDef,
     ListNodesRequestRequestTypeDef,
+    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
     ListScramSecretsRequestRequestTypeDef,
+    ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
+    ListVpcConnectionsRequestRequestTypeDef,
+    VpcConnectionTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
+    PaginatorConfigTypeDef,
+    PutClusterPolicyRequestRequestTypeDef,
+    PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
+    RebootBrokerResponseTypeDef,
+    RejectClientVpcConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
-    UpdateBrokerTypeRequestRequestTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
-    CreateClusterResponseTypeDef,
-    CreateClusterV2ResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DeleteConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBootstrapBrokersResponseTypeDef,
-    ListScramSecretsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
+    UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
+    UserIdentityTypeDef,
+    VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamTypeDef,
+    VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
+    ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
-    ConnectivityInfoTypeDef,
     EncryptionInfoTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
-    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListClustersV2RequestListClustersV2PaginateTypeDef,
-    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
-    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
-    ListNodesRequestListNodesPaginateTypeDef,
-    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
     SaslTypeDef,
+    VpcConnectionInfoTypeDef,
+    VpcConnectivitySaslTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
-    UpdateConnectivityRequestRequestTypeDef,
     ServerlessClientAuthenticationTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationTypeDef,
-    BrokerNodeGroupInfoTypeDef,
+    VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
-    MutableClusterInfoTypeDef,
     UpdateSecurityRequestRequestTypeDef,
+    VpcConnectivityTypeDef,
+    ConnectivityInfoTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    MutableClusterInfoTypeDef,
+    UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
@@ -475,42 +547,42 @@
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

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,57 +4,65 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_kafka import (
         Client,
         KafkaClient,
+        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
+        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
+    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 
 Client = KafkaClient
 
 
 __all__ = (
     "Client",
     "KafkaClient",
+    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
+    "ListVpcConnectionsPaginator",
 )
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,56 +4,64 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_kafka import (
         Client,
         KafkaClient,
+        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
+        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
+    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from .client import KafkaClient
 from .paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 
 Client = KafkaClient
 
 __all__ = (
     "Client",
     "KafkaClient",
+    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
+    "ListVpcConnectionsPaginator",
 )
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.26.60\nVersion:         1.26.60\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Kafka 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.60")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,58 +17,67 @@
 from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
     ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
+    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
+    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     LoggingInfoTypeDef,
     OpenMonitoringInfoTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedThroughputTypeDef,
+    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     ServerlessRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
@@ -210,33 +219,67 @@
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_configuration)
         """
 
+    def create_vpc_connection(
+        self,
+        *,
+        TargetClusterArn: str,
+        Authentication: str,
+        VpcId: str,
+        ClientSubnets: Sequence[str],
+        SecurityGroups: Sequence[str],
+        Tags: Mapping[str, str] = ...
+    ) -> CreateVpcConnectionResponseTypeDef:
+        """
+        Creates a new MSK VPC connection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_vpc_connection)
+        """
+
     def delete_cluster(
         self, *, ClusterArn: str, CurrentVersion: str = ...
     ) -> DeleteClusterResponseTypeDef:
         """
         Deletes the MSK cluster specified by the Amazon Resource Name (ARN) in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster)
         """
 
+    def delete_cluster_policy(self, *, ClusterArn: str) -> Dict[str, Any]:
+        """
+        Deletes the MSK cluster policy specified by the Amazon Resource Name (ARN) in
+        the request.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster_policy)
+        """
+
     def delete_configuration(self, *, Arn: str) -> DeleteConfigurationResponseTypeDef:
         """
         Deletes an MSK Configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_configuration)
         """
 
+    def delete_vpc_connection(self, *, Arn: str) -> DeleteVpcConnectionResponseTypeDef:
+        """
+        Deletes a MSK VPC connection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_vpc_connection)
+        """
+
     def describe_cluster(self, *, ClusterArn: str) -> DescribeClusterResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster)
@@ -275,14 +318,22 @@
         """
         Returns a description of this revision of the configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_configuration_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_configuration_revision)
         """
 
+    def describe_vpc_connection(self, *, Arn: str) -> DescribeVpcConnectionResponseTypeDef:
+        """
+        Returns a description of this MSK VPC connection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_vpc_connection)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -297,24 +348,43 @@
         """
         A list of brokers that a client application can use to bootstrap.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_bootstrap_brokers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_bootstrap_brokers)
         """
 
+    def get_cluster_policy(self, *, ClusterArn: str) -> GetClusterPolicyResponseTypeDef:
+        """
+        Get the MSK cluster policy specified by the Amazon Resource Name (ARN) in the
+        request.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_cluster_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_cluster_policy)
+        """
+
     def get_compatible_kafka_versions(
         self, *, ClusterArn: str = ...
     ) -> GetCompatibleKafkaVersionsResponseTypeDef:
         """
         Gets the Apache Kafka versions to which you can update the MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_compatible_kafka_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_compatible_kafka_versions)
         """
 
+    def list_client_vpc_connections(
+        self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListClientVpcConnectionsResponseTypeDef:
+        """
+        Returns a list of all the VPC connections in this Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_client_vpc_connections)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_client_vpc_connections)
+        """
+
     def list_cluster_operations(
         self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListClusterOperationsResponseTypeDef:
         """
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
@@ -401,24 +471,55 @@
         """
         Returns a list of the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_tags_for_resource)
         """
 
+    def list_vpc_connections(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListVpcConnectionsResponseTypeDef:
+        """
+        Returns a list of all the VPC connections in this Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_vpc_connections)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_vpc_connections)
+        """
+
+    def put_cluster_policy(
+        self, *, ClusterArn: str, Policy: str, CurrentVersion: str = ...
+    ) -> PutClusterPolicyResponseTypeDef:
+        """
+        Creates or updates the MSK cluster policy specified by the cluster Amazon
+        Resource Name (ARN) in the request.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.put_cluster_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#put_cluster_policy)
+        """
+
     def reboot_broker(
         self, *, BrokerIds: Sequence[str], ClusterArn: str
     ) -> RebootBrokerResponseTypeDef:
         """
         Reboots brokers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reboot_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reboot_broker)
         """
 
+    def reject_client_vpc_connection(
+        self, *, ClusterArn: str, VpcConnectionArn: str
+    ) -> Dict[str, Any]:
+        """
+        Returns empty response.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reject_client_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reject_client_vpc_connection)
+        """
+
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to the specified MSK resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.tag_resource)
@@ -564,14 +665,23 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_storage)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_client_vpc_connections"]
+    ) -> ListClientVpcConnectionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_cluster_operations"]
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
 
@@ -627,7 +737,16 @@
     def get_paginator(
         self, operation_name: Literal["list_scram_secrets"]
     ) -> ListScramSecretsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_vpc_connections"]
+    ) -> ListVpcConnectionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -17,58 +17,67 @@
 from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import EnhancedMonitoringType, StorageModeType
 from .paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     BrokerNodeGroupInfoTypeDef,
     ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
+    CreateVpcConnectionResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeClusterV2ResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionInfoTypeDef,
     GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
+    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     LoggingInfoTypeDef,
     OpenMonitoringInfoTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedThroughputTypeDef,
+    PutClusterPolicyResponseTypeDef,
     RebootBrokerResponseTypeDef,
     ServerlessRequestTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
@@ -198,31 +207,62 @@
     ) -> CreateConfigurationResponseTypeDef:
         """
         Creates a new MSK configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_configuration)
         """
+    def create_vpc_connection(
+        self,
+        *,
+        TargetClusterArn: str,
+        Authentication: str,
+        VpcId: str,
+        ClientSubnets: Sequence[str],
+        SecurityGroups: Sequence[str],
+        Tags: Mapping[str, str] = ...
+    ) -> CreateVpcConnectionResponseTypeDef:
+        """
+        Creates a new MSK VPC connection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.create_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#create_vpc_connection)
+        """
     def delete_cluster(
         self, *, ClusterArn: str, CurrentVersion: str = ...
     ) -> DeleteClusterResponseTypeDef:
         """
         Deletes the MSK cluster specified by the Amazon Resource Name (ARN) in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster)
         """
+    def delete_cluster_policy(self, *, ClusterArn: str) -> Dict[str, Any]:
+        """
+        Deletes the MSK cluster policy specified by the Amazon Resource Name (ARN) in
+        the request.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_cluster_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_cluster_policy)
+        """
     def delete_configuration(self, *, Arn: str) -> DeleteConfigurationResponseTypeDef:
         """
         Deletes an MSK Configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_configuration)
         """
+    def delete_vpc_connection(self, *, Arn: str) -> DeleteVpcConnectionResponseTypeDef:
+        """
+        Deletes a MSK VPC connection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.delete_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#delete_vpc_connection)
+        """
     def describe_cluster(self, *, ClusterArn: str) -> DescribeClusterResponseTypeDef:
         """
         Returns a description of the MSK cluster whose Amazon Resource Name (ARN) is
         specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_cluster)
@@ -256,14 +296,21 @@
     ) -> DescribeConfigurationRevisionResponseTypeDef:
         """
         Returns a description of this revision of the configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_configuration_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_configuration_revision)
         """
+    def describe_vpc_connection(self, *, Arn: str) -> DescribeVpcConnectionResponseTypeDef:
+        """
+        Returns a description of this MSK VPC connection.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.describe_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#describe_vpc_connection)
+        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -276,23 +323,40 @@
     def get_bootstrap_brokers(self, *, ClusterArn: str) -> GetBootstrapBrokersResponseTypeDef:
         """
         A list of brokers that a client application can use to bootstrap.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_bootstrap_brokers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_bootstrap_brokers)
         """
+    def get_cluster_policy(self, *, ClusterArn: str) -> GetClusterPolicyResponseTypeDef:
+        """
+        Get the MSK cluster policy specified by the Amazon Resource Name (ARN) in the
+        request.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_cluster_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_cluster_policy)
+        """
     def get_compatible_kafka_versions(
         self, *, ClusterArn: str = ...
     ) -> GetCompatibleKafkaVersionsResponseTypeDef:
         """
         Gets the Apache Kafka versions to which you can update the MSK cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_compatible_kafka_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_compatible_kafka_versions)
         """
+    def list_client_vpc_connections(
+        self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListClientVpcConnectionsResponseTypeDef:
+        """
+        Returns a list of all the VPC connections in this Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_client_vpc_connections)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_client_vpc_connections)
+        """
     def list_cluster_operations(
         self, *, ClusterArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListClusterOperationsResponseTypeDef:
         """
         Returns a list of all the operations that have been performed on the specified
         MSK cluster.
 
@@ -370,23 +434,51 @@
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_tags_for_resource)
         """
+    def list_vpc_connections(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListVpcConnectionsResponseTypeDef:
+        """
+        Returns a list of all the VPC connections in this Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.list_vpc_connections)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#list_vpc_connections)
+        """
+    def put_cluster_policy(
+        self, *, ClusterArn: str, Policy: str, CurrentVersion: str = ...
+    ) -> PutClusterPolicyResponseTypeDef:
+        """
+        Creates or updates the MSK cluster policy specified by the cluster Amazon
+        Resource Name (ARN) in the request.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.put_cluster_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#put_cluster_policy)
+        """
     def reboot_broker(
         self, *, BrokerIds: Sequence[str], ClusterArn: str
     ) -> RebootBrokerResponseTypeDef:
         """
         Reboots brokers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reboot_broker)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reboot_broker)
         """
+    def reject_client_vpc_connection(
+        self, *, ClusterArn: str, VpcConnectionArn: str
+    ) -> Dict[str, Any]:
+        """
+        Returns empty response.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.reject_client_vpc_connection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#reject_client_vpc_connection)
+        """
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to the specified MSK resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.tag_resource)
@@ -520,14 +612,22 @@
         Updates cluster broker volume size (or) sets cluster storage mode to TIERED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_storage)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_client_vpc_connections"]
+    ) -> ListClientVpcConnectionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_cluster_operations"]
     ) -> ListClusterOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
     @overload
@@ -576,7 +676,15 @@
     def get_paginator(
         self, operation_name: Literal["list_scram_secrets"]
     ) -> ListScramSecretsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
         """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["list_vpc_connections"]
+    ) -> ListVpcConnectionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,28 @@
     "BrokerAZDistributionType",
     "ClientBrokerType",
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
+    "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
+    "ListVpcConnectionsPaginatorName",
     "NodeTypeType",
     "StorageModeType",
+    "UserIdentityTypeType",
+    "VpcConnectionStateType",
     "KafkaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -59,24 +63,37 @@
 ]
 ClusterTypeType = Literal["PROVISIONED", "SERVERLESS"]
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
+ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
+ListVpcConnectionsPaginatorName = Literal["list_vpc_connections"]
 NodeTypeType = Literal["BROKER"]
 StorageModeType = Literal["LOCAL", "TIERED"]
+UserIdentityTypeType = Literal["AWSACCOUNT", "AWSSERVICE"]
+VpcConnectionStateType = Literal[
+    "AVAILABLE",
+    "CREATING",
+    "DEACTIVATING",
+    "DELETING",
+    "FAILED",
+    "INACTIVE",
+    "REJECTED",
+    "REJECTING",
+]
 KafkaServiceName = Literal["kafka"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -85,14 +102,15 @@
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
@@ -124,21 +142,23 @@
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
@@ -217,14 +237,15 @@
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
@@ -235,14 +256,15 @@
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
@@ -278,14 +300,15 @@
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
@@ -304,16 +327,19 @@
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
@@ -393,18 +419,21 @@
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
@@ -423,40 +452,47 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_client_vpc_connections",
     "list_cluster_operations",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
+    "list_vpc_connections",
 ]
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
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,28 @@
     "BrokerAZDistributionType",
     "ClientBrokerType",
     "ClusterStateType",
     "ClusterTypeType",
     "ConfigurationStateType",
     "EnhancedMonitoringType",
     "KafkaVersionStatusType",
+    "ListClientVpcConnectionsPaginatorName",
     "ListClusterOperationsPaginatorName",
     "ListClustersPaginatorName",
     "ListClustersV2PaginatorName",
     "ListConfigurationRevisionsPaginatorName",
     "ListConfigurationsPaginatorName",
     "ListKafkaVersionsPaginatorName",
     "ListNodesPaginatorName",
     "ListScramSecretsPaginatorName",
+    "ListVpcConnectionsPaginatorName",
     "NodeTypeType",
     "StorageModeType",
+    "UserIdentityTypeType",
+    "VpcConnectionStateType",
     "KafkaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -57,24 +61,37 @@
 ]
 ClusterTypeType = Literal["PROVISIONED", "SERVERLESS"]
 ConfigurationStateType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 EnhancedMonitoringType = Literal[
     "DEFAULT", "PER_BROKER", "PER_TOPIC_PER_BROKER", "PER_TOPIC_PER_PARTITION"
 ]
 KafkaVersionStatusType = Literal["ACTIVE", "DEPRECATED"]
+ListClientVpcConnectionsPaginatorName = Literal["list_client_vpc_connections"]
 ListClusterOperationsPaginatorName = Literal["list_cluster_operations"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListClustersV2PaginatorName = Literal["list_clusters_v2"]
 ListConfigurationRevisionsPaginatorName = Literal["list_configuration_revisions"]
 ListConfigurationsPaginatorName = Literal["list_configurations"]
 ListKafkaVersionsPaginatorName = Literal["list_kafka_versions"]
 ListNodesPaginatorName = Literal["list_nodes"]
 ListScramSecretsPaginatorName = Literal["list_scram_secrets"]
+ListVpcConnectionsPaginatorName = Literal["list_vpc_connections"]
 NodeTypeType = Literal["BROKER"]
 StorageModeType = Literal["LOCAL", "TIERED"]
+UserIdentityTypeType = Literal["AWSACCOUNT", "AWSSERVICE"]
+VpcConnectionStateType = Literal[
+    "AVAILABLE",
+    "CREATING",
+    "DEACTIVATING",
+    "DELETING",
+    "FAILED",
+    "INACTIVE",
+    "REJECTED",
+    "REJECTING",
+]
 KafkaServiceName = Literal["kafka"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -83,14 +100,15 @@
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
@@ -122,21 +140,23 @@
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
@@ -215,14 +235,15 @@
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
@@ -233,14 +254,15 @@
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
@@ -276,14 +298,15 @@
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
@@ -302,16 +325,19 @@
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
@@ -391,18 +417,21 @@
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
@@ -421,40 +450,47 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
+    "list_client_vpc_connections",
     "list_cluster_operations",
     "list_clusters",
     "list_clusters_v2",
     "list_configuration_revisions",
     "list_configurations",
     "list_kafka_versions",
     "list_nodes",
     "list_scram_secrets",
+    "list_vpc_connections",
 ]
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
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,98 +6,121 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kafka.client import KafkaClient
     from mypy_boto3_kafka.paginator import (
+        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
+        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
+    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
+    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
+    "ListVpcConnectionsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
 
+class ListClientVpcConnectionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
+    """
+
+    def paginate(
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListClientVpcConnectionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
+        """
+
+
 class ListClusterOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNameFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterNameFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
         """
 
 
@@ -108,88 +131,103 @@
     """
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclustersv2paginator)
         """
 
 
 class ListConfigurationRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
         """
 
 
 class ListConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
         """
 
 
 class ListKafkaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKafkaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
         """
 
 
 class ListNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
         """
 
 
 class ListScramSecretsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScramSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
         """
+
+
+class ListVpcConnectionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListVpcConnectionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
+        """
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/paginator.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -6,94 +6,116 @@
 Usage::
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_kafka.client import KafkaClient
     from mypy_boto3_kafka.paginator import (
+        ListClientVpcConnectionsPaginator,
         ListClusterOperationsPaginator,
         ListClustersPaginator,
         ListClustersV2Paginator,
         ListConfigurationRevisionsPaginator,
         ListConfigurationsPaginator,
         ListKafkaVersionsPaginator,
         ListNodesPaginator,
         ListScramSecretsPaginator,
+        ListVpcConnectionsPaginator,
     )
 
     session = Session()
     client: KafkaClient = session.client("kafka")
 
+    list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
     list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator("list_cluster_operations")
     list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
     list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
     list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator("list_configuration_revisions")
     list_configurations_paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")
     list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator("list_kafka_versions")
     list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
     list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+    list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator("list_vpc_connections")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
+    ListClientVpcConnectionsResponseTypeDef,
     ListClusterOperationsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListClustersV2ResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListScramSecretsResponseTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
+    "ListClientVpcConnectionsPaginator",
     "ListClusterOperationsPaginator",
     "ListClustersPaginator",
     "ListClustersV2Paginator",
     "ListConfigurationRevisionsPaginator",
     "ListConfigurationsPaginator",
     "ListKafkaVersionsPaginator",
     "ListNodesPaginator",
     "ListScramSecretsPaginator",
+    "ListVpcConnectionsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+class ListClientVpcConnectionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
+    """
+
+    def paginate(
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListClientVpcConnectionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClientVpcConnections.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclientvpcconnectionspaginator)
+        """
+
 class ListClusterOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNameFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterNameFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
         """
 
 class ListClustersV2Paginator(Paginator):
@@ -103,83 +125,97 @@
     """
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersV2ResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclustersv2paginator)
         """
 
 class ListConfigurationRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurationRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationrevisionspaginator)
         """
 
 class ListConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listconfigurationspaginator)
         """
 
 class ListKafkaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKafkaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListKafkaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listkafkaversionspaginator)
         """
 
 class ListNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listnodespaginator)
         """
 
 class ListScramSecretsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
     """
 
     def paginate(
-        self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListScramSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListScramSecrets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listscramsecretspaginator)
         """
+
+class ListVpcConnectionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListVpcConnectionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListVpcConnections.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listvpcconnectionspaginator)
+        """
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,149 +21,179 @@
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     StorageModeType,
+    UserIdentityTypeType,
+    VpcConnectionStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsTypeDef",
     "UnauthenticatedTypeDef",
+    "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
+    "CreateClusterResponseTypeDef",
+    "CreateClusterV2ResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
+    "CreateVpcConnectionRequestRequestTypeDef",
+    "CreateVpcConnectionResponseTypeDef",
+    "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
+    "DeleteClusterResponseTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
+    "DeleteConfigurationResponseTypeDef",
+    "DeleteVpcConnectionRequestRequestTypeDef",
+    "DeleteVpcConnectionResponseTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
+    "DescribeVpcConnectionRequestRequestTypeDef",
+    "DescribeVpcConnectionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionAtRestTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
+    "GetBootstrapBrokersResponseTypeDef",
+    "GetClusterPolicyRequestRequestTypeDef",
+    "GetClusterPolicyResponseTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    "ListClientVpcConnectionsRequestRequestTypeDef",
+    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListClustersV2RequestRequestTypeDef",
+    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
+    "ListNodesRequestListNodesPaginateTypeDef",
     "ListNodesRequestRequestTypeDef",
+    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
+    "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
+    "ListVpcConnectionsRequestRequestTypeDef",
+    "VpcConnectionTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutClusterPolicyRequestRequestTypeDef",
+    "PutClusterPolicyResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
+    "RebootBrokerResponseTypeDef",
+    "RejectClientVpcConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
-    "UpdateBrokerTypeRequestRequestTypeDef",
-    "UpdateConfigurationRequestRequestTypeDef",
-    "CreateClusterResponseTypeDef",
-    "CreateClusterV2ResponseTypeDef",
-    "DeleteClusterResponseTypeDef",
-    "DeleteConfigurationResponseTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetBootstrapBrokersResponseTypeDef",
-    "ListScramSecretsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RebootBrokerResponseTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
+    "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
     "UpdateClusterConfigurationResponseTypeDef",
     "UpdateClusterKafkaVersionResponseTypeDef",
+    "UpdateConfigurationRequestRequestTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
+    "UserIdentityTypeDef",
+    "VpcConnectivityTlsTypeDef",
+    "VpcConnectivityIamTypeDef",
+    "VpcConnectivityScramTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
+    "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
-    "ConnectivityInfoTypeDef",
     "EncryptionInfoTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
-    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
-    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
-    "ListNodesRequestListNodesPaginateTypeDef",
-    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
     "SaslTypeDef",
+    "VpcConnectionInfoTypeDef",
+    "VpcConnectivitySaslTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
-    "UpdateConnectivityRequestRequestTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ClientAuthenticationTypeDef",
-    "BrokerNodeGroupInfoTypeDef",
+    "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
-    "MutableClusterInfoTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
+    "VpcConnectivityTypeDef",
+    "ConnectivityInfoTypeDef",
+    "BrokerNodeGroupInfoTypeDef",
+    "MutableClusterInfoTypeDef",
+    "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
     "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
@@ -179,25 +209,14 @@
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
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
 UnprocessedScramSecretTypeDef = TypedDict(
     "UnprocessedScramSecretTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "SecretArn": str,
     },
@@ -302,14 +321,38 @@
     "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+_RequiredClientVpcConnectionTypeDef = TypedDict(
+    "_RequiredClientVpcConnectionTypeDef",
+    {
+        "VpcConnectionArn": str,
+    },
+)
+_OptionalClientVpcConnectionTypeDef = TypedDict(
+    "_OptionalClientVpcConnectionTypeDef",
+    {
+        "Authentication": str,
+        "CreationTime": datetime,
+        "State": VpcConnectionStateType,
+        "Owner": str,
+    },
+    total=False,
+)
+
+
+class ClientVpcConnectionTypeDef(
+    _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
+):
+    pass
+
+
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -375,14 +418,35 @@
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+CreateClusterResponseTypeDef = TypedDict(
+    "CreateClusterResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateClusterV2ResponseTypeDef = TypedDict(
+    "CreateClusterV2ResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ClusterType": ClusterTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "Name": str,
         "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
@@ -399,14 +463,62 @@
 class CreateConfigurationRequestRequestTypeDef(
     _RequiredCreateConfigurationRequestRequestTypeDef,
     _OptionalCreateConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpcConnectionRequestRequestTypeDef",
+    {
+        "TargetClusterArn": str,
+        "Authentication": str,
+        "VpcId": str,
+        "ClientSubnets": Sequence[str],
+        "SecurityGroups": Sequence[str],
+    },
+)
+_OptionalCreateVpcConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpcConnectionRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateVpcConnectionRequestRequestTypeDef(
+    _RequiredCreateVpcConnectionRequestRequestTypeDef,
+    _OptionalCreateVpcConnectionRequestRequestTypeDef,
+):
+    pass
+
+
+CreateVpcConnectionResponseTypeDef = TypedDict(
+    "CreateVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "ClientSubnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
+    "DeleteClusterPolicyRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+
 _RequiredDeleteClusterRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalDeleteClusterRequestRequestTypeDef = TypedDict(
@@ -420,21 +532,55 @@
 
 class DeleteClusterRequestRequestTypeDef(
     _RequiredDeleteClusterRequestRequestTypeDef, _OptionalDeleteClusterRequestRequestTypeDef
 ):
     pass
 
 
+DeleteClusterResponseTypeDef = TypedDict(
+    "DeleteClusterResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "State": ClusterStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteConfigurationResponseTypeDef = TypedDict(
+    "DeleteConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "State": ConfigurationStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteVpcConnectionRequestRequestTypeDef = TypedDict(
+    "DeleteVpcConnectionRequestRequestTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
+DeleteVpcConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeClusterOperationRequestRequestTypeDef = TypedDict(
     "DescribeClusterOperationRequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
@@ -463,14 +609,56 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
 
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "Description": str,
+        "Revision": int,
+        "ServerProperties": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeVpcConnectionRequestRequestTypeDef = TypedDict(
+    "DescribeVpcConnectionRequestRequestTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
+DescribeVpcConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "TargetClusterArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "Subnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
@@ -486,14 +674,47 @@
 GetBootstrapBrokersRequestRequestTypeDef = TypedDict(
     "GetBootstrapBrokersRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
+GetBootstrapBrokersResponseTypeDef = TypedDict(
+    "GetBootstrapBrokersResponseTypeDef",
+    {
+        "BootstrapBrokerString": str,
+        "BootstrapBrokerStringTls": str,
+        "BootstrapBrokerStringSaslScram": str,
+        "BootstrapBrokerStringSaslIam": str,
+        "BootstrapBrokerStringPublicTls": str,
+        "BootstrapBrokerStringPublicSaslScram": str,
+        "BootstrapBrokerStringPublicSaslIam": str,
+        "BootstrapBrokerStringVpcConnectivityTls": str,
+        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
+        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetClusterPolicyRequestRequestTypeDef = TypedDict(
+    "GetClusterPolicyRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+
+GetClusterPolicyResponseTypeDef = TypedDict(
+    "GetClusterPolicyResponseTypeDef",
+    {
+        "CurrentVersion": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCompatibleKafkaVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
@@ -525,24 +746,81 @@
     {
         "Version": str,
         "Status": KafkaVersionStatusType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterArn": str,
+    },
+)
+_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
+    _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListClientVpcConnectionsRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListClientVpcConnectionsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListClientVpcConnectionsRequestRequestTypeDef(
+    _RequiredListClientVpcConnectionsRequestRequestTypeDef,
+    _OptionalListClientVpcConnectionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
+    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -558,35 +836,76 @@
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "ClusterTypeFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersV2RequestRequestTypeDef = TypedDict(
     "ListClustersV2RequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "ClusterTypeFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
+    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConfigurationRevisionsRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
@@ -602,32 +921,70 @@
 class ListConfigurationRevisionsRequestRequestTypeDef(
     _RequiredListConfigurationRevisionsRequestRequestTypeDef,
     _OptionalListConfigurationRevisionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConfigurationsRequestRequestTypeDef = TypedDict(
     "ListConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKafkaVersionsRequestRequestTypeDef = TypedDict(
     "ListKafkaVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_RequiredListNodesRequestListNodesPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_OptionalListNodesRequestListNodesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListNodesRequestListNodesPaginateTypeDef(
+    _RequiredListNodesRequestListNodesPaginateTypeDef,
+    _OptionalListNodesRequestListNodesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListNodesRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListNodesRequestRequestTypeDef = TypedDict(
@@ -642,14 +999,36 @@
 
 class ListNodesRequestRequestTypeDef(
     _RequiredListNodesRequestRequestTypeDef, _OptionalListNodesRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
+    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListScramSecretsRequestRequestTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestRequestTypeDef = TypedDict(
@@ -664,333 +1043,393 @@
 
 class ListScramSecretsRequestRequestTypeDef(
     _RequiredListScramSecretsRequestRequestTypeDef, _OptionalListScramSecretsRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+ListScramSecretsResponseTypeDef = TypedDict(
+    "ListScramSecretsResponseTypeDef",
     {
-        "ResourceArn": str,
+        "NextToken": str,
+        "SecretArnList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NodeExporterInfoTypeDef = TypedDict(
-    "NodeExporterInfoTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "EnabledInBroker": bool,
+        "ResourceArn": str,
     },
 )
 
-NodeExporterTypeDef = TypedDict(
-    "NodeExporterTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "EnabledInBroker": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ZookeeperNodeInfoTypeDef = TypedDict(
-    "ZookeeperNodeInfoTypeDef",
+ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     {
-        "AttachedENIId": str,
-        "ClientVpcIpAddress": str,
-        "Endpoints": List[str],
-        "ZookeeperId": float,
-        "ZookeeperVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-RebootBrokerRequestRequestTypeDef = TypedDict(
-    "RebootBrokerRequestRequestTypeDef",
-    {
-        "BrokerIds": Sequence[str],
-        "ClusterArn": str,
-    },
-)
-
-ScramTypeDef = TypedDict(
-    "ScramTypeDef",
+ListVpcConnectionsRequestRequestTypeDef = TypedDict(
+    "ListVpcConnectionsRequestRequestTypeDef",
     {
-        "Enabled": bool,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-_RequiredVpcConfigTypeDef = TypedDict(
-    "_RequiredVpcConfigTypeDef",
+_RequiredVpcConnectionTypeDef = TypedDict(
+    "_RequiredVpcConnectionTypeDef",
     {
-        "SubnetIds": Sequence[str],
+        "VpcConnectionArn": str,
+        "TargetClusterArn": str,
     },
 )
-_OptionalVpcConfigTypeDef = TypedDict(
-    "_OptionalVpcConfigTypeDef",
+_OptionalVpcConnectionTypeDef = TypedDict(
+    "_OptionalVpcConnectionTypeDef",
     {
-        "SecurityGroupIds": Sequence[str],
+        "CreationTime": datetime,
+        "Authentication": str,
+        "VpcId": str,
+        "State": VpcConnectionStateType,
     },
     total=False,
 )
 
 
-class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
+class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+NodeExporterInfoTypeDef = TypedDict(
+    "NodeExporterInfoTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "EnabledInBroker": bool,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+NodeExporterTypeDef = TypedDict(
+    "NodeExporterTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "EnabledInBroker": bool,
     },
 )
 
-UpdateBrokerCountRequestRequestTypeDef = TypedDict(
-    "UpdateBrokerCountRequestRequestTypeDef",
+ZookeeperNodeInfoTypeDef = TypedDict(
+    "ZookeeperNodeInfoTypeDef",
     {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-        "TargetNumberOfBrokerNodes": int,
+        "AttachedENIId": str,
+        "ClientVpcIpAddress": str,
+        "Endpoints": List[str],
+        "ZookeeperId": float,
+        "ZookeeperVersion": str,
     },
+    total=False,
 )
 
-UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
-    "UpdateBrokerTypeRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-        "TargetInstanceType": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+_RequiredPutClusterPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutClusterPolicyRequestRequestTypeDef",
     {
-        "Arn": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
+        "ClusterArn": str,
+        "Policy": str,
     },
 )
-_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+_OptionalPutClusterPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutClusterPolicyRequestRequestTypeDef",
     {
-        "Description": str,
+        "CurrentVersion": str,
     },
     total=False,
 )
 
 
-class UpdateConfigurationRequestRequestTypeDef(
-    _RequiredUpdateConfigurationRequestRequestTypeDef,
-    _OptionalUpdateConfigurationRequestRequestTypeDef,
+class PutClusterPolicyRequestRequestTypeDef(
+    _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
 ):
     pass
 
 
-CreateClusterResponseTypeDef = TypedDict(
-    "CreateClusterResponseTypeDef",
+PutClusterPolicyResponseTypeDef = TypedDict(
+    "PutClusterPolicyResponseTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CurrentVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateClusterV2ResponseTypeDef = TypedDict(
-    "CreateClusterV2ResponseTypeDef",
+RebootBrokerRequestRequestTypeDef = TypedDict(
+    "RebootBrokerRequestRequestTypeDef",
     {
+        "BrokerIds": Sequence[str],
         "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ClusterType": ClusterTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteClusterResponseTypeDef = TypedDict(
-    "DeleteClusterResponseTypeDef",
+RebootBrokerResponseTypeDef = TypedDict(
+    "RebootBrokerResponseTypeDef",
     {
         "ClusterArn": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteConfigurationResponseTypeDef = TypedDict(
-    "DeleteConfigurationResponseTypeDef",
+RejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
+    "RejectClientVpcConnectionRequestRequestTypeDef",
     {
-        "Arn": str,
-        "State": ConfigurationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClusterArn": str,
+        "VpcConnectionArn": str,
     },
 )
 
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "CreationTime": datetime,
-        "Description": str,
-        "Revision": int,
-        "ServerProperties": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ScramTypeDef = TypedDict(
+    "ScramTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Enabled": bool,
     },
+    total=False,
 )
 
-GetBootstrapBrokersResponseTypeDef = TypedDict(
-    "GetBootstrapBrokersResponseTypeDef",
+_RequiredVpcConfigTypeDef = TypedDict(
+    "_RequiredVpcConfigTypeDef",
     {
-        "BootstrapBrokerString": str,
-        "BootstrapBrokerStringTls": str,
-        "BootstrapBrokerStringSaslScram": str,
-        "BootstrapBrokerStringSaslIam": str,
-        "BootstrapBrokerStringPublicTls": str,
-        "BootstrapBrokerStringPublicSaslScram": str,
-        "BootstrapBrokerStringPublicSaslIam": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SubnetIds": Sequence[str],
     },
 )
+_OptionalVpcConfigTypeDef = TypedDict(
+    "_OptionalVpcConfigTypeDef",
+    {
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
 
-ListScramSecretsResponseTypeDef = TypedDict(
-    "ListScramSecretsResponseTypeDef",
+
+class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "SecretArnList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-RebootBrokerResponseTypeDef = TypedDict(
-    "RebootBrokerResponseTypeDef",
+UpdateBrokerCountRequestRequestTypeDef = TypedDict(
+    "UpdateBrokerCountRequestRequestTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CurrentVersion": str,
+        "TargetNumberOfBrokerNodes": int,
     },
 )
 
 UpdateBrokerCountResponseTypeDef = TypedDict(
     "UpdateBrokerCountResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBrokerStorageResponseTypeDef = TypedDict(
     "UpdateBrokerStorageResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
+    "UpdateBrokerTypeRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+        "CurrentVersion": str,
+        "TargetInstanceType": str,
     },
 )
 
 UpdateBrokerTypeResponseTypeDef = TypedDict(
     "UpdateBrokerTypeResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterConfigurationResponseTypeDef = TypedDict(
     "UpdateClusterConfigurationResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterKafkaVersionResponseTypeDef = TypedDict(
     "UpdateClusterKafkaVersionResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Arn": str,
+        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
+_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateConfigurationRequestRequestTypeDef(
+    _RequiredUpdateConfigurationRequestRequestTypeDef,
+    _OptionalUpdateConfigurationRequestRequestTypeDef,
+):
+    pass
+
 
 UpdateConnectivityResponseTypeDef = TypedDict(
     "UpdateConnectivityResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMonitoringResponseTypeDef = TypedDict(
     "UpdateMonitoringResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSecurityResponseTypeDef = TypedDict(
     "UpdateSecurityResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStorageResponseTypeDef = TypedDict(
     "UpdateStorageResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
+    {
+        "Type": UserIdentityTypeType,
+        "PrincipalId": str,
+    },
+    total=False,
+)
+
+VpcConnectivityTlsTypeDef = TypedDict(
+    "VpcConnectivityTlsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityIamTypeDef = TypedDict(
+    "VpcConnectivityIamTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityScramTypeDef = TypedDict(
+    "VpcConnectivityScramTypeDef",
+    {
+        "Enabled": bool,
     },
+    total=False,
 )
 
 BatchAssociateScramSecretResponseTypeDef = TypedDict(
     "BatchAssociateScramSecretResponseTypeDef",
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateScramSecretResponseTypeDef = TypedDict(
     "BatchDisassociateScramSecretResponseTypeDef",
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
@@ -1064,28 +1503,37 @@
         "ClientVpcIpAddress": str,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "Endpoints": List[str],
     },
     total=False,
 )
 
+ListClientVpcConnectionsResponseTypeDef = TypedDict(
+    "ListClientVpcConnectionsResponseTypeDef",
+    {
+        "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
 )
 
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateClusterConfigurationRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1135,56 +1583,48 @@
     "CreateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConfigurationResponseTypeDef = TypedDict(
     "DescribeConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfigurationRevisionsResponseTypeDef = TypedDict(
     "ListConfigurationRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfigurationResponseTypeDef = TypedDict(
     "UpdateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConnectivityInfoTypeDef = TypedDict(
-    "ConnectivityInfoTypeDef",
-    {
-        "PublicAccess": PublicAccessTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
@@ -1201,141 +1641,27 @@
 )
 
 ListKafkaVersionsResponseTypeDef = TypedDict(
     "ListKafkaVersionsResponseTypeDef",
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
-    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "ClusterNameFilter": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
-    {
-        "ClusterNameFilter": str,
-        "ClusterTypeFilter": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
-    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-):
-    pass
-
-
-ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_RequiredListNodesRequestListNodesPaginateTypeDef",
-    {
-        "ClusterArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_OptionalListNodesRequestListNodesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListNodesRequestListNodesPaginateTypeDef(
-    _RequiredListNodesRequestListNodesPaginateTypeDef,
-    _OptionalListNodesRequestListNodesPaginateTypeDef,
-):
-    pass
-
 
-_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
+ListVpcConnectionsResponseTypeDef = TypedDict(
+    "ListVpcConnectionsResponseTypeDef",
     {
-        "ClusterArn": str,
-    },
-)
-_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "VpcConnections": List[VpcConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
-    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
-):
-    pass
-
-
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1355,14 +1681,34 @@
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
+VpcConnectionInfoTypeDef = TypedDict(
+    "VpcConnectionInfoTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "Owner": str,
+        "UserIdentity": UserIdentityTypeDef,
+        "CreationTime": datetime,
+    },
+    total=False,
+)
+
+VpcConnectivitySaslTypeDef = TypedDict(
+    "VpcConnectivitySaslTypeDef",
+    {
+        "Scram": VpcConnectivityScramTypeDef,
+        "Iam": VpcConnectivityIamTypeDef,
+    },
+    total=False,
+)
+
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1397,24 +1743,15 @@
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectivityRequestRequestTypeDef = TypedDict(
-    "UpdateConnectivityRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "CurrentVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
@@ -1442,45 +1779,29 @@
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoTypeDef",
+VpcConnectivityClientAuthenticationTypeDef = TypedDict(
+    "VpcConnectivityClientAuthenticationTypeDef",
     {
-        "ClientSubnets": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoTypeDef",
-    {
-        "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": Sequence[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "Sasl": VpcConnectivitySaslTypeDef,
+        "Tls": VpcConnectivityTlsTypeDef,
     },
     total=False,
 )
 
-
-class BrokerNodeGroupInfoTypeDef(
-    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
-):
-    pass
-
-
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredServerlessRequestTypeDef = TypedDict(
     "_RequiredServerlessRequestTypeDef",
     {
         "VpcConfigs": Sequence[VpcConfigTypeDef],
@@ -1540,14 +1861,80 @@
 
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+        "CurrentVersion": str,
+    },
+)
+_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityRequestRequestTypeDef",
+    {
+        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSecurityRequestRequestTypeDef(
+    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
+):
+    pass
+
+
+VpcConnectivityTypeDef = TypedDict(
+    "VpcConnectivityTypeDef",
+    {
+        "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
+    },
+    total=False,
+)
+
+ConnectivityInfoTypeDef = TypedDict(
+    "ConnectivityInfoTypeDef",
+    {
+        "PublicAccess": PublicAccessTypeDef,
+        "VpcConnectivity": VpcConnectivityTypeDef,
+    },
+    total=False,
+)
+
+_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoTypeDef",
+    {
+        "ClientSubnets": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoTypeDef",
+    {
+        "BrokerAZDistribution": Literal["DEFAULT"],
+        "SecurityGroups": Sequence[str],
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "ZoneIds": Sequence[str],
+    },
+    total=False,
+)
+
+
+class BrokerNodeGroupInfoTypeDef(
+    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+):
+    pass
+
+
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -1559,36 +1946,22 @@
         "EncryptionInfo": EncryptionInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityRequestRequestTypeDef",
+UpdateConnectivityRequestRequestTypeDef = TypedDict(
+    "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
-_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityRequestRequestTypeDef",
-    {
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateSecurityRequestRequestTypeDef(
-    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
-):
-    pass
-
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationTypeDef,
@@ -1710,32 +2083,33 @@
         "ErrorInfo": ErrorInfoTypeDef,
         "OperationArn": str,
         "OperationState": str,
         "OperationSteps": List[ClusterOperationStepTypeDef],
         "OperationType": str,
         "SourceClusterInfo": MutableClusterInfoTypeDef,
         "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterV2RequestRequestTypeDef",
     {
         "ClusterName": str,
@@ -1776,36 +2150,36 @@
     total=False,
 )
 
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClusterOperationsResponseTypeDef = TypedDict(
     "ListClusterOperationsResponseTypeDef",
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersV2ResponseTypeDef = TypedDict(
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -21,148 +21,178 @@
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
     StorageModeType,
+    UserIdentityTypeType,
+    VpcConnectionStateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchAssociateScramSecretRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
     "TlsTypeDef",
     "UnauthenticatedTypeDef",
+    "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
+    "CreateClusterResponseTypeDef",
+    "CreateClusterV2ResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
+    "CreateVpcConnectionRequestRequestTypeDef",
+    "CreateVpcConnectionResponseTypeDef",
+    "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
+    "DeleteClusterResponseTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
+    "DeleteConfigurationResponseTypeDef",
+    "DeleteVpcConnectionRequestRequestTypeDef",
+    "DeleteVpcConnectionResponseTypeDef",
     "DescribeClusterOperationRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeClusterV2RequestRequestTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
+    "DescribeVpcConnectionRequestRequestTypeDef",
+    "DescribeVpcConnectionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionAtRestTypeDef",
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
+    "GetBootstrapBrokersResponseTypeDef",
+    "GetClusterPolicyRequestRequestTypeDef",
+    "GetClusterPolicyResponseTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
     "KafkaVersionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    "ListClientVpcConnectionsRequestRequestTypeDef",
+    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
     "ListClustersV2RequestRequestTypeDef",
+    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
     "ListKafkaVersionsRequestRequestTypeDef",
+    "ListNodesRequestListNodesPaginateTypeDef",
     "ListNodesRequestRequestTypeDef",
+    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListScramSecretsRequestRequestTypeDef",
+    "ListScramSecretsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
+    "ListVpcConnectionsRequestRequestTypeDef",
+    "VpcConnectionTypeDef",
     "NodeExporterInfoTypeDef",
     "NodeExporterTypeDef",
     "ZookeeperNodeInfoTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutClusterPolicyRequestRequestTypeDef",
+    "PutClusterPolicyResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
+    "RebootBrokerResponseTypeDef",
+    "RejectClientVpcConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ScramTypeDef",
     "VpcConfigTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
-    "UpdateBrokerTypeRequestRequestTypeDef",
-    "UpdateConfigurationRequestRequestTypeDef",
-    "CreateClusterResponseTypeDef",
-    "CreateClusterV2ResponseTypeDef",
-    "DeleteClusterResponseTypeDef",
-    "DeleteConfigurationResponseTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetBootstrapBrokersResponseTypeDef",
-    "ListScramSecretsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RebootBrokerResponseTypeDef",
     "UpdateBrokerCountResponseTypeDef",
     "UpdateBrokerStorageResponseTypeDef",
+    "UpdateBrokerTypeRequestRequestTypeDef",
     "UpdateBrokerTypeResponseTypeDef",
     "UpdateClusterConfigurationResponseTypeDef",
     "UpdateClusterKafkaVersionResponseTypeDef",
+    "UpdateConfigurationRequestRequestTypeDef",
     "UpdateConnectivityResponseTypeDef",
     "UpdateMonitoringResponseTypeDef",
     "UpdateSecurityResponseTypeDef",
     "UpdateStorageResponseTypeDef",
+    "UserIdentityTypeDef",
+    "VpcConnectivityTlsTypeDef",
+    "VpcConnectivityIamTypeDef",
+    "VpcConnectivityScramTypeDef",
     "BatchAssociateScramSecretResponseTypeDef",
     "BatchDisassociateScramSecretResponseTypeDef",
     "BrokerEBSVolumeInfoTypeDef",
     "EBSStorageInfoTypeDef",
     "UpdateStorageRequestRequestTypeDef",
     "BrokerLogsTypeDef",
     "BrokerNodeInfoTypeDef",
+    "ListClientVpcConnectionsResponseTypeDef",
     "ClusterOperationStepTypeDef",
     "GetCompatibleKafkaVersionsResponseTypeDef",
     "UpdateClusterConfigurationRequestRequestTypeDef",
     "UpdateClusterKafkaVersionRequestRequestTypeDef",
     "ConfigurationTypeDef",
     "CreateConfigurationResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
     "UpdateConfigurationResponseTypeDef",
-    "ConnectivityInfoTypeDef",
     "EncryptionInfoTypeDef",
     "ServerlessSaslTypeDef",
     "ListKafkaVersionsResponseTypeDef",
-    "ListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
-    "ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
-    "ListNodesRequestListNodesPaginateTypeDef",
-    "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
     "SaslTypeDef",
+    "VpcConnectionInfoTypeDef",
+    "VpcConnectivitySaslTypeDef",
     "UpdateBrokerStorageRequestRequestTypeDef",
     "StorageInfoTypeDef",
     "LoggingInfoTypeDef",
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
-    "UpdateConnectivityRequestRequestTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ClientAuthenticationTypeDef",
-    "BrokerNodeGroupInfoTypeDef",
+    "VpcConnectivityClientAuthenticationTypeDef",
     "ListNodesResponseTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
-    "MutableClusterInfoTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
+    "VpcConnectivityTypeDef",
+    "ConnectivityInfoTypeDef",
+    "BrokerNodeGroupInfoTypeDef",
+    "MutableClusterInfoTypeDef",
+    "UpdateConnectivityRequestRequestTypeDef",
     "ClusterInfoTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
     "ProvisionedTypeDef",
     "ClusterOperationInfoTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
@@ -178,25 +208,14 @@
     "BatchAssociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
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
 UnprocessedScramSecretTypeDef = TypedDict(
     "UnprocessedScramSecretTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "SecretArn": str,
     },
@@ -295,14 +314,36 @@
     "UnauthenticatedTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+_RequiredClientVpcConnectionTypeDef = TypedDict(
+    "_RequiredClientVpcConnectionTypeDef",
+    {
+        "VpcConnectionArn": str,
+    },
+)
+_OptionalClientVpcConnectionTypeDef = TypedDict(
+    "_OptionalClientVpcConnectionTypeDef",
+    {
+        "Authentication": str,
+        "CreationTime": datetime,
+        "State": VpcConnectionStateType,
+        "Owner": str,
+    },
+    total=False,
+)
+
+class ClientVpcConnectionTypeDef(
+    _RequiredClientVpcConnectionTypeDef, _OptionalClientVpcConnectionTypeDef
+):
+    pass
+
 StateInfoTypeDef = TypedDict(
     "StateInfoTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
@@ -366,14 +407,35 @@
     "PublicAccessTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+CreateClusterResponseTypeDef = TypedDict(
+    "CreateClusterResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateClusterV2ResponseTypeDef = TypedDict(
+    "CreateClusterV2ResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "ClusterName": str,
+        "State": ClusterStateType,
+        "ClusterType": ClusterTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "Name": str,
         "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
@@ -388,14 +450,60 @@
 
 class CreateConfigurationRequestRequestTypeDef(
     _RequiredCreateConfigurationRequestRequestTypeDef,
     _OptionalCreateConfigurationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateVpcConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpcConnectionRequestRequestTypeDef",
+    {
+        "TargetClusterArn": str,
+        "Authentication": str,
+        "VpcId": str,
+        "ClientSubnets": Sequence[str],
+        "SecurityGroups": Sequence[str],
+    },
+)
+_OptionalCreateVpcConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpcConnectionRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateVpcConnectionRequestRequestTypeDef(
+    _RequiredCreateVpcConnectionRequestRequestTypeDef,
+    _OptionalCreateVpcConnectionRequestRequestTypeDef,
+):
+    pass
+
+CreateVpcConnectionResponseTypeDef = TypedDict(
+    "CreateVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "ClientSubnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteClusterPolicyRequestRequestTypeDef = TypedDict(
+    "DeleteClusterPolicyRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+
 _RequiredDeleteClusterRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalDeleteClusterRequestRequestTypeDef = TypedDict(
@@ -407,21 +515,55 @@
 )
 
 class DeleteClusterRequestRequestTypeDef(
     _RequiredDeleteClusterRequestRequestTypeDef, _OptionalDeleteClusterRequestRequestTypeDef
 ):
     pass
 
+DeleteClusterResponseTypeDef = TypedDict(
+    "DeleteClusterResponseTypeDef",
+    {
+        "ClusterArn": str,
+        "State": ClusterStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteConfigurationResponseTypeDef = TypedDict(
+    "DeleteConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "State": ConfigurationStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteVpcConnectionRequestRequestTypeDef = TypedDict(
+    "DeleteVpcConnectionRequestRequestTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
+DeleteVpcConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "State": VpcConnectionStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeClusterOperationRequestRequestTypeDef = TypedDict(
     "DescribeClusterOperationRequestRequestTypeDef",
     {
         "ClusterOperationArn": str,
     },
 )
 
@@ -450,14 +592,56 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "Arn": str,
         "Revision": int,
     },
 )
 
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "Description": str,
+        "Revision": int,
+        "ServerProperties": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeVpcConnectionRequestRequestTypeDef = TypedDict(
+    "DescribeVpcConnectionRequestRequestTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
+DescribeVpcConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcConnectionResponseTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "TargetClusterArn": str,
+        "State": VpcConnectionStateType,
+        "Authentication": str,
+        "VpcId": str,
+        "Subnets": List[str],
+        "SecurityGroups": List[str],
+        "CreationTime": datetime,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "DataVolumeKMSKeyId": str,
     },
 )
 
@@ -473,14 +657,47 @@
 GetBootstrapBrokersRequestRequestTypeDef = TypedDict(
     "GetBootstrapBrokersRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 
+GetBootstrapBrokersResponseTypeDef = TypedDict(
+    "GetBootstrapBrokersResponseTypeDef",
+    {
+        "BootstrapBrokerString": str,
+        "BootstrapBrokerStringTls": str,
+        "BootstrapBrokerStringSaslScram": str,
+        "BootstrapBrokerStringSaslIam": str,
+        "BootstrapBrokerStringPublicTls": str,
+        "BootstrapBrokerStringPublicSaslScram": str,
+        "BootstrapBrokerStringPublicSaslIam": str,
+        "BootstrapBrokerStringVpcConnectivityTls": str,
+        "BootstrapBrokerStringVpcConnectivitySaslScram": str,
+        "BootstrapBrokerStringVpcConnectivitySaslIam": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetClusterPolicyRequestRequestTypeDef = TypedDict(
+    "GetClusterPolicyRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+
+GetClusterPolicyResponseTypeDef = TypedDict(
+    "GetClusterPolicyResponseTypeDef",
+    {
+        "CurrentVersion": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetCompatibleKafkaVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
     total=False,
 )
@@ -512,24 +729,75 @@
     {
         "Version": str,
         "Status": KafkaVersionStatusType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterArn": str,
+    },
+)
+_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef(
+    _RequiredListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    _OptionalListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListClientVpcConnectionsRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClientVpcConnectionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListClientVpcConnectionsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListClientVpcConnectionsRequestRequestTypeDef(
+    _RequiredListClientVpcConnectionsRequestRequestTypeDef,
+    _OptionalListClientVpcConnectionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
+    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListClusterOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterOperationsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListClusterOperationsRequestRequestTypeDef = TypedDict(
@@ -543,35 +811,74 @@
 
 class ListClusterOperationsRequestRequestTypeDef(
     _RequiredListClusterOperationsRequestRequestTypeDef,
     _OptionalListClusterOperationsRequestRequestTypeDef,
 ):
     pass
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
+    "ListClustersV2RequestListClustersV2PaginateTypeDef",
+    {
+        "ClusterNameFilter": str,
+        "ClusterTypeFilter": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersV2RequestRequestTypeDef = TypedDict(
     "ListClustersV2RequestRequestTypeDef",
     {
         "ClusterNameFilter": str,
         "ClusterTypeFilter": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
+    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredListConfigurationRevisionsRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListConfigurationRevisionsRequestRequestTypeDef = TypedDict(
@@ -585,32 +892,68 @@
 
 class ListConfigurationRevisionsRequestRequestTypeDef(
     _RequiredListConfigurationRevisionsRequestRequestTypeDef,
     _OptionalListConfigurationRevisionsRequestRequestTypeDef,
 ):
     pass
 
+ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
+    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListConfigurationsRequestRequestTypeDef = TypedDict(
     "ListConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
+    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKafkaVersionsRequestRequestTypeDef = TypedDict(
     "ListKafkaVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_RequiredListNodesRequestListNodesPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
+    "_OptionalListNodesRequestListNodesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListNodesRequestListNodesPaginateTypeDef(
+    _RequiredListNodesRequestListNodesPaginateTypeDef,
+    _OptionalListNodesRequestListNodesPaginateTypeDef,
+):
+    pass
+
 _RequiredListNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListNodesRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListNodesRequestRequestTypeDef = TypedDict(
@@ -623,14 +966,34 @@
 )
 
 class ListNodesRequestRequestTypeDef(
     _RequiredListNodesRequestRequestTypeDef, _OptionalListNodesRequestRequestTypeDef
 ):
     pass
 
+_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "ClusterArn": str,
+    },
+)
+_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
+    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
+    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
+):
+    pass
+
 _RequiredListScramSecretsRequestRequestTypeDef = TypedDict(
     "_RequiredListScramSecretsRequestRequestTypeDef",
     {
         "ClusterArn": str,
     },
 )
 _OptionalListScramSecretsRequestRequestTypeDef = TypedDict(
@@ -643,329 +1006,385 @@
 )
 
 class ListScramSecretsRequestRequestTypeDef(
     _RequiredListScramSecretsRequestRequestTypeDef, _OptionalListScramSecretsRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+ListScramSecretsResponseTypeDef = TypedDict(
+    "ListScramSecretsResponseTypeDef",
     {
-        "ResourceArn": str,
+        "NextToken": str,
+        "SecretArnList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NodeExporterInfoTypeDef = TypedDict(
-    "NodeExporterInfoTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "EnabledInBroker": bool,
+        "ResourceArn": str,
     },
 )
 
-NodeExporterTypeDef = TypedDict(
-    "NodeExporterTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "EnabledInBroker": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ZookeeperNodeInfoTypeDef = TypedDict(
-    "ZookeeperNodeInfoTypeDef",
+ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef = TypedDict(
+    "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     {
-        "AttachedENIId": str,
-        "ClientVpcIpAddress": str,
-        "Endpoints": List[str],
-        "ZookeeperId": float,
-        "ZookeeperVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-RebootBrokerRequestRequestTypeDef = TypedDict(
-    "RebootBrokerRequestRequestTypeDef",
+ListVpcConnectionsRequestRequestTypeDef = TypedDict(
+    "ListVpcConnectionsRequestRequestTypeDef",
     {
-        "BrokerIds": Sequence[str],
-        "ClusterArn": str,
-    },
-)
-
-ScramTypeDef = TypedDict(
-    "ScramTypeDef",
-    {
-        "Enabled": bool,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-_RequiredVpcConfigTypeDef = TypedDict(
-    "_RequiredVpcConfigTypeDef",
+_RequiredVpcConnectionTypeDef = TypedDict(
+    "_RequiredVpcConnectionTypeDef",
     {
-        "SubnetIds": Sequence[str],
+        "VpcConnectionArn": str,
+        "TargetClusterArn": str,
     },
 )
-_OptionalVpcConfigTypeDef = TypedDict(
-    "_OptionalVpcConfigTypeDef",
+_OptionalVpcConnectionTypeDef = TypedDict(
+    "_OptionalVpcConnectionTypeDef",
     {
-        "SecurityGroupIds": Sequence[str],
+        "CreationTime": datetime,
+        "Authentication": str,
+        "VpcId": str,
+        "State": VpcConnectionStateType,
     },
     total=False,
 )
 
-class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
+class VpcConnectionTypeDef(_RequiredVpcConnectionTypeDef, _OptionalVpcConnectionTypeDef):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+NodeExporterInfoTypeDef = TypedDict(
+    "NodeExporterInfoTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "EnabledInBroker": bool,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+NodeExporterTypeDef = TypedDict(
+    "NodeExporterTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "EnabledInBroker": bool,
     },
 )
 
-UpdateBrokerCountRequestRequestTypeDef = TypedDict(
-    "UpdateBrokerCountRequestRequestTypeDef",
+ZookeeperNodeInfoTypeDef = TypedDict(
+    "ZookeeperNodeInfoTypeDef",
     {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-        "TargetNumberOfBrokerNodes": int,
+        "AttachedENIId": str,
+        "ClientVpcIpAddress": str,
+        "Endpoints": List[str],
+        "ZookeeperId": float,
+        "ZookeeperVersion": str,
     },
+    total=False,
 )
 
-UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
-    "UpdateBrokerTypeRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterArn": str,
-        "CurrentVersion": str,
-        "TargetInstanceType": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+_RequiredPutClusterPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutClusterPolicyRequestRequestTypeDef",
     {
-        "Arn": str,
-        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
+        "ClusterArn": str,
+        "Policy": str,
     },
 )
-_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+_OptionalPutClusterPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutClusterPolicyRequestRequestTypeDef",
     {
-        "Description": str,
+        "CurrentVersion": str,
     },
     total=False,
 )
 
-class UpdateConfigurationRequestRequestTypeDef(
-    _RequiredUpdateConfigurationRequestRequestTypeDef,
-    _OptionalUpdateConfigurationRequestRequestTypeDef,
+class PutClusterPolicyRequestRequestTypeDef(
+    _RequiredPutClusterPolicyRequestRequestTypeDef, _OptionalPutClusterPolicyRequestRequestTypeDef
 ):
     pass
 
-CreateClusterResponseTypeDef = TypedDict(
-    "CreateClusterResponseTypeDef",
+PutClusterPolicyResponseTypeDef = TypedDict(
+    "PutClusterPolicyResponseTypeDef",
     {
-        "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CurrentVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateClusterV2ResponseTypeDef = TypedDict(
-    "CreateClusterV2ResponseTypeDef",
+RebootBrokerRequestRequestTypeDef = TypedDict(
+    "RebootBrokerRequestRequestTypeDef",
     {
+        "BrokerIds": Sequence[str],
         "ClusterArn": str,
-        "ClusterName": str,
-        "State": ClusterStateType,
-        "ClusterType": ClusterTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteClusterResponseTypeDef = TypedDict(
-    "DeleteClusterResponseTypeDef",
+RebootBrokerResponseTypeDef = TypedDict(
+    "RebootBrokerResponseTypeDef",
     {
         "ClusterArn": str,
-        "State": ClusterStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClusterOperationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteConfigurationResponseTypeDef = TypedDict(
-    "DeleteConfigurationResponseTypeDef",
+RejectClientVpcConnectionRequestRequestTypeDef = TypedDict(
+    "RejectClientVpcConnectionRequestRequestTypeDef",
     {
-        "Arn": str,
-        "State": ConfigurationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClusterArn": str,
+        "VpcConnectionArn": str,
     },
 )
 
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "CreationTime": datetime,
-        "Description": str,
-        "Revision": int,
-        "ServerProperties": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ScramTypeDef = TypedDict(
+    "ScramTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Enabled": bool,
     },
+    total=False,
 )
 
-GetBootstrapBrokersResponseTypeDef = TypedDict(
-    "GetBootstrapBrokersResponseTypeDef",
+_RequiredVpcConfigTypeDef = TypedDict(
+    "_RequiredVpcConfigTypeDef",
     {
-        "BootstrapBrokerString": str,
-        "BootstrapBrokerStringTls": str,
-        "BootstrapBrokerStringSaslScram": str,
-        "BootstrapBrokerStringSaslIam": str,
-        "BootstrapBrokerStringPublicTls": str,
-        "BootstrapBrokerStringPublicSaslScram": str,
-        "BootstrapBrokerStringPublicSaslIam": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SubnetIds": Sequence[str],
     },
 )
+_OptionalVpcConfigTypeDef = TypedDict(
+    "_OptionalVpcConfigTypeDef",
+    {
+        "SecurityGroupIds": Sequence[str],
+    },
+    total=False,
+)
 
-ListScramSecretsResponseTypeDef = TypedDict(
-    "ListScramSecretsResponseTypeDef",
+class VpcConfigTypeDef(_RequiredVpcConfigTypeDef, _OptionalVpcConfigTypeDef):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "SecretArnList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-RebootBrokerResponseTypeDef = TypedDict(
-    "RebootBrokerResponseTypeDef",
+UpdateBrokerCountRequestRequestTypeDef = TypedDict(
+    "UpdateBrokerCountRequestRequestTypeDef",
     {
         "ClusterArn": str,
-        "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CurrentVersion": str,
+        "TargetNumberOfBrokerNodes": int,
     },
 )
 
 UpdateBrokerCountResponseTypeDef = TypedDict(
     "UpdateBrokerCountResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBrokerStorageResponseTypeDef = TypedDict(
     "UpdateBrokerStorageResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBrokerTypeRequestRequestTypeDef = TypedDict(
+    "UpdateBrokerTypeRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+        "CurrentVersion": str,
+        "TargetInstanceType": str,
     },
 )
 
 UpdateBrokerTypeResponseTypeDef = TypedDict(
     "UpdateBrokerTypeResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterConfigurationResponseTypeDef = TypedDict(
     "UpdateClusterConfigurationResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterKafkaVersionResponseTypeDef = TypedDict(
     "UpdateClusterKafkaVersionResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Arn": str,
+        "ServerProperties": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
+_OptionalUpdateConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateConfigurationRequestRequestTypeDef(
+    _RequiredUpdateConfigurationRequestRequestTypeDef,
+    _OptionalUpdateConfigurationRequestRequestTypeDef,
+):
+    pass
 
 UpdateConnectivityResponseTypeDef = TypedDict(
     "UpdateConnectivityResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMonitoringResponseTypeDef = TypedDict(
     "UpdateMonitoringResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSecurityResponseTypeDef = TypedDict(
     "UpdateSecurityResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStorageResponseTypeDef = TypedDict(
     "UpdateStorageResponseTypeDef",
     {
         "ClusterArn": str,
         "ClusterOperationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
+    {
+        "Type": UserIdentityTypeType,
+        "PrincipalId": str,
     },
+    total=False,
+)
+
+VpcConnectivityTlsTypeDef = TypedDict(
+    "VpcConnectivityTlsTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityIamTypeDef = TypedDict(
+    "VpcConnectivityIamTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
+)
+
+VpcConnectivityScramTypeDef = TypedDict(
+    "VpcConnectivityScramTypeDef",
+    {
+        "Enabled": bool,
+    },
+    total=False,
 )
 
 BatchAssociateScramSecretResponseTypeDef = TypedDict(
     "BatchAssociateScramSecretResponseTypeDef",
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateScramSecretResponseTypeDef = TypedDict(
     "BatchDisassociateScramSecretResponseTypeDef",
     {
         "ClusterArn": str,
         "UnprocessedScramSecrets": List[UnprocessedScramSecretTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBrokerEBSVolumeInfoTypeDef = TypedDict(
     "_RequiredBrokerEBSVolumeInfoTypeDef",
     {
         "KafkaBrokerNodeId": str,
@@ -1035,28 +1454,37 @@
         "ClientVpcIpAddress": str,
         "CurrentBrokerSoftwareInfo": BrokerSoftwareInfoTypeDef,
         "Endpoints": List[str],
     },
     total=False,
 )
 
+ListClientVpcConnectionsResponseTypeDef = TypedDict(
+    "ListClientVpcConnectionsResponseTypeDef",
+    {
+        "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": ClusterOperationStepInfoTypeDef,
         "StepName": str,
     },
     total=False,
 )
 
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateClusterConfigurationRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1104,58 +1532,50 @@
     "CreateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConfigurationResponseTypeDef = TypedDict(
     "DescribeConfigurationResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "Description": str,
         "KafkaVersions": List[str],
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "State": ConfigurationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfigurationRevisionsResponseTypeDef = TypedDict(
     "ListConfigurationRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfigurationResponseTypeDef = TypedDict(
     "UpdateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ConnectivityInfoTypeDef = TypedDict(
-    "ConnectivityInfoTypeDef",
-    {
-        "PublicAccess": PublicAccessTypeDef,
-    },
-    total=False,
-)
-
 EncryptionInfoTypeDef = TypedDict(
     "EncryptionInfoTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "EncryptionInTransit": EncryptionInTransitTypeDef,
     },
     total=False,
@@ -1170,133 +1590,27 @@
 )
 
 ListKafkaVersionsResponseTypeDef = TypedDict(
     "ListKafkaVersionsResponseTypeDef",
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListClusterOperationsRequestListClusterOperationsPaginateTypeDef(
-    _RequiredListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    _OptionalListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "ClusterNameFilter": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListClustersV2RequestListClustersV2PaginateTypeDef = TypedDict(
-    "ListClustersV2RequestListClustersV2PaginateTypeDef",
-    {
-        "ClusterNameFilter": str,
-        "ClusterTypeFilter": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef(
-    _RequiredListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    _OptionalListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-):
-    pass
-
-ListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
-    "ListConfigurationsRequestListConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef = TypedDict(
-    "ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_RequiredListNodesRequestListNodesPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListNodesRequestListNodesPaginateTypeDef = TypedDict(
-    "_OptionalListNodesRequestListNodesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListNodesRequestListNodesPaginateTypeDef(
-    _RequiredListNodesRequestListNodesPaginateTypeDef,
-    _OptionalListNodesRequestListNodesPaginateTypeDef,
-):
-    pass
-
-_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef",
-    {
-        "ClusterArn": str,
-    },
-)
-_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef = TypedDict(
-    "_OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef",
+ListVpcConnectionsResponseTypeDef = TypedDict(
+    "ListVpcConnectionsResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "VpcConnections": List[VpcConnectionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListScramSecretsRequestListScramSecretsPaginateTypeDef(
-    _RequiredListScramSecretsRequestListScramSecretsPaginateTypeDef,
-    _OptionalListScramSecretsRequestListScramSecretsPaginateTypeDef,
-):
-    pass
-
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": JmxExporterInfoTypeDef,
         "NodeExporter": NodeExporterInfoTypeDef,
     },
     total=False,
@@ -1316,14 +1630,34 @@
     {
         "Scram": ScramTypeDef,
         "Iam": IamTypeDef,
     },
     total=False,
 )
 
+VpcConnectionInfoTypeDef = TypedDict(
+    "VpcConnectionInfoTypeDef",
+    {
+        "VpcConnectionArn": str,
+        "Owner": str,
+        "UserIdentity": UserIdentityTypeDef,
+        "CreationTime": datetime,
+    },
+    total=False,
+)
+
+VpcConnectivitySaslTypeDef = TypedDict(
+    "VpcConnectivitySaslTypeDef",
+    {
+        "Scram": VpcConnectivityScramTypeDef,
+        "Iam": VpcConnectivityIamTypeDef,
+    },
+    total=False,
+)
+
 UpdateBrokerStorageRequestRequestTypeDef = TypedDict(
     "UpdateBrokerStorageRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "TargetBrokerEBSVolumeInfo": Sequence[BrokerEBSVolumeInfoTypeDef],
     },
@@ -1358,24 +1692,15 @@
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateConnectivityRequestRequestTypeDef = TypedDict(
-    "UpdateConnectivityRequestRequestTypeDef",
-    {
-        "ClusterArn": str,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
-        "CurrentVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": ServerlessSaslTypeDef,
@@ -1403,43 +1728,29 @@
         "Sasl": SaslTypeDef,
         "Tls": TlsTypeDef,
         "Unauthenticated": UnauthenticatedTypeDef,
     },
     total=False,
 )
 
-_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_RequiredBrokerNodeGroupInfoTypeDef",
+VpcConnectivityClientAuthenticationTypeDef = TypedDict(
+    "VpcConnectivityClientAuthenticationTypeDef",
     {
-        "ClientSubnets": Sequence[str],
-        "InstanceType": str,
-    },
-)
-_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
-    "_OptionalBrokerNodeGroupInfoTypeDef",
-    {
-        "BrokerAZDistribution": Literal["DEFAULT"],
-        "SecurityGroups": Sequence[str],
-        "StorageInfo": StorageInfoTypeDef,
-        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "Sasl": VpcConnectivitySaslTypeDef,
+        "Tls": VpcConnectivityTlsTypeDef,
     },
     total=False,
 )
 
-class BrokerNodeGroupInfoTypeDef(
-    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
-):
-    pass
-
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredServerlessRequestTypeDef = TypedDict(
     "_RequiredServerlessRequestTypeDef",
     {
         "VpcConfigs": Sequence[VpcConfigTypeDef],
@@ -1493,14 +1804,76 @@
 )
 
 class UpdateMonitoringRequestRequestTypeDef(
     _RequiredUpdateMonitoringRequestRequestTypeDef, _OptionalUpdateMonitoringRequestRequestTypeDef
 ):
     pass
 
+_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecurityRequestRequestTypeDef",
+    {
+        "ClusterArn": str,
+        "CurrentVersion": str,
+    },
+)
+_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecurityRequestRequestTypeDef",
+    {
+        "ClientAuthentication": ClientAuthenticationTypeDef,
+        "EncryptionInfo": EncryptionInfoTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSecurityRequestRequestTypeDef(
+    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
+):
+    pass
+
+VpcConnectivityTypeDef = TypedDict(
+    "VpcConnectivityTypeDef",
+    {
+        "ClientAuthentication": VpcConnectivityClientAuthenticationTypeDef,
+    },
+    total=False,
+)
+
+ConnectivityInfoTypeDef = TypedDict(
+    "ConnectivityInfoTypeDef",
+    {
+        "PublicAccess": PublicAccessTypeDef,
+        "VpcConnectivity": VpcConnectivityTypeDef,
+    },
+    total=False,
+)
+
+_RequiredBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_RequiredBrokerNodeGroupInfoTypeDef",
+    {
+        "ClientSubnets": Sequence[str],
+        "InstanceType": str,
+    },
+)
+_OptionalBrokerNodeGroupInfoTypeDef = TypedDict(
+    "_OptionalBrokerNodeGroupInfoTypeDef",
+    {
+        "BrokerAZDistribution": Literal["DEFAULT"],
+        "SecurityGroups": Sequence[str],
+        "StorageInfo": StorageInfoTypeDef,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
+        "ZoneIds": Sequence[str],
+    },
+    total=False,
+)
+
+class BrokerNodeGroupInfoTypeDef(
+    _RequiredBrokerNodeGroupInfoTypeDef, _OptionalBrokerNodeGroupInfoTypeDef
+):
+    pass
+
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": List[BrokerEBSVolumeInfoTypeDef],
         "ConfigurationInfo": ConfigurationInfoTypeDef,
         "NumberOfBrokerNodes": int,
         "EnhancedMonitoring": EnhancedMonitoringType,
@@ -1512,34 +1885,22 @@
         "EncryptionInfo": EncryptionInfoTypeDef,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "StorageMode": StorageModeType,
     },
     total=False,
 )
 
-_RequiredUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecurityRequestRequestTypeDef",
+UpdateConnectivityRequestRequestTypeDef = TypedDict(
+    "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
+        "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
-_OptionalUpdateSecurityRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecurityRequestRequestTypeDef",
-    {
-        "ClientAuthentication": ClientAuthenticationTypeDef,
-        "EncryptionInfo": EncryptionInfoTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSecurityRequestRequestTypeDef(
-    _RequiredUpdateSecurityRequestRequestTypeDef, _OptionalUpdateSecurityRequestRequestTypeDef
-):
-    pass
 
 ClusterInfoTypeDef = TypedDict(
     "ClusterInfoTypeDef",
     {
         "ActiveOperationArn": str,
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClientAuthentication": ClientAuthenticationTypeDef,
@@ -1655,32 +2016,33 @@
         "ErrorInfo": ErrorInfoTypeDef,
         "OperationArn": str,
         "OperationState": str,
         "OperationSteps": List[ClusterOperationStepTypeDef],
         "OperationType": str,
         "SourceClusterInfo": MutableClusterInfoTypeDef,
         "TargetClusterInfo": MutableClusterInfoTypeDef,
+        "VpcConnectionInfo": VpcConnectionInfoTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateClusterV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterV2RequestRequestTypeDef",
     {
         "ClusterName": str,
@@ -1719,36 +2081,36 @@
     total=False,
 )
 
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClusterOperationsResponseTypeDef = TypedDict(
     "ListClusterOperationsResponseTypeDef",
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersV2ResponseTypeDef = TypedDict(
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.27.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kafka
-Version: 1.26.60
-Summary: Type annotations for boto3.Kafka 1.26.60 service generated with mypy-boto3-builder 7.12.3
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kafka type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-kafka"></a>
 
 # mypy-boto3-kafka
 
 [![PyPI - mypy-boto3-kafka](https://img.shields.io/pypi/v/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kafka?color=blue)](https://pypistats.org/packages/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
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
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,28 +247,33 @@
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_kafka import KafkaClient
 from mypy_boto3_kafka.paginator import (
+    ListClientVpcConnectionsPaginator,
     ListClusterOperationsPaginator,
     ListClustersPaginator,
     ListClustersV2Paginator,
     ListConfigurationRevisionsPaginator,
     ListConfigurationsPaginator,
     ListKafkaVersionsPaginator,
     ListNodesPaginator,
     ListScramSecretsPaginator,
+    ListVpcConnectionsPaginator,
 )
 
 client: KafkaClient = Session().client("kafka")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
+list_client_vpc_connections_paginator: ListClientVpcConnectionsPaginator = client.get_paginator(
+    "list_client_vpc_connections"
+)
 list_cluster_operations_paginator: ListClusterOperationsPaginator = client.get_paginator(
     "list_cluster_operations"
 )
 list_clusters_paginator: ListClustersPaginator = client.get_paginator("list_clusters")
 list_clusters_v2_paginator: ListClustersV2Paginator = client.get_paginator("list_clusters_v2")
 list_configuration_revisions_paginator: ListConfigurationRevisionsPaginator = client.get_paginator(
     "list_configuration_revisions"
@@ -309,14 +282,17 @@
     "list_configurations"
 )
 list_kafka_versions_paginator: ListKafkaVersionsPaginator = client.get_paginator(
     "list_kafka_versions"
 )
 list_nodes_paginator: ListNodesPaginator = client.get_paginator("list_nodes")
 list_scram_secrets_paginator: ListScramSecretsPaginator = client.get_paginator("list_scram_secrets")
+list_vpc_connections_paginator: ListVpcConnectionsPaginator = client.get_paginator(
+    "list_vpc_connections"
+)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kafka.literals` module contains literals extracted from shapes that
@@ -327,24 +303,28 @@
     BrokerAZDistributionType,
     ClientBrokerType,
     ClusterStateType,
     ClusterTypeType,
     ConfigurationStateType,
     EnhancedMonitoringType,
     KafkaVersionStatusType,
+    ListClientVpcConnectionsPaginatorName,
     ListClusterOperationsPaginatorName,
     ListClustersPaginatorName,
     ListClustersV2PaginatorName,
     ListConfigurationRevisionsPaginatorName,
     ListConfigurationsPaginatorName,
     ListKafkaVersionsPaginatorName,
     ListNodesPaginatorName,
     ListScramSecretsPaginatorName,
+    ListVpcConnectionsPaginatorName,
     NodeTypeType,
     StorageModeType,
+    UserIdentityTypeType,
+    VpcConnectionStateType,
     KafkaServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
@@ -359,135 +339,163 @@
 
 `mypy_boto3_kafka.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kafka.type_defs import (
     BatchAssociateScramSecretRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UnprocessedScramSecretTypeDef,
     BatchDisassociateScramSecretRequestRequestTypeDef,
     ProvisionedThroughputTypeDef,
     CloudWatchLogsTypeDef,
     FirehoseTypeDef,
     S3TypeDef,
     BrokerSoftwareInfoTypeDef,
     TlsTypeDef,
     UnauthenticatedTypeDef,
+    ClientVpcConnectionTypeDef,
     StateInfoTypeDef,
     ErrorInfoTypeDef,
     ClusterOperationStepInfoTypeDef,
     CompatibleKafkaVersionTypeDef,
     ConfigurationInfoTypeDef,
     ConfigurationRevisionTypeDef,
     PublicAccessTypeDef,
+    CreateClusterResponseTypeDef,
+    CreateClusterV2ResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
+    CreateVpcConnectionRequestRequestTypeDef,
+    CreateVpcConnectionResponseTypeDef,
+    DeleteClusterPolicyRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
+    DeleteClusterResponseTypeDef,
     DeleteConfigurationRequestRequestTypeDef,
+    DeleteConfigurationResponseTypeDef,
+    DeleteVpcConnectionRequestRequestTypeDef,
+    DeleteVpcConnectionResponseTypeDef,
     DescribeClusterOperationRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeClusterV2RequestRequestTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    DescribeVpcConnectionRequestRequestTypeDef,
+    DescribeVpcConnectionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionAtRestTypeDef,
     EncryptionInTransitTypeDef,
     GetBootstrapBrokersRequestRequestTypeDef,
+    GetBootstrapBrokersResponseTypeDef,
+    GetClusterPolicyRequestRequestTypeDef,
+    GetClusterPolicyResponseTypeDef,
     GetCompatibleKafkaVersionsRequestRequestTypeDef,
     IamTypeDef,
     JmxExporterInfoTypeDef,
     JmxExporterTypeDef,
     KafkaVersionTypeDef,
-    PaginatorConfigTypeDef,
+    ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef,
+    ListClientVpcConnectionsRequestRequestTypeDef,
+    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
     ListClusterOperationsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersV2RequestListClustersV2PaginateTypeDef,
     ListClustersV2RequestRequestTypeDef,
+    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
+    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
     ListConfigurationsRequestRequestTypeDef,
+    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
     ListKafkaVersionsRequestRequestTypeDef,
+    ListNodesRequestListNodesPaginateTypeDef,
     ListNodesRequestRequestTypeDef,
+    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
     ListScramSecretsRequestRequestTypeDef,
+    ListScramSecretsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef,
+    ListVpcConnectionsRequestRequestTypeDef,
+    VpcConnectionTypeDef,
     NodeExporterInfoTypeDef,
     NodeExporterTypeDef,
     ZookeeperNodeInfoTypeDef,
+    PaginatorConfigTypeDef,
+    PutClusterPolicyRequestRequestTypeDef,
+    PutClusterPolicyResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
+    RebootBrokerResponseTypeDef,
+    RejectClientVpcConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ScramTypeDef,
     VpcConfigTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBrokerCountRequestRequestTypeDef,
-    UpdateBrokerTypeRequestRequestTypeDef,
-    UpdateConfigurationRequestRequestTypeDef,
-    CreateClusterResponseTypeDef,
-    CreateClusterV2ResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DeleteConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBootstrapBrokersResponseTypeDef,
-    ListScramSecretsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RebootBrokerResponseTypeDef,
     UpdateBrokerCountResponseTypeDef,
     UpdateBrokerStorageResponseTypeDef,
+    UpdateBrokerTypeRequestRequestTypeDef,
     UpdateBrokerTypeResponseTypeDef,
     UpdateClusterConfigurationResponseTypeDef,
     UpdateClusterKafkaVersionResponseTypeDef,
+    UpdateConfigurationRequestRequestTypeDef,
     UpdateConnectivityResponseTypeDef,
     UpdateMonitoringResponseTypeDef,
     UpdateSecurityResponseTypeDef,
     UpdateStorageResponseTypeDef,
+    UserIdentityTypeDef,
+    VpcConnectivityTlsTypeDef,
+    VpcConnectivityIamTypeDef,
+    VpcConnectivityScramTypeDef,
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
     EBSStorageInfoTypeDef,
     UpdateStorageRequestRequestTypeDef,
     BrokerLogsTypeDef,
     BrokerNodeInfoTypeDef,
+    ListClientVpcConnectionsResponseTypeDef,
     ClusterOperationStepTypeDef,
     GetCompatibleKafkaVersionsResponseTypeDef,
     UpdateClusterConfigurationRequestRequestTypeDef,
     UpdateClusterKafkaVersionRequestRequestTypeDef,
     ConfigurationTypeDef,
     CreateConfigurationResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     UpdateConfigurationResponseTypeDef,
-    ConnectivityInfoTypeDef,
     EncryptionInfoTypeDef,
     ServerlessSaslTypeDef,
     ListKafkaVersionsResponseTypeDef,
-    ListClusterOperationsRequestListClusterOperationsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListClustersV2RequestListClustersV2PaginateTypeDef,
-    ListConfigurationRevisionsRequestListConfigurationRevisionsPaginateTypeDef,
-    ListConfigurationsRequestListConfigurationsPaginateTypeDef,
-    ListKafkaVersionsRequestListKafkaVersionsPaginateTypeDef,
-    ListNodesRequestListNodesPaginateTypeDef,
-    ListScramSecretsRequestListScramSecretsPaginateTypeDef,
+    ListVpcConnectionsResponseTypeDef,
     PrometheusInfoTypeDef,
     PrometheusTypeDef,
     SaslTypeDef,
+    VpcConnectionInfoTypeDef,
+    VpcConnectivitySaslTypeDef,
     UpdateBrokerStorageRequestRequestTypeDef,
     StorageInfoTypeDef,
     LoggingInfoTypeDef,
     NodeInfoTypeDef,
     ListConfigurationsResponseTypeDef,
-    UpdateConnectivityRequestRequestTypeDef,
     ServerlessClientAuthenticationTypeDef,
     OpenMonitoringInfoTypeDef,
     OpenMonitoringTypeDef,
     ClientAuthenticationTypeDef,
-    BrokerNodeGroupInfoTypeDef,
+    VpcConnectivityClientAuthenticationTypeDef,
     ListNodesResponseTypeDef,
     ServerlessRequestTypeDef,
     ServerlessTypeDef,
     UpdateMonitoringRequestRequestTypeDef,
-    MutableClusterInfoTypeDef,
     UpdateSecurityRequestRequestTypeDef,
+    VpcConnectivityTypeDef,
+    ConnectivityInfoTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    MutableClusterInfoTypeDef,
+    UpdateConnectivityRequestRequestTypeDef,
     ClusterInfoTypeDef,
     CreateClusterRequestRequestTypeDef,
     ProvisionedRequestTypeDef,
     ProvisionedTypeDef,
     ClusterOperationInfoTypeDef,
     DescribeClusterResponseTypeDef,
     ListClustersResponseTypeDef,
@@ -507,42 +515,42 @@
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

### Comparing `mypy-boto3-kafka-1.26.60/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.27.0/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.26.60/setup.py` & `mypy-boto3-kafka-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-kafka.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.26.60",
+    version="1.27.0",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kafka 1.26.60 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Kafka 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/",
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


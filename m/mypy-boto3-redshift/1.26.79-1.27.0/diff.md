# Comparing `tmp/mypy-boto3-redshift-1.26.79.tar.gz` & `tmp/mypy-boto3-redshift-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-1.27.0.tar", last modified: Mon Jul  3 19:51:19 2023, max compression
```

## Comparing `mypy-boto3-redshift-1.26.79.tar` & `mypy-boto3-redshift-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34736 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   112008 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   111846 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-02-24 21:22:13.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42229 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42195 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   130787 2023-02-24 21:22:17.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   130668 2023-02-24 21:22:15.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.259870 mypy-boto3-redshift-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36979 2023-07-03 19:51:19.259870 mypy-boto3-redshift-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35490 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.259870 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115402 2023-07-03 19:46:02.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115235 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-03 19:46:03.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-07-03 19:46:03.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43616 2023-07-03 19:46:03.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43581 2023-07-03 19:46:02.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   134445 2023-07-03 19:46:05.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134326 2023-07-03 19:46:04.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-03 19:46:03.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-03 19:46:03.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.259870 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36979 2023-07-03 19:51:19.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-03 19:51:19.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:19.000000 mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:19.259870 mypy-boto3-redshift-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:45:59.000000 mypy-boto3-redshift-1.27.0/setup.py
```

### Comparing `mypy-boto3-redshift-1.26.79/LICENSE` & `mypy-boto3-redshift-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-redshift-1.26.79/PKG-INFO` & `mypy-boto3-redshift-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.26.79
-Summary: Type annotations for boto3.Redshift 1.26.79 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.Redshift 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-redshift"></a>
 
 # mypy-boto3-redshift
 
 [![PyPI - mypy-boto3-redshift](https://img.shields.io/pypi/v/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +289,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
     DescribeClustersPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventSubscriptionsPaginator,
@@ -343,14 +344,17 @@
 describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator(
     "describe_cluster_tracks"
 )
 describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator(
     "describe_cluster_versions"
 )
 describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = (
+    client.get_paginator("describe_custom_domain_associations")
+)
 describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator(
     "describe_data_shares"
 )
 describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = (
     client.get_paginator("describe_data_shares_for_consumer")
 )
 describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = (
@@ -465,14 +469,15 @@
     DescribeClusterParametersPaginatorName,
     DescribeClusterSecurityGroupsPaginatorName,
     DescribeClusterSnapshotsPaginatorName,
     DescribeClusterSubnetGroupsPaginatorName,
     DescribeClusterTracksPaginatorName,
     DescribeClusterVersionsPaginatorName,
     DescribeClustersPaginatorName,
+    DescribeCustomDomainAssociationsPaginatorName,
     DescribeDataSharesForConsumerPaginatorName,
     DescribeDataSharesForProducerPaginatorName,
     DescribeDataSharesPaginatorName,
     DescribeDefaultClusterParametersPaginatorName,
     DescribeEndpointAccessPaginatorName,
     DescribeEndpointAuthorizationPaginatorName,
     DescribeEventSubscriptionsPaginatorName,
@@ -533,34 +538,37 @@
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
+    CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     AuthorizeDataShareMessageRequestTypeDef,
     AuthorizeEndpointAccessMessageRequestTypeDef,
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
+    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
+    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
     ParameterTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
     ClusterParameterStatusTypeDef,
     TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
@@ -569,133 +577,168 @@
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationMessageRequestTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
+    CustomerStorageMessageTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
+    DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteHsmClientCertificateMessageRequestTypeDef,
     DeleteHsmConfigurationMessageRequestTypeDef,
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageRequestTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
+    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
+    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
+    ModifyCustomDomainAssociationMessageRequestTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
+    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
+    ResizeProgressMessageTypeDef,
+    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
-    ClusterCredentialsTypeDef,
-    ClusterExtendedCredentialsTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
-    CustomerStorageMessageTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
-    LoggingStatusTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
-    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
+    AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
@@ -728,43 +771,14 @@
     TaggedResourceTypeDef,
     UsageLimitResponseMetadataTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
     DataShareResponseMetadataTypeDef,
     DataShareTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -780,14 +794,15 @@
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
     DescribeDefaultClusterParametersResultTypeDef,
     ClusterParameterGroupsMessageTypeDef,
     CreateClusterParameterGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
@@ -868,42 +883,42 @@
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

### Comparing `mypy-boto3-redshift-1.26.79/README.md` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-redshift
+Version: 1.27.0
+Summary: Type annotations for boto3.Redshift 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 redshift type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-redshift"></a>
 
 # mypy-boto3-redshift
 
 [![PyPI - mypy-boto3-redshift](https://img.shields.io/pypi/v/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,14 +289,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
     DescribeClustersPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventSubscriptionsPaginator,
@@ -311,14 +344,17 @@
 describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator(
     "describe_cluster_tracks"
 )
 describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator(
     "describe_cluster_versions"
 )
 describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = (
+    client.get_paginator("describe_custom_domain_associations")
+)
 describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator(
     "describe_data_shares"
 )
 describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = (
     client.get_paginator("describe_data_shares_for_consumer")
 )
 describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = (
@@ -433,14 +469,15 @@
     DescribeClusterParametersPaginatorName,
     DescribeClusterSecurityGroupsPaginatorName,
     DescribeClusterSnapshotsPaginatorName,
     DescribeClusterSubnetGroupsPaginatorName,
     DescribeClusterTracksPaginatorName,
     DescribeClusterVersionsPaginatorName,
     DescribeClustersPaginatorName,
+    DescribeCustomDomainAssociationsPaginatorName,
     DescribeDataSharesForConsumerPaginatorName,
     DescribeDataSharesForProducerPaginatorName,
     DescribeDataSharesPaginatorName,
     DescribeDefaultClusterParametersPaginatorName,
     DescribeEndpointAccessPaginatorName,
     DescribeEndpointAuthorizationPaginatorName,
     DescribeEventSubscriptionsPaginatorName,
@@ -501,34 +538,37 @@
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
+    CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     AuthorizeDataShareMessageRequestTypeDef,
     AuthorizeEndpointAccessMessageRequestTypeDef,
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
+    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
+    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
     ParameterTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
     ClusterParameterStatusTypeDef,
     TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
@@ -537,133 +577,168 @@
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationMessageRequestTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
+    CustomerStorageMessageTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
+    DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteHsmClientCertificateMessageRequestTypeDef,
     DeleteHsmConfigurationMessageRequestTypeDef,
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageRequestTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
+    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
+    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
+    ModifyCustomDomainAssociationMessageRequestTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
+    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
+    ResizeProgressMessageTypeDef,
+    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
-    ClusterCredentialsTypeDef,
-    ClusterExtendedCredentialsTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
-    CustomerStorageMessageTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
-    LoggingStatusTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
-    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
+    AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
@@ -696,43 +771,14 @@
     TaggedResourceTypeDef,
     UsageLimitResponseMetadataTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
     DataShareResponseMetadataTypeDef,
     DataShareTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -748,14 +794,15 @@
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
     DescribeDefaultClusterParametersResultTypeDef,
     ClusterParameterGroupsMessageTypeDef,
     CreateClusterParameterGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
@@ -836,42 +883,42 @@
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

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         DescribeClusterParametersPaginator,
         DescribeClusterSecurityGroupsPaginator,
         DescribeClusterSnapshotsPaginator,
         DescribeClusterSubnetGroupsPaginator,
         DescribeClusterTracksPaginator,
         DescribeClusterVersionsPaginator,
         DescribeClustersPaginator,
+        DescribeCustomDomainAssociationsPaginator,
         DescribeDataSharesForConsumerPaginator,
         DescribeDataSharesForProducerPaginator,
         DescribeDataSharesPaginator,
         DescribeDefaultClusterParametersPaginator,
         DescribeEndpointAccessPaginator,
         DescribeEndpointAuthorizationPaginator,
         DescribeEventSubscriptionsPaginator,
@@ -59,14 +60,15 @@
     describe_cluster_parameters_paginator: DescribeClusterParametersPaginator = client.get_paginator("describe_cluster_parameters")
     describe_cluster_security_groups_paginator: DescribeClusterSecurityGroupsPaginator = client.get_paginator("describe_cluster_security_groups")
     describe_cluster_snapshots_paginator: DescribeClusterSnapshotsPaginator = client.get_paginator("describe_cluster_snapshots")
     describe_cluster_subnet_groups_paginator: DescribeClusterSubnetGroupsPaginator = client.get_paginator("describe_cluster_subnet_groups")
     describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator("describe_cluster_tracks")
     describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator("describe_cluster_versions")
     describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+    describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = client.get_paginator("describe_custom_domain_associations")
     describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator("describe_data_shares")
     describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = client.get_paginator("describe_data_shares_for_consumer")
     describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = client.get_paginator("describe_data_shares_for_producer")
     describe_default_cluster_parameters_paginator: DescribeDefaultClusterParametersPaginator = client.get_paginator("describe_default_cluster_parameters")
     describe_endpoint_access_paginator: DescribeEndpointAccessPaginator = client.get_paginator("describe_endpoint_access")
     describe_endpoint_authorization_paginator: DescribeEndpointAuthorizationPaginator = client.get_paginator("describe_endpoint_authorization")
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
@@ -95,14 +97,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClustersPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDataSharesPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventsPaginator,
@@ -143,14 +146,15 @@
     "DescribeClusterParametersPaginator",
     "DescribeClusterSecurityGroupsPaginator",
     "DescribeClusterSnapshotsPaginator",
     "DescribeClusterSubnetGroupsPaginator",
     "DescribeClusterTracksPaginator",
     "DescribeClusterVersionsPaginator",
     "DescribeClustersPaginator",
+    "DescribeCustomDomainAssociationsPaginator",
     "DescribeDataSharesForConsumerPaginator",
     "DescribeDataSharesForProducerPaginator",
     "DescribeDataSharesPaginator",
     "DescribeDefaultClusterParametersPaginator",
     "DescribeEndpointAccessPaginator",
     "DescribeEndpointAuthorizationPaginator",
     "DescribeEventSubscriptionsPaginator",
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.pyi` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         DescribeClusterParametersPaginator,
         DescribeClusterSecurityGroupsPaginator,
         DescribeClusterSnapshotsPaginator,
         DescribeClusterSubnetGroupsPaginator,
         DescribeClusterTracksPaginator,
         DescribeClusterVersionsPaginator,
         DescribeClustersPaginator,
+        DescribeCustomDomainAssociationsPaginator,
         DescribeDataSharesForConsumerPaginator,
         DescribeDataSharesForProducerPaginator,
         DescribeDataSharesPaginator,
         DescribeDefaultClusterParametersPaginator,
         DescribeEndpointAccessPaginator,
         DescribeEndpointAuthorizationPaginator,
         DescribeEventSubscriptionsPaginator,
@@ -59,14 +60,15 @@
     describe_cluster_parameters_paginator: DescribeClusterParametersPaginator = client.get_paginator("describe_cluster_parameters")
     describe_cluster_security_groups_paginator: DescribeClusterSecurityGroupsPaginator = client.get_paginator("describe_cluster_security_groups")
     describe_cluster_snapshots_paginator: DescribeClusterSnapshotsPaginator = client.get_paginator("describe_cluster_snapshots")
     describe_cluster_subnet_groups_paginator: DescribeClusterSubnetGroupsPaginator = client.get_paginator("describe_cluster_subnet_groups")
     describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator("describe_cluster_tracks")
     describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator("describe_cluster_versions")
     describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+    describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = client.get_paginator("describe_custom_domain_associations")
     describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator("describe_data_shares")
     describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = client.get_paginator("describe_data_shares_for_consumer")
     describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = client.get_paginator("describe_data_shares_for_producer")
     describe_default_cluster_parameters_paginator: DescribeDefaultClusterParametersPaginator = client.get_paginator("describe_default_cluster_parameters")
     describe_endpoint_access_paginator: DescribeEndpointAccessPaginator = client.get_paginator("describe_endpoint_access")
     describe_endpoint_authorization_paginator: DescribeEndpointAuthorizationPaginator = client.get_paginator("describe_endpoint_authorization")
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
@@ -95,14 +97,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClustersPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDataSharesPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventsPaginator,
@@ -142,14 +145,15 @@
     "DescribeClusterParametersPaginator",
     "DescribeClusterSecurityGroupsPaginator",
     "DescribeClusterSnapshotsPaginator",
     "DescribeClusterSubnetGroupsPaginator",
     "DescribeClusterTracksPaginator",
     "DescribeClusterVersionsPaginator",
     "DescribeClustersPaginator",
+    "DescribeCustomDomainAssociationsPaginator",
     "DescribeDataSharesForConsumerPaginator",
     "DescribeDataSharesForProducerPaginator",
     "DescribeDataSharesPaginator",
     "DescribeDefaultClusterParametersPaginator",
     "DescribeEndpointAccessPaginator",
     "DescribeEndpointAuthorizationPaginator",
     "DescribeEventSubscriptionsPaginator",
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__main__.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.26.79\nVersion:         1.26.79\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.Redshift 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.79")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClustersPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDataSharesPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventsPaginator,
@@ -88,18 +89,20 @@
     CopyClusterSnapshotResultTypeDef,
     CreateAuthenticationProfileResultTypeDef,
     CreateClusterParameterGroupResultTypeDef,
     CreateClusterResultTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     CreateClusterSnapshotResultTypeDef,
     CreateClusterSubnetGroupResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateHsmClientCertificateResultTypeDef,
     CreateHsmConfigurationResultTypeDef,
     CreateSnapshotCopyGrantResultTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     CustomerStorageMessageTypeDef,
     DataShareResponseMetadataTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterResultTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     DeleteClusterSnapshotResultTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
@@ -129,14 +132,15 @@
     ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionResultTypeDef,
     ModifyClusterIamRolesResultTypeDef,
     ModifyClusterMaintenanceResultTypeDef,
     ModifyClusterResultTypeDef,
     ModifyClusterSnapshotResultTypeDef,
     ModifyClusterSubnetGroupResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     ModifySnapshotCopyRetentionPeriodResultTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ParameterTypeDef,
     PartnerIntegrationOutputMessageTypeDef,
@@ -219,14 +223,16 @@
     ClusterSnapshotNotFoundFault: Type[BotocoreClientError]
     ClusterSnapshotQuotaExceededFault: Type[BotocoreClientError]
     ClusterSubnetGroupAlreadyExistsFault: Type[BotocoreClientError]
     ClusterSubnetGroupNotFoundFault: Type[BotocoreClientError]
     ClusterSubnetGroupQuotaExceededFault: Type[BotocoreClientError]
     ClusterSubnetQuotaExceededFault: Type[BotocoreClientError]
     CopyToRegionDisabledFault: Type[BotocoreClientError]
+    CustomCnameAssociationFault: Type[BotocoreClientError]
+    CustomDomainAssociationNotFoundFault: Type[BotocoreClientError]
     DependentServiceRequestThrottlingFault: Type[BotocoreClientError]
     DependentServiceUnavailableFault: Type[BotocoreClientError]
     EndpointAlreadyExistsFault: Type[BotocoreClientError]
     EndpointAuthorizationAlreadyExistsFault: Type[BotocoreClientError]
     EndpointAuthorizationNotFoundFault: Type[BotocoreClientError]
     EndpointAuthorizationsPerClusterLimitExceededFault: Type[BotocoreClientError]
     EndpointNotFoundFault: Type[BotocoreClientError]
@@ -598,14 +604,24 @@
         """
         Creates a new Amazon Redshift subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_cluster_subnet_group)
         """
 
+    def create_custom_domain_association(
+        self, *, CustomDomainName: str, CustomDomainCertificateArn: str, ClusterIdentifier: str
+    ) -> CreateCustomDomainAssociationResultTypeDef:
+        """
+        Used to create a custom domain name for a cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_custom_domain_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_custom_domain_association)
+        """
+
     def create_endpoint_access(
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
@@ -819,14 +835,24 @@
         """
         Deletes the specified cluster subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_cluster_subnet_group)
         """
 
+    def delete_custom_domain_association(
+        self, *, ClusterIdentifier: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Contains information about deleting a custom domain association for a cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_custom_domain_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_custom_domain_association)
+        """
+
     def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseMetadataTypeDef:
         """
         Deletes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_endpoint_access)
         """
@@ -1074,14 +1100,29 @@
         cluster database properties, maintenance and backup properties, and security and
         access properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#describe_clusters)
         """
 
+    def describe_custom_domain_associations(
+        self,
+        *,
+        CustomDomainName: str = ...,
+        CustomDomainCertificateArn: str = ...,
+        MaxRecords: int = ...,
+        Marker: str = ...
+    ) -> CustomDomainAssociationsMessageTypeDef:
+        """
+        Contains information for custom domain associations for a cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_custom_domain_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#describe_custom_domain_associations)
+        """
+
     def describe_data_shares(
         self, *, DataShareArn: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeDataSharesResultTypeDef:
         """
         Shows the status of any inbound or outbound datashares available in the
         specified account.
 
@@ -1540,30 +1581,36 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#generate_presigned_url)
         """
 
     def get_cluster_credentials(
         self,
         *,
         DbUser: str,
-        ClusterIdentifier: str,
         DbName: str = ...,
+        ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
         AutoCreate: bool = ...,
-        DbGroups: Sequence[str] = ...
+        DbGroups: Sequence[str] = ...,
+        CustomDomainName: str = ...
     ) -> ClusterCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary authorization
         to log on to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_cluster_credentials)
         """
 
     def get_cluster_credentials_with_iam(
-        self, *, ClusterIdentifier: str, DbName: str = ..., DurationSeconds: int = ...
+        self,
+        *,
+        DbName: str = ...,
+        ClusterIdentifier: str = ...,
+        DurationSeconds: int = ...,
+        CustomDomainName: str = ...
     ) -> ClusterExtendedCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary authorization
         to log in to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials_with_iam)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_cluster_credentials_with_iam)
@@ -1739,14 +1786,28 @@
         """
         Modifies a cluster subnet group to include the specified list of VPC subnets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_cluster_subnet_group)
         """
 
+    def modify_custom_domain_association(
+        self,
+        *,
+        ClusterIdentifier: str,
+        CustomDomainName: str = ...,
+        CustomDomainCertificateArn: str = ...
+    ) -> ModifyCustomDomainAssociationResultTypeDef:
+        """
+        Contains information for changing a custom domain association.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_custom_domain_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_custom_domain_association)
+        """
+
     def modify_endpoint_access(
         self, *, EndpointName: str, VpcSecurityGroupIds: Sequence[str] = ...
     ) -> EndpointAccessResponseMetadataTypeDef:
         """
         Modifies a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_endpoint_access)
@@ -2116,14 +2177,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_custom_domain_associations"]
+    ) -> DescribeCustomDomainAssociationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_data_shares"]
     ) -> DescribeDataSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.pyi` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClustersPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDataSharesPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventsPaginator,
@@ -88,18 +89,20 @@
     CopyClusterSnapshotResultTypeDef,
     CreateAuthenticationProfileResultTypeDef,
     CreateClusterParameterGroupResultTypeDef,
     CreateClusterResultTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     CreateClusterSnapshotResultTypeDef,
     CreateClusterSubnetGroupResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateHsmClientCertificateResultTypeDef,
     CreateHsmConfigurationResultTypeDef,
     CreateSnapshotCopyGrantResultTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     CustomerStorageMessageTypeDef,
     DataShareResponseMetadataTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterResultTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     DeleteClusterSnapshotResultTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
@@ -129,14 +132,15 @@
     ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionResultTypeDef,
     ModifyClusterIamRolesResultTypeDef,
     ModifyClusterMaintenanceResultTypeDef,
     ModifyClusterResultTypeDef,
     ModifyClusterSnapshotResultTypeDef,
     ModifyClusterSubnetGroupResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     ModifySnapshotCopyRetentionPeriodResultTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ParameterTypeDef,
     PartnerIntegrationOutputMessageTypeDef,
@@ -216,14 +220,16 @@
     ClusterSnapshotNotFoundFault: Type[BotocoreClientError]
     ClusterSnapshotQuotaExceededFault: Type[BotocoreClientError]
     ClusterSubnetGroupAlreadyExistsFault: Type[BotocoreClientError]
     ClusterSubnetGroupNotFoundFault: Type[BotocoreClientError]
     ClusterSubnetGroupQuotaExceededFault: Type[BotocoreClientError]
     ClusterSubnetQuotaExceededFault: Type[BotocoreClientError]
     CopyToRegionDisabledFault: Type[BotocoreClientError]
+    CustomCnameAssociationFault: Type[BotocoreClientError]
+    CustomDomainAssociationNotFoundFault: Type[BotocoreClientError]
     DependentServiceRequestThrottlingFault: Type[BotocoreClientError]
     DependentServiceUnavailableFault: Type[BotocoreClientError]
     EndpointAlreadyExistsFault: Type[BotocoreClientError]
     EndpointAuthorizationAlreadyExistsFault: Type[BotocoreClientError]
     EndpointAuthorizationNotFoundFault: Type[BotocoreClientError]
     EndpointAuthorizationsPerClusterLimitExceededFault: Type[BotocoreClientError]
     EndpointNotFoundFault: Type[BotocoreClientError]
@@ -574,14 +580,23 @@
     ) -> CreateClusterSubnetGroupResultTypeDef:
         """
         Creates a new Amazon Redshift subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_cluster_subnet_group)
         """
+    def create_custom_domain_association(
+        self, *, CustomDomainName: str, CustomDomainCertificateArn: str, ClusterIdentifier: str
+    ) -> CreateCustomDomainAssociationResultTypeDef:
+        """
+        Used to create a custom domain name for a cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_custom_domain_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_custom_domain_association)
+        """
     def create_endpoint_access(
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
@@ -779,14 +794,23 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified cluster subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_cluster_subnet_group)
         """
+    def delete_custom_domain_association(
+        self, *, ClusterIdentifier: str
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Contains information about deleting a custom domain association for a cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_custom_domain_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_custom_domain_association)
+        """
     def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseMetadataTypeDef:
         """
         Deletes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_endpoint_access)
         """
@@ -1013,14 +1037,28 @@
         Returns properties of provisioned clusters including general cluster properties,
         cluster database properties, maintenance and backup properties, and security and
         access properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#describe_clusters)
         """
+    def describe_custom_domain_associations(
+        self,
+        *,
+        CustomDomainName: str = ...,
+        CustomDomainCertificateArn: str = ...,
+        MaxRecords: int = ...,
+        Marker: str = ...
+    ) -> CustomDomainAssociationsMessageTypeDef:
+        """
+        Contains information for custom domain associations for a cluster.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_custom_domain_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#describe_custom_domain_associations)
+        """
     def describe_data_shares(
         self, *, DataShareArn: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeDataSharesResultTypeDef:
         """
         Shows the status of any inbound or outbound datashares available in the
         specified account.
 
@@ -1447,29 +1485,35 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#generate_presigned_url)
         """
     def get_cluster_credentials(
         self,
         *,
         DbUser: str,
-        ClusterIdentifier: str,
         DbName: str = ...,
+        ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
         AutoCreate: bool = ...,
-        DbGroups: Sequence[str] = ...
+        DbGroups: Sequence[str] = ...,
+        CustomDomainName: str = ...
     ) -> ClusterCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary authorization
         to log on to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_cluster_credentials)
         """
     def get_cluster_credentials_with_iam(
-        self, *, ClusterIdentifier: str, DbName: str = ..., DurationSeconds: int = ...
+        self,
+        *,
+        DbName: str = ...,
+        ClusterIdentifier: str = ...,
+        DurationSeconds: int = ...,
+        CustomDomainName: str = ...
     ) -> ClusterExtendedCredentialsTypeDef:
         """
         Returns a database user name and temporary password with temporary authorization
         to log in to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials_with_iam)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_cluster_credentials_with_iam)
@@ -1632,14 +1676,27 @@
     ) -> ModifyClusterSubnetGroupResultTypeDef:
         """
         Modifies a cluster subnet group to include the specified list of VPC subnets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_subnet_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_cluster_subnet_group)
         """
+    def modify_custom_domain_association(
+        self,
+        *,
+        ClusterIdentifier: str,
+        CustomDomainName: str = ...,
+        CustomDomainCertificateArn: str = ...
+    ) -> ModifyCustomDomainAssociationResultTypeDef:
+        """
+        Contains information for changing a custom domain association.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_custom_domain_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_custom_domain_association)
+        """
     def modify_endpoint_access(
         self, *, EndpointName: str, VpcSecurityGroupIds: Sequence[str] = ...
     ) -> EndpointAccessResponseMetadataTypeDef:
         """
         Modifies a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_endpoint_access)
@@ -1980,14 +2037,22 @@
     ) -> DescribeClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_custom_domain_associations"]
+    ) -> DescribeCustomDomainAssociationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_data_shares"]
     ) -> DescribeDataSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "DescribeClusterParametersPaginatorName",
     "DescribeClusterSecurityGroupsPaginatorName",
     "DescribeClusterSnapshotsPaginatorName",
     "DescribeClusterSubnetGroupsPaginatorName",
     "DescribeClusterTracksPaginatorName",
     "DescribeClusterVersionsPaginatorName",
     "DescribeClustersPaginatorName",
+    "DescribeCustomDomainAssociationsPaginatorName",
     "DescribeDataSharesForConsumerPaginatorName",
     "DescribeDataSharesForProducerPaginatorName",
     "DescribeDataSharesPaginatorName",
     "DescribeDefaultClusterParametersPaginatorName",
     "DescribeEndpointAccessPaginatorName",
     "DescribeEndpointAuthorizationPaginatorName",
     "DescribeEventSubscriptionsPaginatorName",
@@ -112,14 +113,15 @@
 DescribeClusterParametersPaginatorName = Literal["describe_cluster_parameters"]
 DescribeClusterSecurityGroupsPaginatorName = Literal["describe_cluster_security_groups"]
 DescribeClusterSnapshotsPaginatorName = Literal["describe_cluster_snapshots"]
 DescribeClusterSubnetGroupsPaginatorName = Literal["describe_cluster_subnet_groups"]
 DescribeClusterTracksPaginatorName = Literal["describe_cluster_tracks"]
 DescribeClusterVersionsPaginatorName = Literal["describe_cluster_versions"]
 DescribeClustersPaginatorName = Literal["describe_clusters"]
+DescribeCustomDomainAssociationsPaginatorName = Literal["describe_custom_domain_associations"]
 DescribeDataSharesForConsumerPaginatorName = Literal["describe_data_shares_for_consumer"]
 DescribeDataSharesForProducerPaginatorName = Literal["describe_data_shares_for_producer"]
 DescribeDataSharesPaginatorName = Literal["describe_data_shares"]
 DescribeDefaultClusterParametersPaginatorName = Literal["describe_default_cluster_parameters"]
 DescribeEndpointAccessPaginatorName = Literal["describe_endpoint_access"]
 DescribeEndpointAuthorizationPaginatorName = Literal["describe_endpoint_authorization"]
 DescribeEventSubscriptionsPaginatorName = Literal["describe_event_subscriptions"]
@@ -185,14 +187,15 @@
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
@@ -232,14 +235,15 @@
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
@@ -318,14 +322,15 @@
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
@@ -336,14 +341,15 @@
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
@@ -379,14 +385,15 @@
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
@@ -405,16 +412,19 @@
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
@@ -498,15 +508,17 @@
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
@@ -534,14 +546,15 @@
     "describe_cluster_parameters",
     "describe_cluster_security_groups",
     "describe_cluster_snapshots",
     "describe_cluster_subnet_groups",
     "describe_cluster_tracks",
     "describe_cluster_versions",
     "describe_clusters",
+    "describe_custom_domain_associations",
     "describe_data_shares",
     "describe_data_shares_for_consumer",
     "describe_data_shares_for_producer",
     "describe_default_cluster_parameters",
     "describe_endpoint_access",
     "describe_endpoint_authorization",
     "describe_event_subscriptions",
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.pyi` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "DescribeClusterParametersPaginatorName",
     "DescribeClusterSecurityGroupsPaginatorName",
     "DescribeClusterSnapshotsPaginatorName",
     "DescribeClusterSubnetGroupsPaginatorName",
     "DescribeClusterTracksPaginatorName",
     "DescribeClusterVersionsPaginatorName",
     "DescribeClustersPaginatorName",
+    "DescribeCustomDomainAssociationsPaginatorName",
     "DescribeDataSharesForConsumerPaginatorName",
     "DescribeDataSharesForProducerPaginatorName",
     "DescribeDataSharesPaginatorName",
     "DescribeDefaultClusterParametersPaginatorName",
     "DescribeEndpointAccessPaginatorName",
     "DescribeEndpointAuthorizationPaginatorName",
     "DescribeEventSubscriptionsPaginatorName",
@@ -110,14 +111,15 @@
 DescribeClusterParametersPaginatorName = Literal["describe_cluster_parameters"]
 DescribeClusterSecurityGroupsPaginatorName = Literal["describe_cluster_security_groups"]
 DescribeClusterSnapshotsPaginatorName = Literal["describe_cluster_snapshots"]
 DescribeClusterSubnetGroupsPaginatorName = Literal["describe_cluster_subnet_groups"]
 DescribeClusterTracksPaginatorName = Literal["describe_cluster_tracks"]
 DescribeClusterVersionsPaginatorName = Literal["describe_cluster_versions"]
 DescribeClustersPaginatorName = Literal["describe_clusters"]
+DescribeCustomDomainAssociationsPaginatorName = Literal["describe_custom_domain_associations"]
 DescribeDataSharesForConsumerPaginatorName = Literal["describe_data_shares_for_consumer"]
 DescribeDataSharesForProducerPaginatorName = Literal["describe_data_shares_for_producer"]
 DescribeDataSharesPaginatorName = Literal["describe_data_shares"]
 DescribeDefaultClusterParametersPaginatorName = Literal["describe_default_cluster_parameters"]
 DescribeEndpointAccessPaginatorName = Literal["describe_endpoint_access"]
 DescribeEndpointAuthorizationPaginatorName = Literal["describe_endpoint_authorization"]
 DescribeEventSubscriptionsPaginatorName = Literal["describe_event_subscriptions"]
@@ -183,14 +185,15 @@
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
@@ -230,14 +233,15 @@
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
@@ -316,14 +320,15 @@
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
@@ -334,14 +339,15 @@
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
@@ -377,14 +383,15 @@
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
@@ -403,16 +410,19 @@
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
@@ -496,15 +506,17 @@
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
@@ -532,14 +544,15 @@
     "describe_cluster_parameters",
     "describe_cluster_security_groups",
     "describe_cluster_snapshots",
     "describe_cluster_subnet_groups",
     "describe_cluster_tracks",
     "describe_cluster_versions",
     "describe_clusters",
+    "describe_custom_domain_associations",
     "describe_data_shares",
     "describe_data_shares_for_consumer",
     "describe_data_shares_for_producer",
     "describe_default_cluster_parameters",
     "describe_endpoint_access",
     "describe_endpoint_authorization",
     "describe_event_subscriptions",
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         DescribeClusterParametersPaginator,
         DescribeClusterSecurityGroupsPaginator,
         DescribeClusterSnapshotsPaginator,
         DescribeClusterSubnetGroupsPaginator,
         DescribeClusterTracksPaginator,
         DescribeClusterVersionsPaginator,
         DescribeClustersPaginator,
+        DescribeCustomDomainAssociationsPaginator,
         DescribeDataSharesPaginator,
         DescribeDataSharesForConsumerPaginator,
         DescribeDataSharesForProducerPaginator,
         DescribeDefaultClusterParametersPaginator,
         DescribeEndpointAccessPaginator,
         DescribeEndpointAuthorizationPaginator,
         DescribeEventSubscriptionsPaginator,
@@ -52,14 +53,15 @@
     describe_cluster_parameters_paginator: DescribeClusterParametersPaginator = client.get_paginator("describe_cluster_parameters")
     describe_cluster_security_groups_paginator: DescribeClusterSecurityGroupsPaginator = client.get_paginator("describe_cluster_security_groups")
     describe_cluster_snapshots_paginator: DescribeClusterSnapshotsPaginator = client.get_paginator("describe_cluster_snapshots")
     describe_cluster_subnet_groups_paginator: DescribeClusterSubnetGroupsPaginator = client.get_paginator("describe_cluster_subnet_groups")
     describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator("describe_cluster_tracks")
     describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator("describe_cluster_versions")
     describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+    describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = client.get_paginator("describe_custom_domain_associations")
     describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator("describe_data_shares")
     describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = client.get_paginator("describe_data_shares_for_consumer")
     describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = client.get_paginator("describe_data_shares_for_producer")
     describe_default_cluster_parameters_paginator: DescribeDefaultClusterParametersPaginator = client.get_paginator("describe_default_cluster_parameters")
     describe_endpoint_access_paginator: DescribeEndpointAccessPaginator = client.get_paginator("describe_endpoint_access")
     describe_endpoint_authorization_paginator: DescribeEndpointAuthorizationPaginator = client.get_paginator("describe_endpoint_authorization")
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
@@ -99,14 +101,15 @@
     ClusterDbRevisionsMessageTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     ClusterParameterGroupsMessageTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     ClustersMessageTypeDef,
     ClusterSubnetGroupMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     DescribeDefaultClusterParametersResultTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     DescribeSnapshotSchedulesOutputMessageTypeDef,
     EndpointAccessListTypeDef,
@@ -140,14 +143,15 @@
     "DescribeClusterParametersPaginator",
     "DescribeClusterSecurityGroupsPaginator",
     "DescribeClusterSnapshotsPaginator",
     "DescribeClusterSubnetGroupsPaginator",
     "DescribeClusterTracksPaginator",
     "DescribeClusterVersionsPaginator",
     "DescribeClustersPaginator",
+    "DescribeCustomDomainAssociationsPaginator",
     "DescribeDataSharesPaginator",
     "DescribeDataSharesForConsumerPaginator",
     "DescribeDataSharesForProducerPaginator",
     "DescribeDefaultClusterParametersPaginator",
     "DescribeEndpointAccessPaginator",
     "DescribeEndpointAuthorizationPaginator",
     "DescribeEventSubscriptionsPaginator",
@@ -183,15 +187,15 @@
 class DescribeClusterDbRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
     """
 
     def paginate(
-        self, *, ClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterIdentifier: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterDbRevisionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
         """
 
 
@@ -203,15 +207,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 
@@ -222,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 
@@ -242,15 +246,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 
@@ -270,15 +274,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 
@@ -290,30 +294,30 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 
 class DescribeClusterTracksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
     """
 
     def paginate(
-        self, *, MaintenanceTrackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, MaintenanceTrackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TrackListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
         """
 
 
@@ -324,15 +328,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterversionspaginator)
         """
 
 
@@ -344,30 +348,49 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterspaginator)
         """
 
 
+class DescribeCustomDomainAssociationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describecustomdomainassociationspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        CustomDomainName: str = ...,
+        CustomDomainCertificateArn: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[CustomDomainAssociationsMessageTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describecustomdomainassociationspaginator)
+        """
+
+
 class DescribeDataSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
     """
 
     def paginate(
-        self, *, DataShareArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DataShareArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSharesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
         """
 
 
@@ -378,15 +401,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 
@@ -397,30 +420,30 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 
 class DescribeDefaultClusterParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
         """
 
 
@@ -433,15 +456,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 
@@ -453,15 +476,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 
@@ -473,15 +496,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -495,15 +518,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventspaginator)
         """
 
 
@@ -515,15 +538,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 
@@ -535,15 +558,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 
@@ -558,15 +581,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 
@@ -577,15 +600,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 
@@ -596,45 +619,45 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 
 class DescribeReservedNodeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedNodeOfferingsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
         """
 
 
 class DescribeReservedNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReservedNodeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedNodesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
         """
 
 
@@ -649,15 +672,15 @@
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -669,15 +692,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 
@@ -690,15 +713,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 
@@ -709,15 +732,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 
@@ -730,15 +753,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetagspaginator)
         """
 
 
@@ -752,15 +775,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeusagelimitspaginator)
         """
 
 
@@ -772,28 +795,28 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 
 class GetReservedNodeExchangeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReservedNodeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
         """
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.pyi` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         DescribeClusterParametersPaginator,
         DescribeClusterSecurityGroupsPaginator,
         DescribeClusterSnapshotsPaginator,
         DescribeClusterSubnetGroupsPaginator,
         DescribeClusterTracksPaginator,
         DescribeClusterVersionsPaginator,
         DescribeClustersPaginator,
+        DescribeCustomDomainAssociationsPaginator,
         DescribeDataSharesPaginator,
         DescribeDataSharesForConsumerPaginator,
         DescribeDataSharesForProducerPaginator,
         DescribeDefaultClusterParametersPaginator,
         DescribeEndpointAccessPaginator,
         DescribeEndpointAuthorizationPaginator,
         DescribeEventSubscriptionsPaginator,
@@ -52,14 +53,15 @@
     describe_cluster_parameters_paginator: DescribeClusterParametersPaginator = client.get_paginator("describe_cluster_parameters")
     describe_cluster_security_groups_paginator: DescribeClusterSecurityGroupsPaginator = client.get_paginator("describe_cluster_security_groups")
     describe_cluster_snapshots_paginator: DescribeClusterSnapshotsPaginator = client.get_paginator("describe_cluster_snapshots")
     describe_cluster_subnet_groups_paginator: DescribeClusterSubnetGroupsPaginator = client.get_paginator("describe_cluster_subnet_groups")
     describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator("describe_cluster_tracks")
     describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator("describe_cluster_versions")
     describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+    describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = client.get_paginator("describe_custom_domain_associations")
     describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator("describe_data_shares")
     describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = client.get_paginator("describe_data_shares_for_consumer")
     describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = client.get_paginator("describe_data_shares_for_producer")
     describe_default_cluster_parameters_paginator: DescribeDefaultClusterParametersPaginator = client.get_paginator("describe_default_cluster_parameters")
     describe_endpoint_access_paginator: DescribeEndpointAccessPaginator = client.get_paginator("describe_endpoint_access")
     describe_endpoint_authorization_paginator: DescribeEndpointAuthorizationPaginator = client.get_paginator("describe_endpoint_authorization")
     describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
@@ -99,14 +101,15 @@
     ClusterDbRevisionsMessageTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     ClusterParameterGroupsMessageTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     ClustersMessageTypeDef,
     ClusterSubnetGroupMessageTypeDef,
     ClusterVersionsMessageTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     DescribeDefaultClusterParametersResultTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     DescribeSnapshotSchedulesOutputMessageTypeDef,
     EndpointAccessListTypeDef,
@@ -140,14 +143,15 @@
     "DescribeClusterParametersPaginator",
     "DescribeClusterSecurityGroupsPaginator",
     "DescribeClusterSnapshotsPaginator",
     "DescribeClusterSubnetGroupsPaginator",
     "DescribeClusterTracksPaginator",
     "DescribeClusterVersionsPaginator",
     "DescribeClustersPaginator",
+    "DescribeCustomDomainAssociationsPaginator",
     "DescribeDataSharesPaginator",
     "DescribeDataSharesForConsumerPaginator",
     "DescribeDataSharesForProducerPaginator",
     "DescribeDefaultClusterParametersPaginator",
     "DescribeEndpointAccessPaginator",
     "DescribeEndpointAuthorizationPaginator",
     "DescribeEventSubscriptionsPaginator",
@@ -180,15 +184,15 @@
 class DescribeClusterDbRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
     """
 
     def paginate(
-        self, *, ClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterIdentifier: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterDbRevisionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterdbrevisionspaginator)
         """
 
 class DescribeClusterParameterGroupsPaginator(Paginator):
@@ -199,15 +203,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 class DescribeClusterParametersPaginator(Paginator):
@@ -217,15 +221,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 class DescribeClusterSecurityGroupsPaginator(Paginator):
@@ -236,15 +240,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 class DescribeClusterSnapshotsPaginator(Paginator):
@@ -263,15 +267,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 class DescribeClusterSubnetGroupsPaginator(Paginator):
@@ -282,29 +286,29 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 class DescribeClusterTracksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
     """
 
     def paginate(
-        self, *, MaintenanceTrackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, MaintenanceTrackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TrackListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclustertrackspaginator)
         """
 
 class DescribeClusterVersionsPaginator(Paginator):
@@ -314,15 +318,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterversionspaginator)
         """
 
 class DescribeClustersPaginator(Paginator):
@@ -333,29 +337,47 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeclusterspaginator)
         """
 
+class DescribeCustomDomainAssociationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describecustomdomainassociationspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        CustomDomainName: str = ...,
+        CustomDomainCertificateArn: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[CustomDomainAssociationsMessageTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describecustomdomainassociationspaginator)
+        """
+
 class DescribeDataSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
     """
 
     def paginate(
-        self, *, DataShareArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DataShareArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSharesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharespaginator)
         """
 
 class DescribeDataSharesForConsumerPaginator(Paginator):
@@ -365,15 +387,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 class DescribeDataSharesForProducerPaginator(Paginator):
@@ -383,29 +405,29 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 class DescribeDefaultClusterParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describedefaultclusterparameterspaginator)
         """
 
 class DescribeEndpointAccessPaginator(Paginator):
@@ -417,15 +439,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 class DescribeEndpointAuthorizationPaginator(Paginator):
@@ -436,15 +458,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -455,15 +477,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -476,15 +498,15 @@
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeeventspaginator)
         """
 
 class DescribeHsmClientCertificatesPaginator(Paginator):
@@ -495,15 +517,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 class DescribeHsmConfigurationsPaginator(Paginator):
@@ -514,15 +536,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 class DescribeNodeConfigurationOptionsPaginator(Paginator):
@@ -536,15 +558,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 class DescribeOrderableClusterOptionsPaginator(Paginator):
@@ -554,15 +576,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 class DescribeReservedNodeExchangeStatusPaginator(Paginator):
@@ -572,43 +594,43 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 class DescribeReservedNodeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedNodeOfferingsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodeofferingspaginator)
         """
 
 class DescribeReservedNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReservedNodeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ReservedNodesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describereservednodespaginator)
         """
 
 class DescribeScheduledActionsPaginator(Paginator):
@@ -622,15 +644,15 @@
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeSnapshotCopyGrantsPaginator(Paginator):
@@ -641,15 +663,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 class DescribeSnapshotSchedulesPaginator(Paginator):
@@ -661,15 +683,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 class DescribeTableRestoreStatusPaginator(Paginator):
@@ -679,15 +701,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
@@ -699,15 +721,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describetagspaginator)
         """
 
 class DescribeUsageLimitsPaginator(Paginator):
@@ -720,15 +742,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#describeusagelimitspaginator)
         """
 
 class GetReservedNodeExchangeConfigurationOptionsPaginator(Paginator):
@@ -739,27 +761,27 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 class GetReservedNodeExchangeOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReservedNodeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/paginators/#getreservednodeexchangeofferingspaginator)
         """
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,34 +50,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
+    "CertificateAssociationTypeDef",
     "AuthenticationProfileTypeDef",
     "AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef",
     "AuthorizeDataShareMessageRequestTypeDef",
     "AuthorizeEndpointAccessMessageRequestTypeDef",
     "AuthorizeSnapshotAccessMessageRequestTypeDef",
     "SupportedPlatformTypeDef",
     "DeleteClusterSnapshotMessageTypeDef",
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
+    "ClusterCredentialsTypeDef",
     "RevisionTargetTypeDef",
+    "ClusterExtendedCredentialsTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
     "ParameterTypeDef",
+    "ClusterParameterGroupNameMessageTypeDef",
     "ClusterParameterStatusTypeDef",
     "TagTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
@@ -86,133 +89,168 @@
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
+    "CreateAuthenticationProfileResultTypeDef",
+    "CreateCustomDomainAssociationMessageRequestTypeDef",
+    "CreateCustomDomainAssociationResultTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
+    "CustomerStorageMessageTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
+    "DeleteAuthenticationProfileResultTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
+    "DeleteCustomDomainAssociationMessageRequestTypeDef",
     "DeleteEndpointAccessMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteHsmClientCertificateMessageRequestTypeDef",
     "DeleteHsmConfigurationMessageRequestTypeDef",
     "DeleteScheduledActionMessageRequestTypeDef",
     "DeleteSnapshotCopyGrantMessageRequestTypeDef",
     "DeleteSnapshotScheduleMessageRequestTypeDef",
     "DeleteTagsMessageRequestTypeDef",
     "DeleteUsageLimitMessageRequestTypeDef",
     "DescribeAccountAttributesMessageRequestTypeDef",
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
+    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterParametersMessageRequestTypeDef",
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     "SnapshotSortingEntityTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     "DescribeClusterTracksMessageRequestTypeDef",
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     "DescribeClusterVersionsMessageRequestTypeDef",
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     "DescribeClustersMessageRequestTypeDef",
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    "DescribeCustomDomainAssociationsMessageRequestTypeDef",
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
     "DescribeDataSharesForProducerMessageRequestTypeDef",
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
+    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesMessageRequestTypeDef",
     "DescribeResizeMessageRequestTypeDef",
     "ScheduledActionFilterTypeDef",
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     "DescribeTableRestoreStatusMessageRequestTypeDef",
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     "DescribeTagsMessageRequestTypeDef",
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     "DescribeUsageLimitsMessageRequestTypeDef",
     "DisableLoggingMessageRequestTypeDef",
     "DisableSnapshotCopyMessageRequestTypeDef",
     "DisassociateDataShareConsumerMessageRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableLoggingMessageRequestTypeDef",
     "EnableSnapshotCopyMessageRequestTypeDef",
     "EndpointAuthorizationTypeDef",
+    "EndpointAuthorizationResponseMetadataTypeDef",
     "EventInfoMapTypeDef",
     "EventTypeDef",
     "GetClusterCredentialsMessageRequestTypeDef",
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
+    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
+    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
+    "LoggingStatusTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
+    "ModifyAuthenticationProfileResultTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
     "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
+    "ModifyCustomDomainAssociationMessageRequestTypeDef",
+    "ModifyCustomDomainAssociationResultTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
+    "PaginatorConfigTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
+    "PartnerIntegrationOutputMessageTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
+    "ResizeProgressMessageTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
     "UpdatePartnerStatusInputMessageRequestTypeDef",
-    "ClusterCredentialsTypeDef",
-    "ClusterExtendedCredentialsTypeDef",
-    "ClusterParameterGroupNameMessageTypeDef",
-    "CreateAuthenticationProfileResultTypeDef",
-    "CustomerStorageMessageTypeDef",
-    "DeleteAuthenticationProfileResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    "LoggingStatusTypeDef",
-    "ModifyAuthenticationProfileResultTypeDef",
-    "PartnerIntegrationOutputMessageTypeDef",
-    "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
+    "AssociationTypeDef",
     "DescribeAuthenticationProfilesResultTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     "ClusterDbRevisionTypeDef",
     "ClusterParameterGroupDetailsTypeDef",
@@ -245,43 +283,14 @@
     "TaggedResourceTypeDef",
     "UsageLimitResponseMetadataTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
     "DataShareResponseMetadataTypeDef",
     "DataShareTypeDef",
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     "DescribeClustersMessageClusterAvailableWaitTypeDef",
     "DescribeClustersMessageClusterDeletedWaitTypeDef",
     "DescribeClustersMessageClusterRestoredWaitTypeDef",
     "DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
@@ -297,14 +306,15 @@
     "ReservedNodeOfferingTypeDef",
     "ReservedNodeTypeDef",
     "RestoreTableFromClusterSnapshotResultTypeDef",
     "TableRestoreStatusMessageTypeDef",
     "ScheduledActionTypeTypeDef",
     "UpdateTargetTypeDef",
     "AccountAttributeListTypeDef",
+    "CustomDomainAssociationsMessageTypeDef",
     "OrderableClusterOptionTypeDef",
     "SubnetTypeDef",
     "ClusterDbRevisionsMessageTypeDef",
     "DescribeDefaultClusterParametersResultTypeDef",
     "ClusterParameterGroupsMessageTypeDef",
     "CreateClusterParameterGroupResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
@@ -381,25 +391,14 @@
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
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
 AttributeValueTargetTypeDef = TypedDict(
     "AttributeValueTargetTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
@@ -442,14 +441,23 @@
 class AssociateDataShareConsumerMessageRequestTypeDef(
     _RequiredAssociateDataShareConsumerMessageRequestTypeDef,
     _OptionalAssociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
 
+CertificateAssociationTypeDef = TypedDict(
+    "CertificateAssociationTypeDef",
+    {
+        "CustomDomainName": str,
+        "ClusterIdentifier": str,
+    },
+    total=False,
+)
+
 AuthenticationProfileTypeDef = TypedDict(
     "AuthenticationProfileTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
     total=False,
@@ -609,24 +617,45 @@
     {
         "ClusterIdentifier": str,
         "ScheduleAssociationState": ScheduleStateType,
     },
     total=False,
 )
 
+ClusterCredentialsTypeDef = TypedDict(
+    "ClusterCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RevisionTargetTypeDef = TypedDict(
     "RevisionTargetTypeDef",
     {
         "DatabaseRevision": str,
         "Description": str,
         "DatabaseRevisionReleaseDate": datetime,
     },
     total=False,
 )
 
+ClusterExtendedCredentialsTypeDef = TypedDict(
+    "ClusterExtendedCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "NextRefreshTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClusterIamRoleTypeDef = TypedDict(
     "ClusterIamRoleTypeDef",
     {
         "IamRoleArn": str,
         "ApplyStatus": str,
     },
     total=False,
@@ -654,14 +683,23 @@
         "ApplyType": ParameterApplyTypeType,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
+ClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "ClusterParameterGroupNameMessageTypeDef",
+    {
+        "ParameterGroupName": str,
+        "ParameterGroupStatus": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClusterParameterStatusTypeDef = TypedDict(
     "ClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
@@ -842,14 +880,43 @@
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
+CreateAuthenticationProfileResultTypeDef = TypedDict(
+    "CreateAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "CreateCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+    },
+)
+
+CreateCustomDomainAssociationResultTypeDef = TypedDict(
+    "CreateCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
         "SubnetGroupName": str,
     },
 )
@@ -867,14 +934,23 @@
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
 
+CustomerStorageMessageTypeDef = TypedDict(
+    "CustomerStorageMessageTypeDef",
+    {
+        "TotalBackupSizeInMegaBytes": float,
+        "TotalProvisionedStorageInMegaBytes": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -894,14 +970,22 @@
 DeleteAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
 )
 
+DeleteAuthenticationProfileResultTypeDef = TypedDict(
+    "DeleteAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalDeleteClusterMessageRequestTypeDef = TypedDict(
@@ -960,14 +1044,21 @@
 DeleteClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
     },
 )
 
+DeleteCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "DeleteCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+
 DeleteEndpointAccessMessageRequestTypeDef = TypedDict(
     "DeleteEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -1040,46 +1131,79 @@
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeClusterDbRevisionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
+    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1096,14 +1220,25 @@
 class DescribeClusterParametersMessageRequestTypeDef(
     _RequiredDescribeClusterParametersMessageRequestTypeDef,
     _OptionalDescribeClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
+DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    {
+        "ClusterSecurityGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1138,91 +1273,204 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    {
+        "ClusterSubnetGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    {
+        "MaintenanceTrackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterTracksMessageRequestTypeDef = TypedDict(
     "DescribeClusterTracksMessageRequestTypeDef",
     {
         "MaintenanceTrackName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "ClusterParameterGroupFamily": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterVersionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterVersionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "ClusterParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClustersMessageRequestTypeDef = TypedDict(
     "DescribeClustersMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+DescribeCustomDomainAssociationsMessageRequestTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageRequestTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    {
+        "ConsumerArn": str,
+        "Status": DataShareStatusForConsumerType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSharesForConsumerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
     {
         "ConsumerArn": str,
         "Status": DataShareStatusForConsumerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    {
+        "ProducerArn": str,
+        "Status": DataShareStatusForProducerType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSharesForProducerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     {
         "ProducerArn": str,
         "Status": DataShareStatusForProducerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    {
+        "DataShareArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSharesMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
+    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDefaultClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupFamily": str,
     },
 )
 _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1238,27 +1486,50 @@
 class DescribeDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
+DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ResourceOwner": str,
+        "EndpointName": str,
+        "VpcId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointAccessMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "EndpointName": str,
         "VpcId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "Account": str,
+        "Grantee": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointAuthorizationMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "Grantee": bool,
         "MaxRecords": int,
@@ -1271,52 +1542,98 @@
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeHsmConfigurationsMessageRequestTypeDef = TypedDict(
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1338,14 +1655,24 @@
         "Name": NodeConfigurationOptionsFilterNameType,
         "Operator": OperatorTypeType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "NodeType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeOrderableClusterOptionsMessageRequestTypeDef = TypedDict(
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "NodeType": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1386,35 +1713,63 @@
         "StatusMessage": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "ReservedNodeExchangeRequestId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "ReservedNodeExchangeRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeOfferingId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodeOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
     {
         "ReservedNodeOfferingId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodesMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1432,63 +1787,121 @@
     "ScheduledActionFilterTypeDef",
     {
         "Name": ScheduledActionFilterNameType,
         "Values": Sequence[str],
     },
 )
 
+DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotCopyGrantsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ScheduleIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotSchedulesMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ScheduleIdentifier": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TableRestoreRequestId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeTableRestoreStatusMessageRequestTypeDef = TypedDict(
     "DescribeTableRestoreStatusMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "TableRestoreRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+        "ResourceType": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeTagsMessageRequestTypeDef = TypedDict(
     "DescribeTagsMessageRequestTypeDef",
     {
         "ResourceName": str,
         "ResourceType": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUsageLimitsMessageRequestTypeDef = TypedDict(
     "DescribeUsageLimitsMessageRequestTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "MaxRecords": int,
@@ -1533,14 +1946,21 @@
 class DisassociateDataShareConsumerMessageRequestTypeDef(
     _RequiredDisassociateDataShareConsumerMessageRequestTypeDef,
     _OptionalDisassociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableLoggingMessageRequestTypeDef = TypedDict(
     "_RequiredEnableLoggingMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalEnableLoggingMessageRequestTypeDef = TypedDict(
@@ -1598,14 +2018,30 @@
         "AllowedAllVPCs": bool,
         "AllowedVPCs": List[str],
         "EndpointCount": int,
     },
     total=False,
 )
 
+EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
+    "EndpointAuthorizationResponseMetadataTypeDef",
+    {
+        "Grantor": str,
+        "Grantee": str,
+        "ClusterIdentifier": str,
+        "AuthorizeTime": datetime,
+        "ClusterStatus": str,
+        "Status": AuthorizationStatusType,
+        "AllowedAllVPCs": bool,
+        "AllowedVPCs": List[str],
+        "EndpointCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventInfoMapTypeDef = TypedDict(
     "EventInfoMapTypeDef",
     {
         "EventId": str,
         "EventCategories": List[str],
         "EventDescription": str,
         "Severity": str,
@@ -1627,55 +2063,68 @@
     total=False,
 )
 
 _RequiredGetClusterCredentialsMessageRequestTypeDef = TypedDict(
     "_RequiredGetClusterCredentialsMessageRequestTypeDef",
     {
         "DbUser": str,
-        "ClusterIdentifier": str,
     },
 )
 _OptionalGetClusterCredentialsMessageRequestTypeDef = TypedDict(
     "_OptionalGetClusterCredentialsMessageRequestTypeDef",
     {
         "DbName": str,
+        "ClusterIdentifier": str,
         "DurationSeconds": int,
         "AutoCreate": bool,
         "DbGroups": Sequence[str],
+        "CustomDomainName": str,
     },
     total=False,
 )
 
 
 class GetClusterCredentialsMessageRequestTypeDef(
     _RequiredGetClusterCredentialsMessageRequestTypeDef,
     _OptionalGetClusterCredentialsMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
-    "_RequiredGetClusterCredentialsWithIAMMessageRequestTypeDef",
+GetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
+    "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     {
+        "DbName": str,
         "ClusterIdentifier": str,
+        "DurationSeconds": int,
+        "CustomDomainName": str,
+    },
+    total=False,
+)
+
+_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ActionType": ReservedNodeExchangeActionTypeType,
     },
 )
-_OptionalGetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
-    "_OptionalGetClusterCredentialsWithIAMMessageRequestTypeDef",
+_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     {
-        "DbName": str,
-        "DurationSeconds": int,
+        "ClusterIdentifier": str,
+        "SnapshotIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class GetClusterCredentialsWithIAMMessageRequestTypeDef(
-    _RequiredGetClusterCredentialsWithIAMMessageRequestTypeDef,
-    _OptionalGetClusterCredentialsWithIAMMessageRequestTypeDef,
+class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
 ):
     pass
 
 
 _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     {
@@ -1697,14 +2146,36 @@
 class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+    },
+)
+_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
     },
 )
 _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
@@ -1720,14 +2191,29 @@
 class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
 ):
     pass
 
 
+LoggingStatusTypeDef = TypedDict(
+    "LoggingStatusTypeDef",
+    {
+        "LoggingEnabled": bool,
+        "BucketName": str,
+        "S3KeyPrefix": str,
+        "LastSuccessfulDeliveryTime": datetime,
+        "LastFailureTime": datetime,
+        "LastFailureMessage": str,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogExports": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_RequiredModifyAquaInputMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyAquaInputMessageRequestTypeDef = TypedDict(
@@ -1749,14 +2235,23 @@
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
+ModifyAuthenticationProfileResultTypeDef = TypedDict(
+    "ModifyAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ModifyClusterDbRevisionMessageRequestTypeDef = TypedDict(
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RevisionTarget": str,
     },
 )
@@ -1920,14 +2415,48 @@
 class ModifyClusterSubnetGroupMessageRequestTypeDef(
     _RequiredModifyClusterSubnetGroupMessageRequestTypeDef,
     _OptionalModifyClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
 
+_RequiredModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+    },
+    total=False,
+)
+
+
+class ModifyCustomDomainAssociationMessageRequestTypeDef(
+    _RequiredModifyCustomDomainAssociationMessageRequestTypeDef,
+    _OptionalModifyCustomDomainAssociationMessageRequestTypeDef,
+):
+    pass
+
+
+ModifyCustomDomainAssociationResultTypeDef = TypedDict(
+    "ModifyCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 _OptionalModifyEndpointAccessMessageRequestTypeDef = TypedDict(
@@ -2044,24 +2573,43 @@
         "NumberOfNodes": int,
         "EstimatedDiskUtilizationPercent": float,
         "Mode": ModeType,
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
 PartnerIntegrationInputMessageRequestTypeDef = TypedDict(
     "PartnerIntegrationInputMessageRequestTypeDef",
     {
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
+PartnerIntegrationOutputMessageTypeDef = TypedDict(
+    "PartnerIntegrationOutputMessageTypeDef",
+    {
+        "DatabaseName": str,
+        "PartnerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2165,14 +2713,48 @@
 
 class ResizeClusterMessageTypeDef(
     _RequiredResizeClusterMessageTypeDef, _OptionalResizeClusterMessageTypeDef
 ):
     pass
 
 
+ResizeProgressMessageTypeDef = TypedDict(
+    "ResizeProgressMessageTypeDef",
+    {
+        "TargetNodeType": str,
+        "TargetNumberOfNodes": int,
+        "TargetClusterType": str,
+        "Status": str,
+        "ImportTablesCompleted": List[str],
+        "ImportTablesInProgress": List[str],
+        "ImportTablesNotStarted": List[str],
+        "AvgResizeRateInMegaBytesPerSecond": float,
+        "TotalResizeDataInMegaBytes": int,
+        "ProgressInMegaBytes": int,
+        "ElapsedTimeInSeconds": int,
+        "EstimatedTimeToCompletionInSeconds": int,
+        "ResizeType": str,
+        "Message": str,
+        "TargetEncryptionType": str,
+        "DataTransferProgressPercent": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
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
 _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2382,171 +2964,46 @@
 class UpdatePartnerStatusInputMessageRequestTypeDef(
     _RequiredUpdatePartnerStatusInputMessageRequestTypeDef,
     _OptionalUpdatePartnerStatusInputMessageRequestTypeDef,
 ):
     pass
 
 
-ClusterCredentialsTypeDef = TypedDict(
-    "ClusterCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClusterExtendedCredentialsTypeDef = TypedDict(
-    "ClusterExtendedCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "NextRefreshTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "ClusterParameterGroupNameMessageTypeDef",
-    {
-        "ParameterGroupName": str,
-        "ParameterGroupStatus": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAuthenticationProfileResultTypeDef = TypedDict(
-    "CreateAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CustomerStorageMessageTypeDef = TypedDict(
-    "CustomerStorageMessageTypeDef",
-    {
-        "TotalBackupSizeInMegaBytes": float,
-        "TotalProvisionedStorageInMegaBytes": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteAuthenticationProfileResultTypeDef = TypedDict(
-    "DeleteAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    {
-        "Grantor": str,
-        "Grantee": str,
-        "ClusterIdentifier": str,
-        "AuthorizeTime": datetime,
-        "ClusterStatus": str,
-        "Status": AuthorizationStatusType,
-        "AllowedAllVPCs": bool,
-        "AllowedVPCs": List[str],
-        "EndpointCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LoggingStatusTypeDef = TypedDict(
-    "LoggingStatusTypeDef",
-    {
-        "LoggingEnabled": bool,
-        "BucketName": str,
-        "S3KeyPrefix": str,
-        "LastSuccessfulDeliveryTime": datetime,
-        "LastFailureTime": datetime,
-        "LastFailureMessage": str,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogExports": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyAuthenticationProfileResultTypeDef = TypedDict(
-    "ModifyAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PartnerIntegrationOutputMessageTypeDef = TypedDict(
-    "PartnerIntegrationOutputMessageTypeDef",
-    {
-        "DatabaseName": str,
-        "PartnerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResizeProgressMessageTypeDef = TypedDict(
-    "ResizeProgressMessageTypeDef",
-    {
-        "TargetNodeType": str,
-        "TargetNumberOfNodes": int,
-        "TargetClusterType": str,
-        "Status": str,
-        "ImportTablesCompleted": List[str],
-        "ImportTablesInProgress": List[str],
-        "ImportTablesNotStarted": List[str],
-        "AvgResizeRateInMegaBytesPerSecond": float,
-        "TotalResizeDataInMegaBytes": int,
-        "ProgressInMegaBytes": int,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ResizeType": str,
-        "Message": str,
-        "TargetEncryptionType": str,
-        "DataTransferProgressPercent": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AttributeValueTargetTypeDef],
     },
     total=False,
 )
 
 ModifyAquaOutputMessageTypeDef = TypedDict(
     "ModifyAquaOutputMessageTypeDef",
     {
         "AquaConfiguration": AquaConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AssociationTypeDef = TypedDict(
+    "AssociationTypeDef",
+    {
+        "CustomDomainCertificateArn": str,
+        "CustomDomainCertificateExpiryDate": datetime,
+        "CertificateAssociations": List[CertificateAssociationTypeDef],
+    },
+    total=False,
+)
+
 DescribeAuthenticationProfilesResultTypeDef = TypedDict(
     "DescribeAuthenticationProfilesResultTypeDef",
     {
         "AuthenticationProfiles": List[AuthenticationProfileTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
@@ -2563,24 +3020,24 @@
 )
 
 BatchDeleteClusterSnapshotsResultTypeDef = TypedDict(
     "BatchDeleteClusterSnapshotsResultTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchModifyClusterSnapshotsOutputMessageTypeDef = TypedDict(
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterDbRevisionTypeDef = TypedDict(
     "ClusterDbRevisionTypeDef",
     {
         "ClusterIdentifier": str,
@@ -2592,15 +3049,15 @@
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
@@ -3034,15 +3491,15 @@
         "ScheduleDefinitions": List[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": List[TagTypeDef],
         "NextInvocations": List[datetime],
         "AssociatedClusterCount": int,
         "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotScheduleTypeDef = TypedDict(
     "SnapshotScheduleTypeDef",
     {
         "ScheduleDefinitions": List[str],
@@ -3114,15 +3571,15 @@
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "LimitType": UsageLimitLimitTypeType,
         "Amount": int,
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsageLimitTypeDef = TypedDict(
     "UsageLimitTypeDef",
     {
         "UsageLimitId": str,
@@ -3138,36 +3595,36 @@
 )
 
 DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     {
         "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterVersionsMessageTypeDef = TypedDict(
     "ClusterVersionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataShareResponseMetadataTypeDef = TypedDict(
     "DataShareResponseMetadataTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataShareTypeDef = TypedDict(
     "DataShareTypeDef",
     {
         "DataShareArn": str,
@@ -3175,386 +3632,29 @@
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
     },
     total=False,
 )
 
-DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
-    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-):
-    pass
-
-
-DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    {
-        "ClusterSubnetGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    {
-        "MaintenanceTrackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "ClusterParameterGroupFamily": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    {
-        "ConsumerArn": str,
-        "Status": DataShareStatusForConsumerType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    {
-        "ProducerArn": str,
-        "Status": DataShareStatusForProducerType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    {
-        "DataShareArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
-    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-):
-    pass
-
-
-DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ResourceOwner": str,
-        "EndpointName": str,
-        "VpcId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "Account": str,
-        "Grantee": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "NodeType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "ReservedNodeExchangeRequestId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeOfferingId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ScheduleIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TableRestoreRequestId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "ResourceType": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ActionType": ReservedNodeExchangeActionTypeType,
-    },
-)
-_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "SnapshotIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-    },
-)
-_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-):
-    pass
-
-
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
@@ -3645,15 +3745,15 @@
     "_OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "OwnerAccount": str,
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -3690,28 +3790,28 @@
     pass
 
 
 DescribePartnersOutputMessageTypeDef = TypedDict(
     "DescribePartnersOutputMessageTypeDef",
     {
         "PartnerIntegrationInfoList": List[PartnerIntegrationInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
@@ -3728,15 +3828,15 @@
 )
 
 EndpointAuthorizationListTypeDef = TypedDict(
     "EndpointAuthorizationListTypeDef",
     {
         "EndpointAuthorizationList": List[EndpointAuthorizationTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
@@ -3746,15 +3846,15 @@
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
@@ -3765,15 +3865,15 @@
 )
 
 NodeConfigurationOptionsMessageTypeDef = TypedDict(
     "NodeConfigurationOptionsMessageTypeDef",
     {
         "NodeConfigurationOptionList": List[NodeConfigurationOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedNodeOfferingTypeDef = TypedDict(
     "ReservedNodeOfferingTypeDef",
     {
         "ReservedNodeOfferingId": str,
@@ -3809,24 +3909,24 @@
     total=False,
 )
 
 RestoreTableFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreTableFromClusterSnapshotResultTypeDef",
     {
         "TableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableRestoreStatusMessageTypeDef = TypedDict(
     "TableRestoreStatusMessageTypeDef",
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
@@ -3846,15 +3946,24 @@
     total=False,
 )
 
 AccountAttributeListTypeDef = TypedDict(
     "AccountAttributeListTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CustomDomainAssociationsMessageTypeDef = TypedDict(
+    "CustomDomainAssociationsMessageTypeDef",
+    {
+        "Marker": str,
+        "Associations": List[AssociationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OrderableClusterOptionTypeDef = TypedDict(
     "OrderableClusterOptionTypeDef",
     {
         "ClusterVersion": str,
@@ -3876,99 +3985,99 @@
 )
 
 ClusterDbRevisionsMessageTypeDef = TypedDict(
     "ClusterDbRevisionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterDbRevisions": List[ClusterDbRevisionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeDefaultClusterParametersResultTypeDef",
     {
         "DefaultClusterParameters": DefaultClusterParametersTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterParameterGroupsMessageTypeDef = TypedDict(
     "ClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "ParameterGroups": List[ClusterParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterParameterGroupResultTypeDef = TypedDict(
     "CreateClusterParameterGroupResultTypeDef",
     {
         "ClusterParameterGroup": ClusterParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHsmClientCertificateResultTypeDef = TypedDict(
     "CreateHsmClientCertificateResultTypeDef",
     {
         "HsmClientCertificate": HsmClientCertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HsmClientCertificateMessageTypeDef = TypedDict(
     "HsmClientCertificateMessageTypeDef",
     {
         "Marker": str,
         "HsmClientCertificates": List[HsmClientCertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHsmConfigurationResultTypeDef = TypedDict(
     "CreateHsmConfigurationResultTypeDef",
     {
         "HsmConfiguration": HsmConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HsmConfigurationMessageTypeDef = TypedDict(
     "HsmConfigurationMessageTypeDef",
     {
         "Marker": str,
         "HsmConfigurations": List[HsmConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
@@ -3980,143 +4089,143 @@
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
         "SnapshotCopyGrant": SnapshotCopyGrantTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotCopyGrantMessageTypeDef = TypedDict(
     "SnapshotCopyGrantMessageTypeDef",
     {
         "Marker": str,
         "SnapshotCopyGrants": List[SnapshotCopyGrantTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotSchedulesOutputMessageTypeDef = TypedDict(
     "DescribeSnapshotSchedulesOutputMessageTypeDef",
     {
         "SnapshotSchedules": List[SnapshotScheduleTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeSnapshotAccessResultTypeDef = TypedDict(
     "AuthorizeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopyClusterSnapshotResultTypeDef = TypedDict(
     "CopyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterSnapshotResultTypeDef = TypedDict(
     "CreateClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterSnapshotResultTypeDef = TypedDict(
     "DeleteClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterSnapshotResultTypeDef = TypedDict(
     "ModifyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RevokeSnapshotAccessResultTypeDef = TypedDict(
     "RevokeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotMessageTypeDef = TypedDict(
     "SnapshotMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaggedResourceListMessageTypeDef = TypedDict(
     "TaggedResourceListMessageTypeDef",
     {
         "TaggedResources": List[TaggedResourceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsageLimitListTypeDef = TypedDict(
     "UsageLimitListTypeDef",
     {
         "UsageLimits": List[UsageLimitTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSharesForConsumerResultTypeDef = TypedDict(
     "DescribeDataSharesForConsumerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSharesForProducerResultTypeDef = TypedDict(
     "DescribeDataSharesForProducerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSharesResultTypeDef = TypedDict(
     "DescribeDataSharesResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointAccessResponseMetadataTypeDef = TypedDict(
     "EndpointAccessResponseMetadataTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4125,15 +4234,15 @@
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
         "Port": int,
         "Address": str,
         "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4161,40 +4270,40 @@
 )
 
 GetReservedNodeExchangeOfferingsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedNodeOfferingsMessageTypeDef = TypedDict(
     "ReservedNodeOfferingsMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptReservedNodeExchangeOutputMessageTypeDef = TypedDict(
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     {
         "ExchangedReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseReservedNodeOfferingResultTypeDef = TypedDict(
     "PurchaseReservedNodeOfferingResultTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedNodeConfigurationOptionTypeDef = TypedDict(
     "ReservedNodeConfigurationOptionTypeDef",
     {
         "SourceReservedNode": ReservedNodeTypeDef,
@@ -4205,15 +4314,15 @@
 )
 
 ReservedNodesMessageTypeDef = TypedDict(
     "ReservedNodesMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
@@ -4277,15 +4386,15 @@
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
         "State": ScheduledActionStateType,
         "NextInvocations": List[datetime],
         "StartTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionTypeDef = TypedDict(
     "ScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
@@ -4312,15 +4421,15 @@
 )
 
 OrderableClusterOptionsMessageTypeDef = TypedDict(
     "OrderableClusterOptionsMessageTypeDef",
     {
         "OrderableClusterOptions": List[OrderableClusterOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSubnetGroupTypeDef = TypedDict(
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
@@ -4333,49 +4442,49 @@
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSecurityGroupMessageTypeDef = TypedDict(
     "ClusterSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSecurityGroups": List[ClusterSecurityGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterSecurityGroupResultTypeDef = TypedDict(
     "CreateClusterSecurityGroupResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RevokeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointAccessListTypeDef = TypedDict(
     "EndpointAccessListTypeDef",
     {
         "EndpointAccessList": List[EndpointAccessTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4426,191 +4535,194 @@
         "ResizeInfo": ResizeInfoTypeDef,
         "AvailabilityZoneRelocationStatus": str,
         "ClusterNamespaceArn": str,
         "TotalStorageCapacityInMegaBytes": int,
         "AquaConfiguration": AquaConfigurationTypeDef,
         "DefaultIamRoleArn": str,
         "ReservedNodeExchangeStatus": ReservedNodeExchangeStatusTypeDef,
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "CustomDomainCertificateExpiryDate": datetime,
     },
     total=False,
 )
 
 GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeConfigurationOptionList": List[ReservedNodeConfigurationOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionsMessageTypeDef = TypedDict(
     "ScheduledActionsMessageTypeDef",
     {
         "Marker": str,
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrackListMessageTypeDef = TypedDict(
     "TrackListMessageTypeDef",
     {
         "MaintenanceTracks": List[MaintenanceTrackTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSubnetGroupMessageTypeDef = TypedDict(
     "ClusterSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSubnetGroups": List[ClusterSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterSubnetGroupResultTypeDef = TypedDict(
     "CreateClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterSubnetGroupResultTypeDef = TypedDict(
     "ModifyClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClustersMessageTypeDef = TypedDict(
     "ClustersMessageTypeDef",
     {
         "Marker": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResultTypeDef = TypedDict(
     "DeleteClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisableSnapshotCopyResultTypeDef = TypedDict(
     "DisableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableSnapshotCopyResultTypeDef = TypedDict(
     "EnableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterDbRevisionResultTypeDef = TypedDict(
     "ModifyClusterDbRevisionResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterIamRolesResultTypeDef = TypedDict(
     "ModifyClusterIamRolesResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterMaintenanceResultTypeDef = TypedDict(
     "ModifyClusterMaintenanceResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterResultTypeDef = TypedDict(
     "ModifyClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifySnapshotCopyRetentionPeriodResultTypeDef = TypedDict(
     "ModifySnapshotCopyRetentionPeriodResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PauseClusterResultTypeDef = TypedDict(
     "PauseClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootClusterResultTypeDef = TypedDict(
     "RebootClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResizeClusterResultTypeDef = TypedDict(
     "ResizeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreFromClusterSnapshotResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResumeClusterResultTypeDef = TypedDict(
     "ResumeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateEncryptionKeyResultTypeDef = TypedDict(
     "RotateEncryptionKeyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.pyi` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -49,34 +49,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
+    "CertificateAssociationTypeDef",
     "AuthenticationProfileTypeDef",
     "AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef",
     "AuthorizeDataShareMessageRequestTypeDef",
     "AuthorizeEndpointAccessMessageRequestTypeDef",
     "AuthorizeSnapshotAccessMessageRequestTypeDef",
     "SupportedPlatformTypeDef",
     "DeleteClusterSnapshotMessageTypeDef",
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
+    "ClusterCredentialsTypeDef",
     "RevisionTargetTypeDef",
+    "ClusterExtendedCredentialsTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
     "ParameterTypeDef",
+    "ClusterParameterGroupNameMessageTypeDef",
     "ClusterParameterStatusTypeDef",
     "TagTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
@@ -85,133 +88,168 @@
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
+    "CreateAuthenticationProfileResultTypeDef",
+    "CreateCustomDomainAssociationMessageRequestTypeDef",
+    "CreateCustomDomainAssociationResultTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
+    "CustomerStorageMessageTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
+    "DeleteAuthenticationProfileResultTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
+    "DeleteCustomDomainAssociationMessageRequestTypeDef",
     "DeleteEndpointAccessMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteHsmClientCertificateMessageRequestTypeDef",
     "DeleteHsmConfigurationMessageRequestTypeDef",
     "DeleteScheduledActionMessageRequestTypeDef",
     "DeleteSnapshotCopyGrantMessageRequestTypeDef",
     "DeleteSnapshotScheduleMessageRequestTypeDef",
     "DeleteTagsMessageRequestTypeDef",
     "DeleteUsageLimitMessageRequestTypeDef",
     "DescribeAccountAttributesMessageRequestTypeDef",
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
+    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterParametersMessageRequestTypeDef",
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     "SnapshotSortingEntityTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     "DescribeClusterTracksMessageRequestTypeDef",
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     "DescribeClusterVersionsMessageRequestTypeDef",
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     "DescribeClustersMessageRequestTypeDef",
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    "DescribeCustomDomainAssociationsMessageRequestTypeDef",
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
     "DescribeDataSharesForProducerMessageRequestTypeDef",
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
+    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesMessageRequestTypeDef",
     "DescribeResizeMessageRequestTypeDef",
     "ScheduledActionFilterTypeDef",
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     "DescribeTableRestoreStatusMessageRequestTypeDef",
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     "DescribeTagsMessageRequestTypeDef",
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     "DescribeUsageLimitsMessageRequestTypeDef",
     "DisableLoggingMessageRequestTypeDef",
     "DisableSnapshotCopyMessageRequestTypeDef",
     "DisassociateDataShareConsumerMessageRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableLoggingMessageRequestTypeDef",
     "EnableSnapshotCopyMessageRequestTypeDef",
     "EndpointAuthorizationTypeDef",
+    "EndpointAuthorizationResponseMetadataTypeDef",
     "EventInfoMapTypeDef",
     "EventTypeDef",
     "GetClusterCredentialsMessageRequestTypeDef",
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
+    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
+    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
+    "LoggingStatusTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
+    "ModifyAuthenticationProfileResultTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
     "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
+    "ModifyCustomDomainAssociationMessageRequestTypeDef",
+    "ModifyCustomDomainAssociationResultTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
+    "PaginatorConfigTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
+    "PartnerIntegrationOutputMessageTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
+    "ResizeProgressMessageTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
     "UpdatePartnerStatusInputMessageRequestTypeDef",
-    "ClusterCredentialsTypeDef",
-    "ClusterExtendedCredentialsTypeDef",
-    "ClusterParameterGroupNameMessageTypeDef",
-    "CreateAuthenticationProfileResultTypeDef",
-    "CustomerStorageMessageTypeDef",
-    "DeleteAuthenticationProfileResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    "LoggingStatusTypeDef",
-    "ModifyAuthenticationProfileResultTypeDef",
-    "PartnerIntegrationOutputMessageTypeDef",
-    "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
+    "AssociationTypeDef",
     "DescribeAuthenticationProfilesResultTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     "ClusterDbRevisionTypeDef",
     "ClusterParameterGroupDetailsTypeDef",
@@ -244,43 +282,14 @@
     "TaggedResourceTypeDef",
     "UsageLimitResponseMetadataTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
     "DataShareResponseMetadataTypeDef",
     "DataShareTypeDef",
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     "DescribeClustersMessageClusterAvailableWaitTypeDef",
     "DescribeClustersMessageClusterDeletedWaitTypeDef",
     "DescribeClustersMessageClusterRestoredWaitTypeDef",
     "DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
@@ -296,14 +305,15 @@
     "ReservedNodeOfferingTypeDef",
     "ReservedNodeTypeDef",
     "RestoreTableFromClusterSnapshotResultTypeDef",
     "TableRestoreStatusMessageTypeDef",
     "ScheduledActionTypeTypeDef",
     "UpdateTargetTypeDef",
     "AccountAttributeListTypeDef",
+    "CustomDomainAssociationsMessageTypeDef",
     "OrderableClusterOptionTypeDef",
     "SubnetTypeDef",
     "ClusterDbRevisionsMessageTypeDef",
     "DescribeDefaultClusterParametersResultTypeDef",
     "ClusterParameterGroupsMessageTypeDef",
     "CreateClusterParameterGroupResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
@@ -380,25 +390,14 @@
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
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
 AttributeValueTargetTypeDef = TypedDict(
     "AttributeValueTargetTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
@@ -439,14 +438,23 @@
 
 class AssociateDataShareConsumerMessageRequestTypeDef(
     _RequiredAssociateDataShareConsumerMessageRequestTypeDef,
     _OptionalAssociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
+CertificateAssociationTypeDef = TypedDict(
+    "CertificateAssociationTypeDef",
+    {
+        "CustomDomainName": str,
+        "ClusterIdentifier": str,
+    },
+    total=False,
+)
+
 AuthenticationProfileTypeDef = TypedDict(
     "AuthenticationProfileTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
     total=False,
@@ -596,24 +604,45 @@
     {
         "ClusterIdentifier": str,
         "ScheduleAssociationState": ScheduleStateType,
     },
     total=False,
 )
 
+ClusterCredentialsTypeDef = TypedDict(
+    "ClusterCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RevisionTargetTypeDef = TypedDict(
     "RevisionTargetTypeDef",
     {
         "DatabaseRevision": str,
         "Description": str,
         "DatabaseRevisionReleaseDate": datetime,
     },
     total=False,
 )
 
+ClusterExtendedCredentialsTypeDef = TypedDict(
+    "ClusterExtendedCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "NextRefreshTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClusterIamRoleTypeDef = TypedDict(
     "ClusterIamRoleTypeDef",
     {
         "IamRoleArn": str,
         "ApplyStatus": str,
     },
     total=False,
@@ -641,14 +670,23 @@
         "ApplyType": ParameterApplyTypeType,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
+ClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "ClusterParameterGroupNameMessageTypeDef",
+    {
+        "ParameterGroupName": str,
+        "ParameterGroupStatus": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClusterParameterStatusTypeDef = TypedDict(
     "ClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
@@ -827,14 +865,43 @@
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
+CreateAuthenticationProfileResultTypeDef = TypedDict(
+    "CreateAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "CreateCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+    },
+)
+
+CreateCustomDomainAssociationResultTypeDef = TypedDict(
+    "CreateCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
         "SubnetGroupName": str,
     },
 )
@@ -850,14 +917,23 @@
 
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
+CustomerStorageMessageTypeDef = TypedDict(
+    "CustomerStorageMessageTypeDef",
+    {
+        "TotalBackupSizeInMegaBytes": float,
+        "TotalProvisionedStorageInMegaBytes": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -877,14 +953,22 @@
 DeleteAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
 )
 
+DeleteAuthenticationProfileResultTypeDef = TypedDict(
+    "DeleteAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalDeleteClusterMessageRequestTypeDef = TypedDict(
@@ -939,14 +1023,21 @@
 DeleteClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
     },
 )
 
+DeleteCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "DeleteCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+
 DeleteEndpointAccessMessageRequestTypeDef = TypedDict(
     "DeleteEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -1019,46 +1110,77 @@
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeClusterDbRevisionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
+    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1073,14 +1195,25 @@
 
 class DescribeClusterParametersMessageRequestTypeDef(
     _RequiredDescribeClusterParametersMessageRequestTypeDef,
     _OptionalDescribeClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    {
+        "ClusterSecurityGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1113,91 +1246,202 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    {
+        "ClusterSubnetGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    {
+        "MaintenanceTrackName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterTracksMessageRequestTypeDef = TypedDict(
     "DescribeClusterTracksMessageRequestTypeDef",
     {
         "MaintenanceTrackName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "ClusterParameterGroupFamily": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClusterVersionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterVersionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "ClusterParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeClustersMessageRequestTypeDef = TypedDict(
     "DescribeClustersMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+DescribeCustomDomainAssociationsMessageRequestTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageRequestTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    {
+        "ConsumerArn": str,
+        "Status": DataShareStatusForConsumerType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSharesForConsumerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
     {
         "ConsumerArn": str,
         "Status": DataShareStatusForConsumerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    {
+        "ProducerArn": str,
+        "Status": DataShareStatusForProducerType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSharesForProducerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     {
         "ProducerArn": str,
         "Status": DataShareStatusForProducerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    {
+        "DataShareArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDataSharesMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
+    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDefaultClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupFamily": str,
     },
 )
 _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1211,27 +1455,50 @@
 
 class DescribeDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ResourceOwner": str,
+        "EndpointName": str,
+        "VpcId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointAccessMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "EndpointName": str,
         "VpcId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "Account": str,
+        "Grantee": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointAuthorizationMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "Grantee": bool,
         "MaxRecords": int,
@@ -1244,52 +1511,98 @@
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Duration": int,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeHsmConfigurationsMessageRequestTypeDef = TypedDict(
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1311,14 +1624,24 @@
         "Name": NodeConfigurationOptionsFilterNameType,
         "Operator": OperatorTypeType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "NodeType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeOrderableClusterOptionsMessageRequestTypeDef = TypedDict(
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "NodeType": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1357,35 +1680,63 @@
         "StatusMessage": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "ReservedNodeExchangeRequestId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "ReservedNodeExchangeRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeOfferingId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodeOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
     {
         "ReservedNodeOfferingId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReservedNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodesMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1403,63 +1754,121 @@
     "ScheduledActionFilterTypeDef",
     {
         "Name": ScheduledActionFilterNameType,
         "Values": Sequence[str],
     },
 )
 
+DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotCopyGrantsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ScheduleIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSnapshotSchedulesMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ScheduleIdentifier": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TableRestoreRequestId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeTableRestoreStatusMessageRequestTypeDef = TypedDict(
     "DescribeTableRestoreStatusMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "TableRestoreRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+        "ResourceType": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeTagsMessageRequestTypeDef = TypedDict(
     "DescribeTagsMessageRequestTypeDef",
     {
         "ResourceName": str,
         "ResourceType": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
+DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeUsageLimitsMessageRequestTypeDef = TypedDict(
     "DescribeUsageLimitsMessageRequestTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "MaxRecords": int,
@@ -1502,14 +1911,21 @@
 
 class DisassociateDataShareConsumerMessageRequestTypeDef(
     _RequiredDisassociateDataShareConsumerMessageRequestTypeDef,
     _OptionalDisassociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEnableLoggingMessageRequestTypeDef = TypedDict(
     "_RequiredEnableLoggingMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalEnableLoggingMessageRequestTypeDef = TypedDict(
@@ -1563,14 +1979,30 @@
         "AllowedAllVPCs": bool,
         "AllowedVPCs": List[str],
         "EndpointCount": int,
     },
     total=False,
 )
 
+EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
+    "EndpointAuthorizationResponseMetadataTypeDef",
+    {
+        "Grantor": str,
+        "Grantee": str,
+        "ClusterIdentifier": str,
+        "AuthorizeTime": datetime,
+        "ClusterStatus": str,
+        "Status": AuthorizationStatusType,
+        "AllowedAllVPCs": bool,
+        "AllowedVPCs": List[str],
+        "EndpointCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventInfoMapTypeDef = TypedDict(
     "EventInfoMapTypeDef",
     {
         "EventId": str,
         "EventCategories": List[str],
         "EventDescription": str,
         "Severity": str,
@@ -1592,52 +2024,65 @@
     total=False,
 )
 
 _RequiredGetClusterCredentialsMessageRequestTypeDef = TypedDict(
     "_RequiredGetClusterCredentialsMessageRequestTypeDef",
     {
         "DbUser": str,
-        "ClusterIdentifier": str,
     },
 )
 _OptionalGetClusterCredentialsMessageRequestTypeDef = TypedDict(
     "_OptionalGetClusterCredentialsMessageRequestTypeDef",
     {
         "DbName": str,
+        "ClusterIdentifier": str,
         "DurationSeconds": int,
         "AutoCreate": bool,
         "DbGroups": Sequence[str],
+        "CustomDomainName": str,
     },
     total=False,
 )
 
 class GetClusterCredentialsMessageRequestTypeDef(
     _RequiredGetClusterCredentialsMessageRequestTypeDef,
     _OptionalGetClusterCredentialsMessageRequestTypeDef,
 ):
     pass
 
-_RequiredGetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
-    "_RequiredGetClusterCredentialsWithIAMMessageRequestTypeDef",
+GetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
+    "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     {
+        "DbName": str,
         "ClusterIdentifier": str,
+        "DurationSeconds": int,
+        "CustomDomainName": str,
     },
+    total=False,
 )
-_OptionalGetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
-    "_OptionalGetClusterCredentialsWithIAMMessageRequestTypeDef",
+
+_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     {
-        "DbName": str,
-        "DurationSeconds": int,
+        "ActionType": ReservedNodeExchangeActionTypeType,
+    },
+)
+_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "SnapshotIdentifier": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class GetClusterCredentialsWithIAMMessageRequestTypeDef(
-    _RequiredGetClusterCredentialsWithIAMMessageRequestTypeDef,
-    _OptionalGetClusterCredentialsWithIAMMessageRequestTypeDef,
+class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
 ):
     pass
 
 _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     {
         "ActionType": ReservedNodeExchangeActionTypeType,
@@ -1656,14 +2101,34 @@
 
 class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
 ):
     pass
 
+_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+    },
+)
+_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
     },
 )
 _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
@@ -1677,14 +2142,29 @@
 
 class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
 ):
     pass
 
+LoggingStatusTypeDef = TypedDict(
+    "LoggingStatusTypeDef",
+    {
+        "LoggingEnabled": bool,
+        "BucketName": str,
+        "S3KeyPrefix": str,
+        "LastSuccessfulDeliveryTime": datetime,
+        "LastFailureTime": datetime,
+        "LastFailureMessage": str,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogExports": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_RequiredModifyAquaInputMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyAquaInputMessageRequestTypeDef = TypedDict(
@@ -1704,14 +2184,23 @@
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
+ModifyAuthenticationProfileResultTypeDef = TypedDict(
+    "ModifyAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ModifyClusterDbRevisionMessageRequestTypeDef = TypedDict(
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RevisionTarget": str,
     },
 )
@@ -1863,14 +2352,46 @@
 
 class ModifyClusterSubnetGroupMessageRequestTypeDef(
     _RequiredModifyClusterSubnetGroupMessageRequestTypeDef,
     _OptionalModifyClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+_RequiredModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyCustomDomainAssociationMessageRequestTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+    },
+    total=False,
+)
+
+class ModifyCustomDomainAssociationMessageRequestTypeDef(
+    _RequiredModifyCustomDomainAssociationMessageRequestTypeDef,
+    _OptionalModifyCustomDomainAssociationMessageRequestTypeDef,
+):
+    pass
+
+ModifyCustomDomainAssociationResultTypeDef = TypedDict(
+    "ModifyCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 _OptionalModifyEndpointAccessMessageRequestTypeDef = TypedDict(
@@ -1979,24 +2500,43 @@
         "NumberOfNodes": int,
         "EstimatedDiskUtilizationPercent": float,
         "Mode": ModeType,
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
 PartnerIntegrationInputMessageRequestTypeDef = TypedDict(
     "PartnerIntegrationInputMessageRequestTypeDef",
     {
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
+PartnerIntegrationOutputMessageTypeDef = TypedDict(
+    "PartnerIntegrationOutputMessageTypeDef",
+    {
+        "DatabaseName": str,
+        "PartnerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2094,14 +2634,48 @@
 )
 
 class ResizeClusterMessageTypeDef(
     _RequiredResizeClusterMessageTypeDef, _OptionalResizeClusterMessageTypeDef
 ):
     pass
 
+ResizeProgressMessageTypeDef = TypedDict(
+    "ResizeProgressMessageTypeDef",
+    {
+        "TargetNodeType": str,
+        "TargetNumberOfNodes": int,
+        "TargetClusterType": str,
+        "Status": str,
+        "ImportTablesCompleted": List[str],
+        "ImportTablesInProgress": List[str],
+        "ImportTablesNotStarted": List[str],
+        "AvgResizeRateInMegaBytesPerSecond": float,
+        "TotalResizeDataInMegaBytes": int,
+        "ProgressInMegaBytes": int,
+        "ElapsedTimeInSeconds": int,
+        "EstimatedTimeToCompletionInSeconds": int,
+        "ResizeType": str,
+        "Message": str,
+        "TargetEncryptionType": str,
+        "DataTransferProgressPercent": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
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
 _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2301,171 +2875,46 @@
 
 class UpdatePartnerStatusInputMessageRequestTypeDef(
     _RequiredUpdatePartnerStatusInputMessageRequestTypeDef,
     _OptionalUpdatePartnerStatusInputMessageRequestTypeDef,
 ):
     pass
 
-ClusterCredentialsTypeDef = TypedDict(
-    "ClusterCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClusterExtendedCredentialsTypeDef = TypedDict(
-    "ClusterExtendedCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "NextRefreshTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "ClusterParameterGroupNameMessageTypeDef",
-    {
-        "ParameterGroupName": str,
-        "ParameterGroupStatus": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAuthenticationProfileResultTypeDef = TypedDict(
-    "CreateAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CustomerStorageMessageTypeDef = TypedDict(
-    "CustomerStorageMessageTypeDef",
-    {
-        "TotalBackupSizeInMegaBytes": float,
-        "TotalProvisionedStorageInMegaBytes": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteAuthenticationProfileResultTypeDef = TypedDict(
-    "DeleteAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    {
-        "Grantor": str,
-        "Grantee": str,
-        "ClusterIdentifier": str,
-        "AuthorizeTime": datetime,
-        "ClusterStatus": str,
-        "Status": AuthorizationStatusType,
-        "AllowedAllVPCs": bool,
-        "AllowedVPCs": List[str],
-        "EndpointCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LoggingStatusTypeDef = TypedDict(
-    "LoggingStatusTypeDef",
-    {
-        "LoggingEnabled": bool,
-        "BucketName": str,
-        "S3KeyPrefix": str,
-        "LastSuccessfulDeliveryTime": datetime,
-        "LastFailureTime": datetime,
-        "LastFailureMessage": str,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogExports": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModifyAuthenticationProfileResultTypeDef = TypedDict(
-    "ModifyAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PartnerIntegrationOutputMessageTypeDef = TypedDict(
-    "PartnerIntegrationOutputMessageTypeDef",
-    {
-        "DatabaseName": str,
-        "PartnerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResizeProgressMessageTypeDef = TypedDict(
-    "ResizeProgressMessageTypeDef",
-    {
-        "TargetNodeType": str,
-        "TargetNumberOfNodes": int,
-        "TargetClusterType": str,
-        "Status": str,
-        "ImportTablesCompleted": List[str],
-        "ImportTablesInProgress": List[str],
-        "ImportTablesNotStarted": List[str],
-        "AvgResizeRateInMegaBytesPerSecond": float,
-        "TotalResizeDataInMegaBytes": int,
-        "ProgressInMegaBytes": int,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ResizeType": str,
-        "Message": str,
-        "TargetEncryptionType": str,
-        "DataTransferProgressPercent": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AttributeValueTargetTypeDef],
     },
     total=False,
 )
 
 ModifyAquaOutputMessageTypeDef = TypedDict(
     "ModifyAquaOutputMessageTypeDef",
     {
         "AquaConfiguration": AquaConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AssociationTypeDef = TypedDict(
+    "AssociationTypeDef",
+    {
+        "CustomDomainCertificateArn": str,
+        "CustomDomainCertificateExpiryDate": datetime,
+        "CertificateAssociations": List[CertificateAssociationTypeDef],
+    },
+    total=False,
+)
+
 DescribeAuthenticationProfilesResultTypeDef = TypedDict(
     "DescribeAuthenticationProfilesResultTypeDef",
     {
         "AuthenticationProfiles": List[AuthenticationProfileTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
@@ -2482,24 +2931,24 @@
 )
 
 BatchDeleteClusterSnapshotsResultTypeDef = TypedDict(
     "BatchDeleteClusterSnapshotsResultTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchModifyClusterSnapshotsOutputMessageTypeDef = TypedDict(
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterDbRevisionTypeDef = TypedDict(
     "ClusterDbRevisionTypeDef",
     {
         "ClusterIdentifier": str,
@@ -2511,15 +2960,15 @@
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
@@ -2931,15 +3380,15 @@
         "ScheduleDefinitions": List[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": List[TagTypeDef],
         "NextInvocations": List[datetime],
         "AssociatedClusterCount": int,
         "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotScheduleTypeDef = TypedDict(
     "SnapshotScheduleTypeDef",
     {
         "ScheduleDefinitions": List[str],
@@ -3011,15 +3460,15 @@
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "LimitType": UsageLimitLimitTypeType,
         "Amount": int,
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsageLimitTypeDef = TypedDict(
     "UsageLimitTypeDef",
     {
         "UsageLimitId": str,
@@ -3035,36 +3484,36 @@
 )
 
 DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     {
         "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterVersionsMessageTypeDef = TypedDict(
     "ClusterVersionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataShareResponseMetadataTypeDef = TypedDict(
     "DataShareResponseMetadataTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataShareTypeDef = TypedDict(
     "DataShareTypeDef",
     {
         "DataShareArn": str,
@@ -3072,378 +3521,29 @@
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
     },
     total=False,
 )
 
-DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
-    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-):
-    pass
-
-DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    {
-        "ClusterSubnetGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    {
-        "MaintenanceTrackName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "ClusterParameterGroupFamily": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    {
-        "ConsumerArn": str,
-        "Status": DataShareStatusForConsumerType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    {
-        "ProducerArn": str,
-        "Status": DataShareStatusForProducerType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    {
-        "DataShareArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
-    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-):
-    pass
-
-DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ResourceOwner": str,
-        "EndpointName": str,
-        "VpcId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "Account": str,
-        "Grantee": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "NodeType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "ReservedNodeExchangeRequestId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeOfferingId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ScheduleIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TableRestoreRequestId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "ResourceType": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ActionType": ReservedNodeExchangeActionTypeType,
-    },
-)
-_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "SnapshotIdentifier": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-    },
-)
-_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-):
-    pass
-
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
@@ -3534,15 +3634,15 @@
     "_OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "OwnerAccount": str,
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -3575,28 +3675,28 @@
 ):
     pass
 
 DescribePartnersOutputMessageTypeDef = TypedDict(
     "DescribePartnersOutputMessageTypeDef",
     {
         "PartnerIntegrationInfoList": List[PartnerIntegrationInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
@@ -3613,15 +3713,15 @@
 )
 
 EndpointAuthorizationListTypeDef = TypedDict(
     "EndpointAuthorizationListTypeDef",
     {
         "EndpointAuthorizationList": List[EndpointAuthorizationTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
@@ -3631,15 +3731,15 @@
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
@@ -3650,15 +3750,15 @@
 )
 
 NodeConfigurationOptionsMessageTypeDef = TypedDict(
     "NodeConfigurationOptionsMessageTypeDef",
     {
         "NodeConfigurationOptionList": List[NodeConfigurationOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedNodeOfferingTypeDef = TypedDict(
     "ReservedNodeOfferingTypeDef",
     {
         "ReservedNodeOfferingId": str,
@@ -3694,24 +3794,24 @@
     total=False,
 )
 
 RestoreTableFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreTableFromClusterSnapshotResultTypeDef",
     {
         "TableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableRestoreStatusMessageTypeDef = TypedDict(
     "TableRestoreStatusMessageTypeDef",
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
@@ -3731,15 +3831,24 @@
     total=False,
 )
 
 AccountAttributeListTypeDef = TypedDict(
     "AccountAttributeListTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CustomDomainAssociationsMessageTypeDef = TypedDict(
+    "CustomDomainAssociationsMessageTypeDef",
+    {
+        "Marker": str,
+        "Associations": List[AssociationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OrderableClusterOptionTypeDef = TypedDict(
     "OrderableClusterOptionTypeDef",
     {
         "ClusterVersion": str,
@@ -3761,99 +3870,99 @@
 )
 
 ClusterDbRevisionsMessageTypeDef = TypedDict(
     "ClusterDbRevisionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterDbRevisions": List[ClusterDbRevisionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeDefaultClusterParametersResultTypeDef",
     {
         "DefaultClusterParameters": DefaultClusterParametersTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterParameterGroupsMessageTypeDef = TypedDict(
     "ClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "ParameterGroups": List[ClusterParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterParameterGroupResultTypeDef = TypedDict(
     "CreateClusterParameterGroupResultTypeDef",
     {
         "ClusterParameterGroup": ClusterParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHsmClientCertificateResultTypeDef = TypedDict(
     "CreateHsmClientCertificateResultTypeDef",
     {
         "HsmClientCertificate": HsmClientCertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HsmClientCertificateMessageTypeDef = TypedDict(
     "HsmClientCertificateMessageTypeDef",
     {
         "Marker": str,
         "HsmClientCertificates": List[HsmClientCertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHsmConfigurationResultTypeDef = TypedDict(
     "CreateHsmConfigurationResultTypeDef",
     {
         "HsmConfiguration": HsmConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HsmConfigurationMessageTypeDef = TypedDict(
     "HsmConfigurationMessageTypeDef",
     {
         "Marker": str,
         "HsmConfigurations": List[HsmConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
@@ -3865,143 +3974,143 @@
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
         "SnapshotCopyGrant": SnapshotCopyGrantTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotCopyGrantMessageTypeDef = TypedDict(
     "SnapshotCopyGrantMessageTypeDef",
     {
         "Marker": str,
         "SnapshotCopyGrants": List[SnapshotCopyGrantTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotSchedulesOutputMessageTypeDef = TypedDict(
     "DescribeSnapshotSchedulesOutputMessageTypeDef",
     {
         "SnapshotSchedules": List[SnapshotScheduleTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizeSnapshotAccessResultTypeDef = TypedDict(
     "AuthorizeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopyClusterSnapshotResultTypeDef = TypedDict(
     "CopyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterSnapshotResultTypeDef = TypedDict(
     "CreateClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterSnapshotResultTypeDef = TypedDict(
     "DeleteClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterSnapshotResultTypeDef = TypedDict(
     "ModifyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RevokeSnapshotAccessResultTypeDef = TypedDict(
     "RevokeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotMessageTypeDef = TypedDict(
     "SnapshotMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaggedResourceListMessageTypeDef = TypedDict(
     "TaggedResourceListMessageTypeDef",
     {
         "TaggedResources": List[TaggedResourceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsageLimitListTypeDef = TypedDict(
     "UsageLimitListTypeDef",
     {
         "UsageLimits": List[UsageLimitTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSharesForConsumerResultTypeDef = TypedDict(
     "DescribeDataSharesForConsumerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSharesForProducerResultTypeDef = TypedDict(
     "DescribeDataSharesForProducerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataSharesResultTypeDef = TypedDict(
     "DescribeDataSharesResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointAccessResponseMetadataTypeDef = TypedDict(
     "EndpointAccessResponseMetadataTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4010,15 +4119,15 @@
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
         "Port": int,
         "Address": str,
         "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4046,40 +4155,40 @@
 )
 
 GetReservedNodeExchangeOfferingsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedNodeOfferingsMessageTypeDef = TypedDict(
     "ReservedNodeOfferingsMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AcceptReservedNodeExchangeOutputMessageTypeDef = TypedDict(
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     {
         "ExchangedReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseReservedNodeOfferingResultTypeDef = TypedDict(
     "PurchaseReservedNodeOfferingResultTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservedNodeConfigurationOptionTypeDef = TypedDict(
     "ReservedNodeConfigurationOptionTypeDef",
     {
         "SourceReservedNode": ReservedNodeTypeDef,
@@ -4090,15 +4199,15 @@
 )
 
 ReservedNodesMessageTypeDef = TypedDict(
     "ReservedNodesMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
@@ -4158,15 +4267,15 @@
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
         "State": ScheduledActionStateType,
         "NextInvocations": List[datetime],
         "StartTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionTypeDef = TypedDict(
     "ScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
@@ -4193,15 +4302,15 @@
 )
 
 OrderableClusterOptionsMessageTypeDef = TypedDict(
     "OrderableClusterOptionsMessageTypeDef",
     {
         "OrderableClusterOptions": List[OrderableClusterOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSubnetGroupTypeDef = TypedDict(
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
@@ -4214,49 +4323,49 @@
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSecurityGroupMessageTypeDef = TypedDict(
     "ClusterSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSecurityGroups": List[ClusterSecurityGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterSecurityGroupResultTypeDef = TypedDict(
     "CreateClusterSecurityGroupResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RevokeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointAccessListTypeDef = TypedDict(
     "EndpointAccessListTypeDef",
     {
         "EndpointAccessList": List[EndpointAccessTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4307,191 +4416,194 @@
         "ResizeInfo": ResizeInfoTypeDef,
         "AvailabilityZoneRelocationStatus": str,
         "ClusterNamespaceArn": str,
         "TotalStorageCapacityInMegaBytes": int,
         "AquaConfiguration": AquaConfigurationTypeDef,
         "DefaultIamRoleArn": str,
         "ReservedNodeExchangeStatus": ReservedNodeExchangeStatusTypeDef,
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "CustomDomainCertificateExpiryDate": datetime,
     },
     total=False,
 )
 
 GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeConfigurationOptionList": List[ReservedNodeConfigurationOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScheduledActionsMessageTypeDef = TypedDict(
     "ScheduledActionsMessageTypeDef",
     {
         "Marker": str,
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TrackListMessageTypeDef = TypedDict(
     "TrackListMessageTypeDef",
     {
         "MaintenanceTracks": List[MaintenanceTrackTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterSubnetGroupMessageTypeDef = TypedDict(
     "ClusterSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSubnetGroups": List[ClusterSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterSubnetGroupResultTypeDef = TypedDict(
     "CreateClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterSubnetGroupResultTypeDef = TypedDict(
     "ModifyClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClustersMessageTypeDef = TypedDict(
     "ClustersMessageTypeDef",
     {
         "Marker": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResultTypeDef = TypedDict(
     "DeleteClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisableSnapshotCopyResultTypeDef = TypedDict(
     "DisableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnableSnapshotCopyResultTypeDef = TypedDict(
     "EnableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterDbRevisionResultTypeDef = TypedDict(
     "ModifyClusterDbRevisionResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterIamRolesResultTypeDef = TypedDict(
     "ModifyClusterIamRolesResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterMaintenanceResultTypeDef = TypedDict(
     "ModifyClusterMaintenanceResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyClusterResultTypeDef = TypedDict(
     "ModifyClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifySnapshotCopyRetentionPeriodResultTypeDef = TypedDict(
     "ModifySnapshotCopyRetentionPeriodResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PauseClusterResultTypeDef = TypedDict(
     "PauseClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootClusterResultTypeDef = TypedDict(
     "RebootClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResizeClusterResultTypeDef = TypedDict(
     "ResizeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreFromClusterSnapshotResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResumeClusterResultTypeDef = TypedDict(
     "ResumeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateEncryptionKeyResultTypeDef = TypedDict(
     "RotateEncryptionKeyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.py` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.pyi` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy-boto3-redshift-1.27.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-redshift
-Version: 1.26.79
-Summary: Type annotations for boto3.Redshift 1.26.79 service generated with mypy-boto3-builder 7.12.4
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 redshift type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-redshift"></a>
 
 # mypy-boto3-redshift
 
 [![PyPI - mypy-boto3-redshift](https://img.shields.io/pypi/v/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,14 +257,15 @@
     DescribeClusterParametersPaginator,
     DescribeClusterSecurityGroupsPaginator,
     DescribeClusterSnapshotsPaginator,
     DescribeClusterSubnetGroupsPaginator,
     DescribeClusterTracksPaginator,
     DescribeClusterVersionsPaginator,
     DescribeClustersPaginator,
+    DescribeCustomDomainAssociationsPaginator,
     DescribeDataSharesPaginator,
     DescribeDataSharesForConsumerPaginator,
     DescribeDataSharesForProducerPaginator,
     DescribeDefaultClusterParametersPaginator,
     DescribeEndpointAccessPaginator,
     DescribeEndpointAuthorizationPaginator,
     DescribeEventSubscriptionsPaginator,
@@ -343,14 +312,17 @@
 describe_cluster_tracks_paginator: DescribeClusterTracksPaginator = client.get_paginator(
     "describe_cluster_tracks"
 )
 describe_cluster_versions_paginator: DescribeClusterVersionsPaginator = client.get_paginator(
     "describe_cluster_versions"
 )
 describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+describe_custom_domain_associations_paginator: DescribeCustomDomainAssociationsPaginator = (
+    client.get_paginator("describe_custom_domain_associations")
+)
 describe_data_shares_paginator: DescribeDataSharesPaginator = client.get_paginator(
     "describe_data_shares"
 )
 describe_data_shares_for_consumer_paginator: DescribeDataSharesForConsumerPaginator = (
     client.get_paginator("describe_data_shares_for_consumer")
 )
 describe_data_shares_for_producer_paginator: DescribeDataSharesForProducerPaginator = (
@@ -465,14 +437,15 @@
     DescribeClusterParametersPaginatorName,
     DescribeClusterSecurityGroupsPaginatorName,
     DescribeClusterSnapshotsPaginatorName,
     DescribeClusterSubnetGroupsPaginatorName,
     DescribeClusterTracksPaginatorName,
     DescribeClusterVersionsPaginatorName,
     DescribeClustersPaginatorName,
+    DescribeCustomDomainAssociationsPaginatorName,
     DescribeDataSharesForConsumerPaginatorName,
     DescribeDataSharesForProducerPaginatorName,
     DescribeDataSharesPaginatorName,
     DescribeDefaultClusterParametersPaginatorName,
     DescribeEndpointAccessPaginatorName,
     DescribeEndpointAuthorizationPaginatorName,
     DescribeEventSubscriptionsPaginatorName,
@@ -533,34 +506,37 @@
 
 `mypy_boto3_redshift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
+    CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     AuthorizeDataShareMessageRequestTypeDef,
     AuthorizeEndpointAccessMessageRequestTypeDef,
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
+    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
+    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
     ParameterTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
     ClusterParameterStatusTypeDef,
     TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
@@ -569,133 +545,168 @@
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationMessageRequestTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
+    CustomerStorageMessageTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
+    DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteHsmClientCertificateMessageRequestTypeDef,
     DeleteHsmConfigurationMessageRequestTypeDef,
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageRequestTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
+    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
+    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
+    ModifyCustomDomainAssociationMessageRequestTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
+    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
+    ResizeProgressMessageTypeDef,
+    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
-    ClusterCredentialsTypeDef,
-    ClusterExtendedCredentialsTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
-    CustomerStorageMessageTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
-    LoggingStatusTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
-    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
+    AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
@@ -728,43 +739,14 @@
     TaggedResourceTypeDef,
     UsageLimitResponseMetadataTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
     DataShareResponseMetadataTypeDef,
     DataShareTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -780,14 +762,15 @@
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
+    CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
     DescribeDefaultClusterParametersResultTypeDef,
     ClusterParameterGroupsMessageTypeDef,
     CreateClusterParameterGroupResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
@@ -868,42 +851,42 @@
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

### Comparing `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy-boto3-redshift-1.27.0/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.79/setup.py` & `mypy-boto3-redshift-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-redshift.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.26.79",
+    version="1.27.0",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Redshift 1.26.79 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.Redshift 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/",
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


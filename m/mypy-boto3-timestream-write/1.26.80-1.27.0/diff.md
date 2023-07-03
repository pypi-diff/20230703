# Comparing `tmp/mypy-boto3-timestream-write-1.26.80.tar.gz` & `tmp/mypy-boto3-timestream-write-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-write-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-write-1.27.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
```

## Comparing `mypy-boto3-timestream-write-1.26.80.tar` & `mypy-boto3-timestream-write-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20497 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-02-27 20:35:18.000000 mypy-boto3-timestream-write-1.26.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.672100 mypy-boto3-timestream-write-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-03 19:51:33.672100 mypy-boto3-timestream-write-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.664100 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21308 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.672100 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-03 19:51:33.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-03 19:51:33.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:33.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:33.000000 mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:33.672100 mypy-boto3-timestream-write-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 19:49:06.000000 mypy-boto3-timestream-write-1.27.0/setup.py
```

### Comparing `mypy-boto3-timestream-write-1.26.80/LICENSE` & `mypy-boto3-timestream-write-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-timestream-write-1.26.80/PKG-INFO` & `mypy-boto3-timestream-write-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.26.80
-Summary: Type annotations for boto3.TimestreamWrite 1.26.80 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.TimestreamWrite 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,14 +281,16 @@
 
 ```python
 from mypy_boto3_timestream_write.literals import (
     BatchLoadDataFormatType,
     BatchLoadStatusType,
     DimensionValueTypeType,
     MeasureValueTypeType,
+    PartitionKeyEnforcementLevelType,
+    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
     TimestreamWriteServiceName,
     ServiceName,
     ResourceServiceName,
@@ -307,57 +309,59 @@
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
     CsvConfigurationTypeDef,
     DataModelS3ConfigurationTypeDef,
     DimensionMappingTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
@@ -380,42 +384,42 @@
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

### Comparing `mypy-boto3-timestream-write-1.26.80/README.md` & `mypy-boto3-timestream-write-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,14 +249,16 @@
 
 ```python
 from mypy_boto3_timestream_write.literals import (
     BatchLoadDataFormatType,
     BatchLoadStatusType,
     DimensionValueTypeType,
     MeasureValueTypeType,
+    PartitionKeyEnforcementLevelType,
+    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
     TimestreamWriteServiceName,
     ServiceName,
     ResourceServiceName,
@@ -275,57 +277,59 @@
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
     CsvConfigurationTypeDef,
     DataModelS3ConfigurationTypeDef,
     DimensionMappingTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
@@ -348,42 +352,42 @@
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

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__main__.py` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamWrite 1.26.80\nVersion:         1.26.80\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.TimestreamWrite 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.80")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.py` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
+    SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -131,15 +132,16 @@
     def create_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
+        Schema: SchemaTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -286,15 +288,16 @@
 
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
+        Schema: SchemaTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.pyi` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
+    SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -123,15 +124,16 @@
     def create_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
+        Schema: SchemaTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -262,15 +264,16 @@
         """
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
+        Schema: SchemaTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.py` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 
 __all__ = (
     "BatchLoadDataFormatType",
     "BatchLoadStatusType",
     "DimensionValueTypeType",
     "MeasureValueTypeType",
+    "PartitionKeyEnforcementLevelType",
+    "PartitionKeyTypeType",
     "S3EncryptionOptionType",
     "ScalarMeasureValueTypeType",
     "TableStatusType",
     "TimeUnitType",
     "TimestreamWriteServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -37,14 +39,16 @@
 
 BatchLoadDataFormatType = Literal["CSV"]
 BatchLoadStatusType = Literal[
     "CREATED", "FAILED", "IN_PROGRESS", "PENDING_RESUME", "PROGRESS_STOPPED", "SUCCEEDED"
 ]
 DimensionValueTypeType = Literal["VARCHAR"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "TIMESTAMP", "VARCHAR"]
+PartitionKeyEnforcementLevelType = Literal["OPTIONAL", "REQUIRED"]
+PartitionKeyTypeType = Literal["DIMENSION", "MEASURE"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
 TableStatusType = Literal["ACTIVE", "DELETING", "RESTORING"]
 TimeUnitType = Literal["MICROSECONDS", "MILLISECONDS", "NANOSECONDS", "SECONDS"]
 TimestreamWriteServiceName = Literal["timestream-write"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -57,14 +61,15 @@
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
@@ -104,14 +109,15 @@
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
@@ -209,14 +215,15 @@
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
@@ -252,14 +259,15 @@
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
@@ -278,16 +286,19 @@
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
@@ -371,15 +382,17 @@
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

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.pyi` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     from typing_extensions import Literal
 
 __all__ = (
     "BatchLoadDataFormatType",
     "BatchLoadStatusType",
     "DimensionValueTypeType",
     "MeasureValueTypeType",
+    "PartitionKeyEnforcementLevelType",
+    "PartitionKeyTypeType",
     "S3EncryptionOptionType",
     "ScalarMeasureValueTypeType",
     "TableStatusType",
     "TimeUnitType",
     "TimestreamWriteServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -35,14 +37,16 @@
 
 BatchLoadDataFormatType = Literal["CSV"]
 BatchLoadStatusType = Literal[
     "CREATED", "FAILED", "IN_PROGRESS", "PENDING_RESUME", "PROGRESS_STOPPED", "SUCCEEDED"
 ]
 DimensionValueTypeType = Literal["VARCHAR"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "TIMESTAMP", "VARCHAR"]
+PartitionKeyEnforcementLevelType = Literal["OPTIONAL", "REQUIRED"]
+PartitionKeyTypeType = Literal["DIMENSION", "MEASURE"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
 TableStatusType = Literal["ACTIVE", "DELETING", "RESTORING"]
 TimeUnitType = Literal["MICROSECONDS", "MILLISECONDS", "NANOSECONDS", "SECONDS"]
 TimestreamWriteServiceName = Literal["timestream-write"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -55,14 +59,15 @@
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
@@ -102,14 +107,15 @@
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
@@ -207,14 +213,15 @@
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
@@ -250,14 +257,15 @@
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
@@ -276,16 +284,19 @@
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
@@ -369,15 +380,17 @@
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

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.py` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
+    PartitionKeyEnforcementLevelType,
+    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
 )
 
 if sys.version_info >= (3, 9):
@@ -33,57 +35,59 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBatchLoadTaskResponseTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
     "CsvConfigurationTypeDef",
     "DataModelS3ConfigurationTypeDef",
     "DimensionMappingTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
+    "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
     "ReportS3ConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
-    "CreateBatchLoadTaskResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
@@ -121,22 +125,19 @@
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBatchLoadTaskResponseTypeDef = TypedDict(
+    "CreateBatchLoadTaskResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "TaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -277,14 +278,21 @@
 )
 
 
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -355,14 +363,34 @@
 
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
 
+_RequiredPartitionKeyTypeDef = TypedDict(
+    "_RequiredPartitionKeyTypeDef",
+    {
+        "Type": PartitionKeyTypeType,
+    },
+)
+_OptionalPartitionKeyTypeDef = TypedDict(
+    "_OptionalPartitionKeyTypeDef",
+    {
+        "Name": str,
+        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
+    },
+    total=False,
+)
+
+
+class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
+    pass
+
+
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
@@ -388,14 +416,25 @@
 
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
 
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
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
@@ -411,35 +450,20 @@
     "UpdateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "KmsKeyId": str,
     },
 )
 
-CreateBatchLoadTaskResponseTypeDef = TypedDict(
-    "CreateBatchLoadTaskResponseTypeDef",
-    {
-        "TaskId": str,
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
 ListBatchLoadTasksResponseTypeDef = TypedDict(
     "ListBatchLoadTasksResponseTypeDef",
     {
         "NextToken": str,
         "BatchLoadTasks": List[BatchLoadTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -461,15 +485,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -477,40 +501,40 @@
     },
 )
 
 CreateDatabaseResponseTypeDef = TypedDict(
     "CreateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatabaseResponseTypeDef = TypedDict(
     "DescribeDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatabasesResponseTypeDef = TypedDict(
     "ListDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDatabaseResponseTypeDef = TypedDict(
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
@@ -532,15 +556,15 @@
     pass
 
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -604,19 +628,27 @@
 
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
 
+SchemaTypeDef = TypedDict(
+    "SchemaTypeDef",
+    {
+        "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
+    },
+    total=False,
+)
+
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
@@ -700,14 +732,15 @@
 )
 _OptionalCreateTableRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
@@ -722,14 +755,15 @@
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -738,14 +772,15 @@
     },
 )
 _OptionalUpdateTableRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
@@ -762,40 +797,40 @@
     total=False,
 )
 
 CreateTableResponseTypeDef = TypedDict(
     "CreateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "Tables": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableResponseTypeDef = TypedDict(
     "UpdateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
@@ -842,10 +877,10 @@
     pass
 
 
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.pyi` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
+    PartitionKeyEnforcementLevelType,
+    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
 )
 
 if sys.version_info >= (3, 9):
@@ -32,57 +34,59 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBatchLoadTaskResponseTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
     "CsvConfigurationTypeDef",
     "DataModelS3ConfigurationTypeDef",
     "DimensionMappingTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
+    "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
     "ReportS3ConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
-    "CreateBatchLoadTaskResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
@@ -120,22 +124,19 @@
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBatchLoadTaskResponseTypeDef = TypedDict(
+    "CreateBatchLoadTaskResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "TaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -272,14 +273,21 @@
     },
     total=False,
 )
 
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -348,14 +356,32 @@
 )
 
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
+_RequiredPartitionKeyTypeDef = TypedDict(
+    "_RequiredPartitionKeyTypeDef",
+    {
+        "Type": PartitionKeyTypeType,
+    },
+)
+_OptionalPartitionKeyTypeDef = TypedDict(
+    "_OptionalPartitionKeyTypeDef",
+    {
+        "Name": str,
+        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
+    },
+    total=False,
+)
+
+class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
+    pass
+
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
@@ -379,14 +405,25 @@
 )
 
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
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
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
@@ -402,35 +439,20 @@
     "UpdateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "KmsKeyId": str,
     },
 )
 
-CreateBatchLoadTaskResponseTypeDef = TypedDict(
-    "CreateBatchLoadTaskResponseTypeDef",
-    {
-        "TaskId": str,
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
 ListBatchLoadTasksResponseTypeDef = TypedDict(
     "ListBatchLoadTasksResponseTypeDef",
     {
         "NextToken": str,
         "BatchLoadTasks": List[BatchLoadTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -450,15 +472,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -466,40 +488,40 @@
     },
 )
 
 CreateDatabaseResponseTypeDef = TypedDict(
     "CreateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatabaseResponseTypeDef = TypedDict(
     "DescribeDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatabasesResponseTypeDef = TypedDict(
     "ListDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDatabaseResponseTypeDef = TypedDict(
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
@@ -519,15 +541,15 @@
 ):
     pass
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -587,19 +609,27 @@
 )
 
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+SchemaTypeDef = TypedDict(
+    "SchemaTypeDef",
+    {
+        "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
+    },
+    total=False,
+)
+
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
@@ -677,14 +707,15 @@
 )
 _OptionalCreateTableRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
@@ -697,14 +728,15 @@
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -713,14 +745,15 @@
     },
 )
 _OptionalUpdateTableRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
+        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
@@ -735,40 +768,40 @@
     total=False,
 )
 
 CreateTableResponseTypeDef = TypedDict(
     "CreateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "Tables": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableResponseTypeDef = TypedDict(
     "UpdateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
@@ -813,10 +846,10 @@
 ):
     pass
 
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/PKG-INFO` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.26.80
-Summary: Type annotations for boto3.TimestreamWrite 1.26.80 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.TimestreamWrite 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,14 +281,16 @@
 
 ```python
 from mypy_boto3_timestream_write.literals import (
     BatchLoadDataFormatType,
     BatchLoadStatusType,
     DimensionValueTypeType,
     MeasureValueTypeType,
+    PartitionKeyEnforcementLevelType,
+    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
     TimestreamWriteServiceName,
     ServiceName,
     ResourceServiceName,
@@ -307,57 +309,59 @@
 `mypy_boto3_timestream_write.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
     CsvConfigurationTypeDef,
     DataModelS3ConfigurationTypeDef,
     DimensionMappingTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
+    PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
@@ -380,42 +384,42 @@
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

### Comparing `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/SOURCES.txt` & `mypy-boto3-timestream-write-1.27.0/mypy_boto3_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.26.80/setup.py` & `mypy-boto3-timestream-write-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-timestream-write.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-write",
-    version="1.26.80",
+    version="1.27.0",
     packages=["mypy_boto3_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamWrite 1.26.80 service generated with"
-        " mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.TimestreamWrite 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/",
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


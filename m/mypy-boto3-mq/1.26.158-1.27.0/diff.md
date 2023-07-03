# Comparing `tmp/mypy-boto3-mq-1.26.158.tar.gz` & `tmp/mypy-boto3-mq-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mq-1.26.158.tar", last modified: Wed Jun 21 19:33:01 2023, max compression
+gzip compressed data, was "mypy-boto3-mq-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
```

## Comparing `mypy-boto3-mq-1.26.158.tar` & `mypy-boto3-mq-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/mypy_boto3_mq/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-06-21 19:32:25.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-06-21 19:32:25.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 19:33:01.000000 mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:33:01.301544 mypy-boto3-mq-1.26.158/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 19:32:24.000000 mypy-boto3-mq-1.26.158/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.291719 mypy-boto3-mq-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-03 19:51:10.291719 mypy-boto3-mq-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.283718 mypy-boto3-mq-1.27.0/mypy_boto3_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28057 2023-07-03 19:42:32.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.291719 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-03 19:51:10.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 19:51:10.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:51:10.000000 mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.291719 mypy-boto3-mq-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 19:42:31.000000 mypy-boto3-mq-1.27.0/setup.py
```

### Comparing `mypy-boto3-mq-1.26.158/LICENSE` & `mypy-boto3-mq-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.158/PKG-INFO` & `mypy-boto3-mq-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.26.158
-Summary: Type annotations for boto3.MQ 1.26.158 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MQ 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.26.158](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,63 +339,63 @@
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBrokerResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
+    DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
-    PaginatorConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListBrokersRequestListBrokersPaginateTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
     PendingLogsTypeDef,
+    PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
+    PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
+    ListBrokersResponseTypeDef,
     ConfigurationsTypeDef,
     ConfigurationTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
-    CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
-    DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PromoteResponseTypeDef,
+    CreateBrokerRequestRequestTypeDef,
+    UpdateBrokerRequestRequestTypeDef,
     DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
```

### Comparing `mypy-boto3-mq-1.26.158/README.md` & `mypy-boto3-mq-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.26.158](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -307,63 +307,63 @@
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBrokerResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
+    DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
-    PaginatorConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListBrokersRequestListBrokersPaginateTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
     PendingLogsTypeDef,
+    PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
+    PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
+    ListBrokersResponseTypeDef,
     ConfigurationsTypeDef,
     ConfigurationTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
-    CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
-    DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PromoteResponseTypeDef,
+    CreateBrokerRequestRequestTypeDef,
+    UpdateBrokerRequestRequestTypeDef,
     DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.py` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/__init__.pyi` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/__main__.py` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MQ 1.26.158\nVersion:         1.26.158\nBuilder version:"
+        "Type annotations for boto3.MQ 1.27.0\nVersion:         1.27.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.158")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.py` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/client.pyi` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.py` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
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
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/literals.pyi` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
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
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.py` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListBrokersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBrokersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
         """
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/paginator.pyi` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListBrokersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBrokersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
         """
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.py` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,63 +43,63 @@
     "ConfigurationIdTypeDef",
     "ConfigurationRevisionTypeDef",
     "EncryptionOptionsTypeDef",
     "LdapServerMetadataInputTypeDef",
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBrokerResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DataReplicationCounterpartTypeDef",
     "DeleteBrokerRequestRequestTypeDef",
+    "DeleteBrokerResponseTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
     "LdapServerMetadataOutputTypeDef",
     "UserSummaryTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserPendingChangesTypeDef",
-    "PaginatorConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListBrokersRequestListBrokersPaginateTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "ListUsersRequestRequestTypeDef",
     "PendingLogsTypeDef",
+    "PaginatorConfigTypeDef",
     "PromoteRequestRequestTypeDef",
+    "PromoteResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SanitizationWarningTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "BrokerInstanceOptionTypeDef",
     "BrokerEngineTypeTypeDef",
+    "ListBrokersResponseTypeDef",
     "ConfigurationsTypeDef",
     "ConfigurationTypeDef",
-    "CreateBrokerRequestRequestTypeDef",
-    "UpdateBrokerRequestRequestTypeDef",
-    "CreateBrokerResponseTypeDef",
     "CreateConfigurationResponseTypeDef",
-    "DeleteBrokerResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListBrokersResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "PromoteResponseTypeDef",
+    "CreateBrokerRequestRequestTypeDef",
+    "UpdateBrokerRequestRequestTypeDef",
     "DataReplicationMetadataOutputTypeDef",
     "ListUsersResponseTypeDef",
     "DescribeUserResponseTypeDef",
-    "ListBrokersRequestListBrokersPaginateTypeDef",
     "LogsSummaryTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     "DescribeBrokerEngineTypesResponseTypeDef",
     "ListConfigurationsResponseTypeDef",
     "UpdateBrokerResponseTypeDef",
     "DescribeBrokerResponseTypeDef",
@@ -304,22 +304,20 @@
 )
 
 
 class WeeklyStartTimeTypeDef(_RequiredWeeklyStartTimeTypeDef, _OptionalWeeklyStartTimeTypeDef):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBrokerResponseTypeDef = TypedDict(
+    "CreateBrokerResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "BrokerArn": str,
+        "BrokerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "EngineType": EngineTypeType,
@@ -401,14 +399,22 @@
 DeleteBrokerRequestRequestTypeDef = TypedDict(
     "DeleteBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
+DeleteBrokerResponseTypeDef = TypedDict(
+    "DeleteBrokerResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTagsRequestRequestTypeDef = TypedDict(
     "DeleteTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -509,14 +515,25 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "ConfigurationId": str,
         "ConfigurationRevision": str,
     },
 )
 
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "Created": datetime,
+        "Data": str,
+        "Description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Username": str,
     },
 )
@@ -539,20 +556,25 @@
 
 class UserPendingChangesTypeDef(
     _RequiredUserPendingChangesTypeDef, _OptionalUserPendingChangesTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
+    "ListBrokersRequestListBrokersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBrokersRequestRequestTypeDef = TypedDict(
     "ListBrokersRequestRequestTypeDef",
     {
@@ -597,14 +619,22 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -628,29 +658,58 @@
     {
         "Audit": bool,
         "General": bool,
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
 PromoteRequestRequestTypeDef = TypedDict(
     "PromoteRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Mode": PromoteModeType,
     },
 )
 
+PromoteResponseTypeDef = TypedDict(
+    "PromoteResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
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
 _RequiredSanitizationWarningTypeDef = TypedDict(
     "_RequiredSanitizationWarningTypeDef",
     {
         "Reason": SanitizationWarningReasonType,
     },
 )
 _OptionalSanitizationWarningTypeDef = TypedDict(
@@ -735,14 +794,23 @@
     {
         "EngineType": EngineTypeType,
         "EngineVersions": List[EngineVersionTypeDef],
     },
     total=False,
 )
 
+ListBrokersResponseTypeDef = TypedDict(
+    "ListBrokersResponseTypeDef",
+    {
+        "BrokerSummaries": List[BrokerSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfigurationsTypeDef = TypedDict(
     "ConfigurationsTypeDef",
     {
         "Current": ConfigurationIdTypeDef,
         "History": List[ConfigurationIdTypeDef],
         "Pending": ConfigurationIdTypeDef,
     },
@@ -772,14 +840,55 @@
 )
 
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
 
+CreateConfigurationResponseTypeDef = TypedDict(
+    "CreateConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeConfigurationResponseTypeDef = TypedDict(
+    "DescribeConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Description": str,
+        "EngineType": EngineTypeType,
+        "EngineVersion": str,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListConfigurationRevisionsResponseTypeDef = TypedDict(
+    "ListConfigurationRevisionsResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "MaxResults": int,
+        "NextToken": str,
+        "Revisions": List[ConfigurationRevisionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBrokerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrokerRequestRequestTypeDef",
     {
         "AutoMinorVersionUpgrade": bool,
         "BrokerName": str,
         "DeploymentMode": DeploymentModeType,
         "EngineType": EngineTypeType,
@@ -842,115 +951,14 @@
 
 class UpdateBrokerRequestRequestTypeDef(
     _RequiredUpdateBrokerRequestRequestTypeDef, _OptionalUpdateBrokerRequestRequestTypeDef
 ):
     pass
 
 
-CreateBrokerResponseTypeDef = TypedDict(
-    "CreateBrokerResponseTypeDef",
-    {
-        "BrokerArn": str,
-        "BrokerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConfigurationResponseTypeDef = TypedDict(
-    "CreateConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBrokerResponseTypeDef = TypedDict(
-    "DeleteBrokerResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeConfigurationResponseTypeDef = TypedDict(
-    "DescribeConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Description": str,
-        "EngineType": EngineTypeType,
-        "EngineVersion": str,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "Created": datetime,
-        "Data": str,
-        "Description": str,
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
-ListBrokersResponseTypeDef = TypedDict(
-    "ListBrokersResponseTypeDef",
-    {
-        "BrokerSummaries": List[BrokerSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationRevisionsResponseTypeDef = TypedDict(
-    "ListConfigurationRevisionsResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PromoteResponseTypeDef = TypedDict(
-    "PromoteResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDataReplicationMetadataOutputTypeDef = TypedDict(
     "_RequiredDataReplicationMetadataOutputTypeDef",
     {
         "DataReplicationRole": str,
     },
 )
 _OptionalDataReplicationMetadataOutputTypeDef = TypedDict(
@@ -971,39 +979,31 @@
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "BrokerId": str,
         "MaxResults": int,
         "NextToken": str,
         "Users": List[UserSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "BrokerId": str,
         "ConsoleAccess": bool,
         "Groups": List[str],
         "Pending": UserPendingChangesTypeDef,
         "Username": str,
         "ReplicationUser": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
-    "ListBrokersRequestListBrokersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredLogsSummaryTypeDef = TypedDict(
     "_RequiredLogsSummaryTypeDef",
     {
         "General": bool,
         "GeneralLogGroup": str,
     },
 )
@@ -1027,45 +1027,45 @@
     {
         "Arn": str,
         "Created": datetime,
         "Id": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "Warnings": List[SanitizationWarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBrokerInstanceOptionsResponseTypeDef = TypedDict(
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     {
         "BrokerInstanceOptions": List[BrokerInstanceOptionTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBrokerEngineTypesResponseTypeDef = TypedDict(
     "DescribeBrokerEngineTypesResponseTypeDef",
     {
         "BrokerEngineTypes": List[BrokerEngineTypeTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBrokerResponseTypeDef = TypedDict(
     "UpdateBrokerResponseTypeDef",
     {
         "AuthenticationStrategy": AuthenticationStrategyType,
@@ -1078,15 +1078,15 @@
         "Logs": LogsTypeDef,
         "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": List[str],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBrokerResponseTypeDef = TypedDict(
     "DescribeBrokerResponseTypeDef",
     {
         "ActionsRequired": List[ActionRequiredTypeDef],
@@ -1118,10 +1118,10 @@
         "SubnetIds": List[str],
         "Tags": Dict[str, str],
         "Users": List[UserSummaryTypeDef],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq/type_defs.pyi` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -42,63 +42,63 @@
     "ConfigurationIdTypeDef",
     "ConfigurationRevisionTypeDef",
     "EncryptionOptionsTypeDef",
     "LdapServerMetadataInputTypeDef",
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateBrokerResponseTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DataReplicationCounterpartTypeDef",
     "DeleteBrokerRequestRequestTypeDef",
+    "DeleteBrokerResponseTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
     "LdapServerMetadataOutputTypeDef",
     "UserSummaryTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserPendingChangesTypeDef",
-    "PaginatorConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListBrokersRequestListBrokersPaginateTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "ListUsersRequestRequestTypeDef",
     "PendingLogsTypeDef",
+    "PaginatorConfigTypeDef",
     "PromoteRequestRequestTypeDef",
+    "PromoteResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SanitizationWarningTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "BrokerInstanceOptionTypeDef",
     "BrokerEngineTypeTypeDef",
+    "ListBrokersResponseTypeDef",
     "ConfigurationsTypeDef",
     "ConfigurationTypeDef",
-    "CreateBrokerRequestRequestTypeDef",
-    "UpdateBrokerRequestRequestTypeDef",
-    "CreateBrokerResponseTypeDef",
     "CreateConfigurationResponseTypeDef",
-    "DeleteBrokerResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListBrokersResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "PromoteResponseTypeDef",
+    "CreateBrokerRequestRequestTypeDef",
+    "UpdateBrokerRequestRequestTypeDef",
     "DataReplicationMetadataOutputTypeDef",
     "ListUsersResponseTypeDef",
     "DescribeUserResponseTypeDef",
-    "ListBrokersRequestListBrokersPaginateTypeDef",
     "LogsSummaryTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     "DescribeBrokerEngineTypesResponseTypeDef",
     "ListConfigurationsResponseTypeDef",
     "UpdateBrokerResponseTypeDef",
     "DescribeBrokerResponseTypeDef",
@@ -289,22 +289,20 @@
     },
     total=False,
 )
 
 class WeeklyStartTimeTypeDef(_RequiredWeeklyStartTimeTypeDef, _OptionalWeeklyStartTimeTypeDef):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateBrokerResponseTypeDef = TypedDict(
+    "CreateBrokerResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "BrokerArn": str,
+        "BrokerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "EngineType": EngineTypeType,
@@ -380,14 +378,22 @@
 DeleteBrokerRequestRequestTypeDef = TypedDict(
     "DeleteBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
+DeleteBrokerResponseTypeDef = TypedDict(
+    "DeleteBrokerResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTagsRequestRequestTypeDef = TypedDict(
     "DeleteTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -484,14 +490,25 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "ConfigurationId": str,
         "ConfigurationRevision": str,
     },
 )
 
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "Created": datetime,
+        "Data": str,
+        "Description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Username": str,
     },
 )
@@ -512,20 +529,25 @@
 )
 
 class UserPendingChangesTypeDef(
     _RequiredUserPendingChangesTypeDef, _OptionalUserPendingChangesTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
+    "ListBrokersRequestListBrokersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBrokersRequestRequestTypeDef = TypedDict(
     "ListBrokersRequestRequestTypeDef",
     {
@@ -568,14 +590,22 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -597,29 +627,58 @@
     {
         "Audit": bool,
         "General": bool,
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
 PromoteRequestRequestTypeDef = TypedDict(
     "PromoteRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Mode": PromoteModeType,
     },
 )
 
+PromoteResponseTypeDef = TypedDict(
+    "PromoteResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
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
 _RequiredSanitizationWarningTypeDef = TypedDict(
     "_RequiredSanitizationWarningTypeDef",
     {
         "Reason": SanitizationWarningReasonType,
     },
 )
 _OptionalSanitizationWarningTypeDef = TypedDict(
@@ -698,14 +757,23 @@
     {
         "EngineType": EngineTypeType,
         "EngineVersions": List[EngineVersionTypeDef],
     },
     total=False,
 )
 
+ListBrokersResponseTypeDef = TypedDict(
+    "ListBrokersResponseTypeDef",
+    {
+        "BrokerSummaries": List[BrokerSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConfigurationsTypeDef = TypedDict(
     "ConfigurationsTypeDef",
     {
         "Current": ConfigurationIdTypeDef,
         "History": List[ConfigurationIdTypeDef],
         "Pending": ConfigurationIdTypeDef,
     },
@@ -733,14 +801,55 @@
     },
     total=False,
 )
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+CreateConfigurationResponseTypeDef = TypedDict(
+    "CreateConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeConfigurationResponseTypeDef = TypedDict(
+    "DescribeConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Description": str,
+        "EngineType": EngineTypeType,
+        "EngineVersion": str,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListConfigurationRevisionsResponseTypeDef = TypedDict(
+    "ListConfigurationRevisionsResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "MaxResults": int,
+        "NextToken": str,
+        "Revisions": List[ConfigurationRevisionTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBrokerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrokerRequestRequestTypeDef",
     {
         "AutoMinorVersionUpgrade": bool,
         "BrokerName": str,
         "DeploymentMode": DeploymentModeType,
         "EngineType": EngineTypeType,
@@ -799,115 +908,14 @@
 )
 
 class UpdateBrokerRequestRequestTypeDef(
     _RequiredUpdateBrokerRequestRequestTypeDef, _OptionalUpdateBrokerRequestRequestTypeDef
 ):
     pass
 
-CreateBrokerResponseTypeDef = TypedDict(
-    "CreateBrokerResponseTypeDef",
-    {
-        "BrokerArn": str,
-        "BrokerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConfigurationResponseTypeDef = TypedDict(
-    "CreateConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBrokerResponseTypeDef = TypedDict(
-    "DeleteBrokerResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeConfigurationResponseTypeDef = TypedDict(
-    "DescribeConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Description": str,
-        "EngineType": EngineTypeType,
-        "EngineVersion": str,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "Created": datetime,
-        "Data": str,
-        "Description": str,
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
-ListBrokersResponseTypeDef = TypedDict(
-    "ListBrokersResponseTypeDef",
-    {
-        "BrokerSummaries": List[BrokerSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListConfigurationRevisionsResponseTypeDef = TypedDict(
-    "ListConfigurationRevisionsResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PromoteResponseTypeDef = TypedDict(
-    "PromoteResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDataReplicationMetadataOutputTypeDef = TypedDict(
     "_RequiredDataReplicationMetadataOutputTypeDef",
     {
         "DataReplicationRole": str,
     },
 )
 _OptionalDataReplicationMetadataOutputTypeDef = TypedDict(
@@ -926,39 +934,31 @@
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "BrokerId": str,
         "MaxResults": int,
         "NextToken": str,
         "Users": List[UserSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "BrokerId": str,
         "ConsoleAccess": bool,
         "Groups": List[str],
         "Pending": UserPendingChangesTypeDef,
         "Username": str,
         "ReplicationUser": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
-    "ListBrokersRequestListBrokersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredLogsSummaryTypeDef = TypedDict(
     "_RequiredLogsSummaryTypeDef",
     {
         "General": bool,
         "GeneralLogGroup": str,
     },
 )
@@ -980,45 +980,45 @@
     {
         "Arn": str,
         "Created": datetime,
         "Id": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "Warnings": List[SanitizationWarningTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBrokerInstanceOptionsResponseTypeDef = TypedDict(
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     {
         "BrokerInstanceOptions": List[BrokerInstanceOptionTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBrokerEngineTypesResponseTypeDef = TypedDict(
     "DescribeBrokerEngineTypesResponseTypeDef",
     {
         "BrokerEngineTypes": List[BrokerEngineTypeTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBrokerResponseTypeDef = TypedDict(
     "UpdateBrokerResponseTypeDef",
     {
         "AuthenticationStrategy": AuthenticationStrategyType,
@@ -1031,15 +1031,15 @@
         "Logs": LogsTypeDef,
         "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": List[str],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBrokerResponseTypeDef = TypedDict(
     "DescribeBrokerResponseTypeDef",
     {
         "ActionsRequired": List[ActionRequiredTypeDef],
@@ -1071,10 +1071,10 @@
         "SubnetIds": List[str],
         "Tags": Dict[str, str],
         "Users": List[UserSummaryTypeDef],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/PKG-INFO` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.26.158
-Summary: Type annotations for boto3.MQ 1.26.158 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MQ 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.26.158](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,63 +339,63 @@
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
-    ResponseMetadataTypeDef,
+    CreateBrokerResponseTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
+    DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
-    PaginatorConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListBrokersRequestListBrokersPaginateTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
     PendingLogsTypeDef,
+    PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
+    PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
+    ListBrokersResponseTypeDef,
     ConfigurationsTypeDef,
     ConfigurationTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
-    CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
-    DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PromoteResponseTypeDef,
+    CreateBrokerRequestRequestTypeDef,
+    UpdateBrokerRequestRequestTypeDef,
     DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
```

### Comparing `mypy-boto3-mq-1.26.158/mypy_boto3_mq.egg-info/SOURCES.txt` & `mypy-boto3-mq-1.27.0/mypy_boto3_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.26.158/setup.py` & `mypy-boto3-mq-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mq",
-    version="1.26.158",
+    version="1.27.0",
     packages=["mypy_boto3_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MQ 1.26.158 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MQ 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


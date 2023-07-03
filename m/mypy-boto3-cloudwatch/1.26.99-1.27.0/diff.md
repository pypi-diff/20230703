# Comparing `tmp/mypy-boto3-cloudwatch-1.26.99.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.26.99.tar", last modified: Fri Mar 24 19:32:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.26.99.tar` & `mypy-boto3-cloudwatch-1.27.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19286 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42403 2023-03-24 19:32:02.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-03-24 19:32:02.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-03-24 19:32:01.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 19:32:25.000000 mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:32:25.573893 mypy-boto3-cloudwatch-1.26.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-24 19:32:00.000000 mypy-boto3-cloudwatch-1.26.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.522980 mypy-boto3-cloudwatch-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-03 19:50:31.518980 mypy-boto3-cloudwatch-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.518980 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-07-03 19:34:05.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-07-03 19:34:04.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.518980 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.522980 mypy-boto3-cloudwatch-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/LICENSE` & `mypy-boto3-cloudwatch-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/PKG-INFO` & `mypy-boto3-cloudwatch-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.26.99
-Summary: Type annotations for boto3.CloudWatch 1.26.99 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatch 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloudwatch"></a>
 
 # mypy-boto3-cloudwatch
 
 [![PyPI - mypy-boto3-cloudwatch](https://img.shields.io/pypi/v/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -456,75 +456,75 @@
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
-    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
+    GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamStatisticsMetricTypeDef,
+    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
+    PutMetricStreamOutputTypeDef,
+    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
-    GetDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
-    PutMetricStreamOutputTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/README.md` & `mypy-boto3-cloudwatch-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudwatch"></a>
 
 # mypy-boto3-cloudwatch
 
 [![PyPI - mypy-boto3-cloudwatch](https://img.shields.io/pypi/v/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -424,75 +424,75 @@
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
-    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
+    GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamStatisticsMetricTypeDef,
+    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
+    PutMetricStreamOutputTypeDef,
+    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
-    GetDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
-    PutMetricStreamOutputTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.26.99\nVersion:         1.26.99\nBuilder version:"
-        " 7.14.2\nDocs:           "
+        "Type annotations for boto3.CloudWatch 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.99")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
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
@@ -168,14 +169,15 @@
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
@@ -317,14 +319,15 @@
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
@@ -343,16 +346,19 @@
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
@@ -436,15 +442,17 @@
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

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -315,14 +317,15 @@
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
@@ -341,16 +344,19 @@
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
@@ -434,15 +440,17 @@
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

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: Union[datetime, str] = ...,
         EndDate: Union[datetime, str] = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 
@@ -117,15 +117,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAlarmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmspaginator)
         """
 
 
@@ -138,15 +138,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAnomalyDetectorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 
@@ -160,30 +160,30 @@
         self,
         *,
         MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, DashboardNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DashboardNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDashboardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
         """
 
 
@@ -198,13 +198,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMetricsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
         StartDate: Union[datetime, str] = ...,
         EndDate: Union[datetime, str] = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 class DescribeAlarmsPaginator(Paginator):
@@ -112,15 +112,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAlarmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmspaginator)
         """
 
 class DescribeAnomalyDetectorsPaginator(Paginator):
@@ -132,15 +132,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAnomalyDetectorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 class GetMetricDataPaginator(Paginator):
@@ -153,29 +153,29 @@
         self,
         *,
         MetricDataQueries: Sequence[MetricDataQueryTypeDef],
         StartTime: Union[datetime, str],
         EndTime: Union[datetime, str],
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 class ListDashboardsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, DashboardNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DashboardNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDashboardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listdashboardspaginator)
         """
 
 class ListMetricsPaginator(Paginator):
@@ -189,13 +189,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMetricsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,75 +48,75 @@
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
+    "GetDashboardOutputTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
     "MetricStreamFilterTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
+    "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
+    "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
+    "PutMetricStreamOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "DescribeAlarmHistoryOutputTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
     "MetricTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
     "DeleteInsightRulesOutputTypeDef",
-    "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
-    "GetDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
-    "GetMetricWidgetImageOutputTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
-    "PutMetricStreamOutputTypeDef",
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
@@ -271,25 +271,14 @@
         "ExceptionType": str,
         "FailureCode": str,
         "FailureDescription": str,
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
 DeleteMetricStreamInputRequestTypeDef = TypedDict(
     "DeleteMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -303,20 +292,24 @@
         "MaxRecords": int,
         "NextToken": str,
         "ScanBy": ScanByType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": Union[datetime, str],
+        "EndDate": Union[datetime, str],
+        "ScanBy": ScanByType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
     "DescribeAlarmHistoryInputRequestTypeDef",
     {
@@ -337,14 +330,29 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    {
+        "AlarmNames": Sequence[str],
+        "AlarmNamePrefix": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "ChildrenOfAlarmName": str,
+        "ParentsOfAlarmName": str,
+        "StateValue": StateValueType,
+        "ActionPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAlarmsInputRequestTypeDef = TypedDict(
     "DescribeAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "ChildrenOfAlarmName": str,
@@ -417,14 +425,21 @@
 DisableInsightRulesInputRequestTypeDef = TypedDict(
     "DisableInsightRulesInputRequestTypeDef",
     {
         "RuleNames": Sequence[str],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnableAlarmActionsInputRequestTypeDef = TypedDict(
     "EnableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
@@ -438,14 +453,24 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
+GetDashboardOutputTypeDef = TypedDict(
+    "GetDashboardOutputTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardBody": str,
+        "DashboardName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
     "_RequiredGetInsightRuleReportInputRequestTypeDef",
     {
         "RuleName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Period": int,
@@ -520,14 +545,15 @@
     },
 )
 
 MetricStreamFilterTypeDef = TypedDict(
     "MetricStreamFilterTypeDef",
     {
         "Namespace": str,
+        "MetricNames": List[str],
     },
     total=False,
 )
 
 _RequiredGetMetricWidgetImageInputRequestTypeDef = TypedDict(
     "_RequiredGetMetricWidgetImageInputRequestTypeDef",
     {
@@ -546,22 +572,39 @@
 class GetMetricWidgetImageInputRequestTypeDef(
     _RequiredGetMetricWidgetImageInputRequestTypeDef,
     _OptionalGetMetricWidgetImageInputRequestTypeDef,
 ):
     pass
 
 
+GetMetricWidgetImageOutputTypeDef = TypedDict(
+    "GetMetricWidgetImageOutputTypeDef",
+    {
+        "MetricWidgetImage": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InsightRuleContributorDatapointTypeDef = TypedDict(
     "InsightRuleContributorDatapointTypeDef",
     {
         "Timestamp": datetime,
         "ApproximateValue": float,
     },
 )
 
+ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
+    {
+        "DashboardNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDashboardsInputRequestTypeDef = TypedDict(
     "ListDashboardsInputRequestTypeDef",
     {
         "DashboardNamePrefix": str,
         "NextToken": str,
     },
     total=False,
@@ -650,22 +693,51 @@
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
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
 PutDashboardInputRequestTypeDef = TypedDict(
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
+PutMetricStreamOutputTypeDef = TypedDict(
+    "PutMetricStreamOutputTypeDef",
+    {
+        "Arn": str,
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
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
@@ -725,14 +797,23 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeAlarmHistoryOutputTypeDef = TypedDict(
+    "DescribeAlarmHistoryOutputTypeDef",
+    {
+        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AnomalyDetectorConfigurationTypeDef = TypedDict(
     "AnomalyDetectorConfigurationTypeDef",
     {
         "ExcludedTimeRanges": List[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
@@ -761,14 +842,26 @@
 class DescribeAlarmsForMetricInputRequestTypeDef(
     _RequiredDescribeAlarmsForMetricInputRequestTypeDef,
     _OptionalDescribeAlarmsForMetricInputRequestTypeDef,
 ):
     pass
 
 
+DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
@@ -850,162 +943,70 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
     },
     total=False,
 )
 
-DeleteInsightRulesOutputTypeDef = TypedDict(
-    "DeleteInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAlarmHistoryOutputTypeDef = TypedDict(
-    "DescribeAlarmHistoryOutputTypeDef",
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
     {
-        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "DashboardEntries": List[DashboardEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableInsightRulesOutputTypeDef = TypedDict(
-    "DisableInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
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
-EnableInsightRulesOutputTypeDef = TypedDict(
-    "EnableInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDashboardOutputTypeDef = TypedDict(
-    "GetDashboardOutputTypeDef",
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
     {
-        "DashboardArn": str,
-        "DashboardBody": str,
-        "DashboardName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMetricStatisticsOutputTypeDef = TypedDict(
     "GetMetricStatisticsOutputTypeDef",
     {
         "Label": str,
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetMetricWidgetImageOutputTypeDef = TypedDict(
-    "GetMetricWidgetImageOutputTypeDef",
+DeleteInsightRulesOutputTypeDef = TypedDict(
+    "DeleteInsightRulesOutputTypeDef",
     {
-        "MetricWidgetImage": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
+DisableInsightRulesOutputTypeDef = TypedDict(
+    "DisableInsightRulesOutputTypeDef",
     {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
+EnableInsightRulesOutputTypeDef = TypedDict(
+    "EnableInsightRulesOutputTypeDef",
     {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedInsightRulesOutputTypeDef = TypedDict(
     "PutManagedInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutMetricStreamOutputTypeDef = TypedDict(
-    "PutMetricStreamOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
-    {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "ScanBy": ScanByType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    {
-        "AlarmNames": Sequence[str],
-        "AlarmNamePrefix": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "ChildrenOfAlarmName": str,
-        "ParentsOfAlarmName": str,
-        "StateValue": StateValueType,
-        "ActionPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
-    {
-        "DashboardNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 DescribeAlarmsInputAlarmExistsWaitTypeDef = TypedDict(
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
@@ -1039,28 +1040,28 @@
 )
 
 DescribeInsightRulesOutputTypeDef = TypedDict(
     "DescribeInsightRulesOutputTypeDef",
     {
         "NextToken": str,
         "InsightRules": List[InsightRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMetricsInputListMetricsPaginateTypeDef = TypedDict(
     "ListMetricsInputListMetricsPaginateTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionFilterTypeDef],
         "RecentlyActive": Literal["PT3H"],
         "IncludeLinkedAccounts": bool,
         "OwningAccount": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMetricsInputRequestTypeDef = TypedDict(
     "ListMetricsInputRequestTypeDef",
     {
@@ -1098,23 +1099,23 @@
 )
 
 ListMetricStreamsOutputTypeDef = TypedDict(
     "ListMetricStreamsOutputTypeDef",
     {
         "NextToken": str,
         "Entries": List[MetricStreamEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
@@ -1241,15 +1242,15 @@
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
         "Metrics": List[MetricTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
@@ -1272,28 +1273,28 @@
 
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightRuleReportOutputTypeDef = TypedDict(
     "GetInsightRuleReportOutputTypeDef",
     {
         "KeyLabels": List[str],
         "AggregationStatistic": str,
         "AggregateValue": float,
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedInsightRulesInputRequestTypeDef = TypedDict(
     "PutManagedInsightRulesInputRequestTypeDef",
     {
         "ManagedRules": Sequence[ManagedRuleTypeDef],
@@ -1301,15 +1302,15 @@
 )
 
 ListManagedInsightRulesOutputTypeDef = TypedDict(
     "ListManagedInsightRulesOutputTypeDef",
     {
         "ManagedRules": List[ManagedRuleDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
@@ -1328,15 +1329,15 @@
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
         "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricStreamInputRequestTypeDef",
     {
         "Name": str,
@@ -1397,15 +1398,15 @@
     },
 )
 _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
     "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
         "ScanBy": ScanByType,
         "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetMetricDataInputGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
@@ -1565,25 +1566,25 @@
     pass
 
 
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
         "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAlarmsOutputTypeDef = TypedDict(
     "DescribeAlarmsOutputTypeDef",
     {
         "CompositeAlarms": List[CompositeAlarmTypeDef],
         "MetricAlarms": List[MetricAlarmTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnomalyDetectorTypeDef = TypedDict(
     "AnomalyDetectorTypeDef",
     {
         "Namespace": str,
@@ -1626,10 +1627,10 @@
 )
 
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,75 +47,75 @@
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
-    "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
     "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmHistoryInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
+    "GetDashboardOutputTypeDef",
     "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
     "MetricStreamFilterTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
+    "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
+    "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
+    "PutMetricStreamOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "DescribeAlarmHistoryOutputTypeDef",
     "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
     "GetMetricStatisticsInputRequestTypeDef",
     "MetricTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
     "DeleteInsightRulesOutputTypeDef",
-    "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
-    "GetDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
-    "GetMetricWidgetImageOutputTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
-    "PutMetricStreamOutputTypeDef",
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
@@ -270,25 +270,14 @@
         "ExceptionType": str,
         "FailureCode": str,
         "FailureDescription": str,
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
 DeleteMetricStreamInputRequestTypeDef = TypedDict(
     "DeleteMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -302,20 +291,24 @@
         "MaxRecords": int,
         "NextToken": str,
         "ScanBy": ScanByType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": Union[datetime, str],
+        "EndDate": Union[datetime, str],
+        "ScanBy": ScanByType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
     "DescribeAlarmHistoryInputRequestTypeDef",
     {
@@ -336,14 +329,29 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    {
+        "AlarmNames": Sequence[str],
+        "AlarmNamePrefix": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "ChildrenOfAlarmName": str,
+        "ParentsOfAlarmName": str,
+        "StateValue": StateValueType,
+        "ActionPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAlarmsInputRequestTypeDef = TypedDict(
     "DescribeAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "ChildrenOfAlarmName": str,
@@ -412,14 +420,21 @@
 DisableInsightRulesInputRequestTypeDef = TypedDict(
     "DisableInsightRulesInputRequestTypeDef",
     {
         "RuleNames": Sequence[str],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnableAlarmActionsInputRequestTypeDef = TypedDict(
     "EnableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
@@ -433,14 +448,24 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
+GetDashboardOutputTypeDef = TypedDict(
+    "GetDashboardOutputTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardBody": str,
+        "DashboardName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
     "_RequiredGetInsightRuleReportInputRequestTypeDef",
     {
         "RuleName": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "Period": int,
@@ -511,14 +536,15 @@
     },
 )
 
 MetricStreamFilterTypeDef = TypedDict(
     "MetricStreamFilterTypeDef",
     {
         "Namespace": str,
+        "MetricNames": List[str],
     },
     total=False,
 )
 
 _RequiredGetMetricWidgetImageInputRequestTypeDef = TypedDict(
     "_RequiredGetMetricWidgetImageInputRequestTypeDef",
     {
@@ -535,22 +561,39 @@
 
 class GetMetricWidgetImageInputRequestTypeDef(
     _RequiredGetMetricWidgetImageInputRequestTypeDef,
     _OptionalGetMetricWidgetImageInputRequestTypeDef,
 ):
     pass
 
+GetMetricWidgetImageOutputTypeDef = TypedDict(
+    "GetMetricWidgetImageOutputTypeDef",
+    {
+        "MetricWidgetImage": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InsightRuleContributorDatapointTypeDef = TypedDict(
     "InsightRuleContributorDatapointTypeDef",
     {
         "Timestamp": datetime,
         "ApproximateValue": float,
     },
 )
 
+ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
+    {
+        "DashboardNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDashboardsInputRequestTypeDef = TypedDict(
     "ListDashboardsInputRequestTypeDef",
     {
         "DashboardNamePrefix": str,
         "NextToken": str,
     },
     total=False,
@@ -637,22 +680,51 @@
     "MetricStreamStatisticsMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
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
 PutDashboardInputRequestTypeDef = TypedDict(
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
+PutMetricStreamOutputTypeDef = TypedDict(
+    "PutMetricStreamOutputTypeDef",
+    {
+        "Arn": str,
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
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
@@ -708,14 +780,23 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeAlarmHistoryOutputTypeDef = TypedDict(
+    "DescribeAlarmHistoryOutputTypeDef",
+    {
+        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AnomalyDetectorConfigurationTypeDef = TypedDict(
     "AnomalyDetectorConfigurationTypeDef",
     {
         "ExcludedTimeRanges": List[RangeTypeDef],
         "MetricTimezone": str,
     },
     total=False,
@@ -742,14 +823,26 @@
 
 class DescribeAlarmsForMetricInputRequestTypeDef(
     _RequiredDescribeAlarmsForMetricInputRequestTypeDef,
     _OptionalDescribeAlarmsForMetricInputRequestTypeDef,
 ):
     pass
 
+DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
     "DescribeAnomalyDetectorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
@@ -827,162 +920,70 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
     },
     total=False,
 )
 
-DeleteInsightRulesOutputTypeDef = TypedDict(
-    "DeleteInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAlarmHistoryOutputTypeDef = TypedDict(
-    "DescribeAlarmHistoryOutputTypeDef",
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
     {
-        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "DashboardEntries": List[DashboardEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableInsightRulesOutputTypeDef = TypedDict(
-    "DisableInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
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
-EnableInsightRulesOutputTypeDef = TypedDict(
-    "EnableInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDashboardOutputTypeDef = TypedDict(
-    "GetDashboardOutputTypeDef",
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
     {
-        "DashboardArn": str,
-        "DashboardBody": str,
-        "DashboardName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMetricStatisticsOutputTypeDef = TypedDict(
     "GetMetricStatisticsOutputTypeDef",
     {
         "Label": str,
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetMetricWidgetImageOutputTypeDef = TypedDict(
-    "GetMetricWidgetImageOutputTypeDef",
+DeleteInsightRulesOutputTypeDef = TypedDict(
+    "DeleteInsightRulesOutputTypeDef",
     {
-        "MetricWidgetImage": bytes,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
+DisableInsightRulesOutputTypeDef = TypedDict(
+    "DisableInsightRulesOutputTypeDef",
     {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
+EnableInsightRulesOutputTypeDef = TypedDict(
+    "EnableInsightRulesOutputTypeDef",
     {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedInsightRulesOutputTypeDef = TypedDict(
     "PutManagedInsightRulesOutputTypeDef",
     {
         "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutMetricStreamOutputTypeDef = TypedDict(
-    "PutMetricStreamOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
-    {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "ScanBy": ScanByType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    {
-        "AlarmNames": Sequence[str],
-        "AlarmNamePrefix": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "ChildrenOfAlarmName": str,
-        "ParentsOfAlarmName": str,
-        "StateValue": StateValueType,
-        "ActionPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
-    {
-        "DashboardNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 DescribeAlarmsInputAlarmExistsWaitTypeDef = TypedDict(
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
@@ -1016,28 +1017,28 @@
 )
 
 DescribeInsightRulesOutputTypeDef = TypedDict(
     "DescribeInsightRulesOutputTypeDef",
     {
         "NextToken": str,
         "InsightRules": List[InsightRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMetricsInputListMetricsPaginateTypeDef = TypedDict(
     "ListMetricsInputListMetricsPaginateTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionFilterTypeDef],
         "RecentlyActive": Literal["PT3H"],
         "IncludeLinkedAccounts": bool,
         "OwningAccount": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMetricsInputRequestTypeDef = TypedDict(
     "ListMetricsInputRequestTypeDef",
     {
@@ -1075,23 +1076,23 @@
 )
 
 ListMetricStreamsOutputTypeDef = TypedDict(
     "ListMetricStreamsOutputTypeDef",
     {
         "NextToken": str,
         "Entries": List[MetricStreamEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
@@ -1210,15 +1211,15 @@
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
         "Metrics": List[MetricTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
@@ -1239,28 +1240,28 @@
 
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInsightRuleReportOutputTypeDef = TypedDict(
     "GetInsightRuleReportOutputTypeDef",
     {
         "KeyLabels": List[str],
         "AggregationStatistic": str,
         "AggregateValue": float,
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutManagedInsightRulesInputRequestTypeDef = TypedDict(
     "PutManagedInsightRulesInputRequestTypeDef",
     {
         "ManagedRules": Sequence[ManagedRuleTypeDef],
@@ -1268,15 +1269,15 @@
 )
 
 ListManagedInsightRulesOutputTypeDef = TypedDict(
     "ListManagedInsightRulesOutputTypeDef",
     {
         "ManagedRules": List[ManagedRuleDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
@@ -1295,15 +1296,15 @@
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
         "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricStreamInputRequestTypeDef",
     {
         "Name": str,
@@ -1360,15 +1361,15 @@
     },
 )
 _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
     "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
     {
         "ScanBy": ScanByType,
         "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetMetricDataInputGetMetricDataPaginateTypeDef(
     _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
     _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
@@ -1520,25 +1521,25 @@
 ):
     pass
 
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
         "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAlarmsOutputTypeDef = TypedDict(
     "DescribeAlarmsOutputTypeDef",
     {
         "CompositeAlarms": List[CompositeAlarmTypeDef],
         "MetricAlarms": List[MetricAlarmTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnomalyDetectorTypeDef = TypedDict(
     "AnomalyDetectorTypeDef",
     {
         "Namespace": str,
@@ -1581,10 +1582,10 @@
 )
 
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.26.99
-Summary: Type annotations for boto3.CloudWatch 1.26.99 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatch 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloudwatch"></a>
 
 # mypy-boto3-cloudwatch
 
 [![PyPI - mypy-boto3-cloudwatch](https://img.shields.io/pypi/v/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -456,75 +456,75 @@
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
-    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
     DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
+    GetDashboardOutputTypeDef,
     GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
     MetricStreamStatisticsMetricTypeDef,
+    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
+    PutMetricStreamOutputTypeDef,
+    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
     GetMetricStatisticsInputMetricGetStatisticsTypeDef,
     GetMetricStatisticsInputRequestTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
-    GetDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
-    PutMetricStreamOutputTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
```

### Comparing `mypy-boto3-cloudwatch-1.26.99/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.26.99/setup.py` & `mypy-boto3-cloudwatch-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.26.99",
+    version="1.27.0",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatch 1.26.99 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.CloudWatch 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


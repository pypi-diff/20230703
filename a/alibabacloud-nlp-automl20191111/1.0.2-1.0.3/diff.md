# Comparing `tmp/alibabacloud_nlp-automl20191111-1.0.2.tar.gz` & `tmp/alibabacloud_nlp-automl20191111-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_nlp-automl20191111-1.0.2.tar", last modified: Tue Jan 31 09:44:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud_nlp-automl20191111-1.0.3.tar", last modified: Mon Jul  3 03:30:48 2023, max compression
```

## Comparing `alibabacloud_nlp-automl20191111-1.0.2.tar` & `alibabacloud_nlp-automl20191111-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      171 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15458 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111/client.py
--rw-r--r--   0 root         (0) root         (0)    16269 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2647 2023-01-31 09:44:00.000000 alibabacloud_nlp-automl20191111-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22280 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111/client.py
+-rw-r--r--   0 root         (0) root         (0)    26423 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-03 03:30:48.000000 alibabacloud_nlp-automl20191111-1.0.3/setup.py
```

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/LICENSE` & `alibabacloud_nlp-automl20191111-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/PKG-INFO` & `alibabacloud_nlp-automl20191111-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_nlp-automl20191111
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud nlp-automl (20191111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/README-CN.md` & `alibabacloud_nlp-automl20191111-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/README.md` & `alibabacloud_nlp-automl20191111-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111/client.py` & `alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -147,14 +147,100 @@
     async def create_async_predict_async(
         self,
         request: nlp_automl_20191111_models.CreateAsyncPredictRequest,
     ) -> nlp_automl_20191111_models.CreateAsyncPredictResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_async_predict_with_options_async(request, runtime)
 
+    def find_user_report_4alinlp_with_options(
+        self,
+        request: nlp_automl_20191111_models.FindUserReport4AlinlpRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlp_automl_20191111_models.FindUserReport4AlinlpResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.begin_time):
+            body['BeginTime'] = request.begin_time
+        if not UtilClient.is_unset(request.customer_user_parent_id):
+            body['CustomerUserParentId'] = request.customer_user_parent_id
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.model_type):
+            body['ModelType'] = request.model_type
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='FindUserReport4Alinlp',
+            version='2019-11-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlp_automl_20191111_models.FindUserReport4AlinlpResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def find_user_report_4alinlp_with_options_async(
+        self,
+        request: nlp_automl_20191111_models.FindUserReport4AlinlpRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlp_automl_20191111_models.FindUserReport4AlinlpResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.begin_time):
+            body['BeginTime'] = request.begin_time
+        if not UtilClient.is_unset(request.customer_user_parent_id):
+            body['CustomerUserParentId'] = request.customer_user_parent_id
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.model_type):
+            body['ModelType'] = request.model_type
+        if not UtilClient.is_unset(request.type):
+            body['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='FindUserReport4Alinlp',
+            version='2019-11-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlp_automl_20191111_models.FindUserReport4AlinlpResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def find_user_report_4alinlp(
+        self,
+        request: nlp_automl_20191111_models.FindUserReport4AlinlpRequest,
+    ) -> nlp_automl_20191111_models.FindUserReport4AlinlpResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.find_user_report_4alinlp_with_options(request, runtime)
+
+    async def find_user_report_4alinlp_async(
+        self,
+        request: nlp_automl_20191111_models.FindUserReport4AlinlpRequest,
+    ) -> nlp_automl_20191111_models.FindUserReport4AlinlpResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.find_user_report_4alinlp_with_options_async(request, runtime)
+
     def get_async_predict_with_options(
         self,
         request: nlp_automl_20191111_models.GetAsyncPredictRequest,
         runtime: util_models.RuntimeOptions,
     ) -> nlp_automl_20191111_models.GetAsyncPredictResponse:
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -376,7 +462,85 @@
 
     async def run_pre_train_service_async(
         self,
         request: nlp_automl_20191111_models.RunPreTrainServiceRequest,
     ) -> nlp_automl_20191111_models.RunPreTrainServiceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.run_pre_train_service_with_options_async(request, runtime)
+
+    def run_pre_train_service_new_with_options(
+        self,
+        request: nlp_automl_20191111_models.RunPreTrainServiceNewRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlp_automl_20191111_models.RunPreTrainServiceNewResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.predict_content):
+            body['PredictContent'] = request.predict_content
+        if not UtilClient.is_unset(request.service_name):
+            body['ServiceName'] = request.service_name
+        if not UtilClient.is_unset(request.service_version):
+            body['ServiceVersion'] = request.service_version
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RunPreTrainServiceNew',
+            version='2019-11-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlp_automl_20191111_models.RunPreTrainServiceNewResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def run_pre_train_service_new_with_options_async(
+        self,
+        request: nlp_automl_20191111_models.RunPreTrainServiceNewRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlp_automl_20191111_models.RunPreTrainServiceNewResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.predict_content):
+            body['PredictContent'] = request.predict_content
+        if not UtilClient.is_unset(request.service_name):
+            body['ServiceName'] = request.service_name
+        if not UtilClient.is_unset(request.service_version):
+            body['ServiceVersion'] = request.service_version
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RunPreTrainServiceNew',
+            version='2019-11-11',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlp_automl_20191111_models.RunPreTrainServiceNewResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def run_pre_train_service_new(
+        self,
+        request: nlp_automl_20191111_models.RunPreTrainServiceNewRequest,
+    ) -> nlp_automl_20191111_models.RunPreTrainServiceNewResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.run_pre_train_service_new_with_options(request, runtime)
+
+    async def run_pre_train_service_new_async(
+        self,
+        request: nlp_automl_20191111_models.RunPreTrainServiceNewRequest,
+    ) -> nlp_automl_20191111_models.RunPreTrainServiceNewResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.run_pre_train_service_new_with_options_async(request, runtime)
```

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111/models.py` & `alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict
+from typing import Dict, List
 
 
 class CreateAsyncPredictRequest(TeaModel):
     def __init__(
         self,
         content: str = None,
         detail_tag: str = None,
@@ -164,14 +164,207 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAsyncPredictResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class FindUserReport4AlinlpRequest(TeaModel):
+    def __init__(
+        self,
+        begin_time: str = None,
+        customer_user_parent_id: int = None,
+        end_time: str = None,
+        model_type: str = None,
+        type: str = None,
+    ):
+        self.begin_time = begin_time
+        self.customer_user_parent_id = customer_user_parent_id
+        self.end_time = end_time
+        self.model_type = model_type
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.begin_time is not None:
+            result['BeginTime'] = self.begin_time
+        if self.customer_user_parent_id is not None:
+            result['CustomerUserParentId'] = self.customer_user_parent_id
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.model_type is not None:
+            result['ModelType'] = self.model_type
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BeginTime') is not None:
+            self.begin_time = m.get('BeginTime')
+        if m.get('CustomerUserParentId') is not None:
+            self.customer_user_parent_id = m.get('CustomerUserParentId')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('ModelType') is not None:
+            self.model_type = m.get('ModelType')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class FindUserReport4AlinlpResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        fail_count: int = None,
+        qps_max: int = None,
+        rpt_time: str = None,
+        success_count: int = None,
+        total_count: int = None,
+    ):
+        self.fail_count = fail_count
+        self.qps_max = qps_max
+        self.rpt_time = rpt_time
+        self.success_count = success_count
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fail_count is not None:
+            result['FailCount'] = self.fail_count
+        if self.qps_max is not None:
+            result['QpsMax'] = self.qps_max
+        if self.rpt_time is not None:
+            result['RptTime'] = self.rpt_time
+        if self.success_count is not None:
+            result['SuccessCount'] = self.success_count
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FailCount') is not None:
+            self.fail_count = m.get('FailCount')
+        if m.get('QpsMax') is not None:
+            self.qps_max = m.get('QpsMax')
+        if m.get('RptTime') is not None:
+            self.rpt_time = m.get('RptTime')
+        if m.get('SuccessCount') is not None:
+            self.success_count = m.get('SuccessCount')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class FindUserReport4AlinlpResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: List[FindUserReport4AlinlpResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = FindUserReport4AlinlpResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class FindUserReport4AlinlpResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: FindUserReport4AlinlpResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = FindUserReport4AlinlpResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAsyncPredictRequest(TeaModel):
     def __init__(
         self,
         async_predict_id: int = None,
     ):
         self.async_predict_id = async_predict_id
 
@@ -450,37 +643,43 @@
             self.service_version = m.get('ServiceVersion')
         return self
 
 
 class RunPreTrainServiceResponseBody(TeaModel):
     def __init__(
         self,
+        billing_count: int = None,
         predict_result: str = None,
         request_id: str = None,
     ):
+        self.billing_count = billing_count
         self.predict_result = predict_result
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.billing_count is not None:
+            result['BillingCount'] = self.billing_count
         if self.predict_result is not None:
             result['PredictResult'] = self.predict_result
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('BillingCount') is not None:
+            self.billing_count = m.get('BillingCount')
         if m.get('PredictResult') is not None:
             self.predict_result = m.get('PredictResult')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
@@ -524,7 +723,129 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RunPreTrainServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RunPreTrainServiceNewRequest(TeaModel):
+    def __init__(
+        self,
+        predict_content: str = None,
+        service_name: str = None,
+        service_version: str = None,
+    ):
+        self.predict_content = predict_content
+        self.service_name = service_name
+        self.service_version = service_version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.predict_content is not None:
+            result['PredictContent'] = self.predict_content
+        if self.service_name is not None:
+            result['ServiceName'] = self.service_name
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PredictContent') is not None:
+            self.predict_content = m.get('PredictContent')
+        if m.get('ServiceName') is not None:
+            self.service_name = m.get('ServiceName')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        return self
+
+
+class RunPreTrainServiceNewResponseBody(TeaModel):
+    def __init__(
+        self,
+        billing_count: int = None,
+        predict_result: str = None,
+        request_id: str = None,
+    ):
+        self.billing_count = billing_count
+        self.predict_result = predict_result
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.billing_count is not None:
+            result['BillingCount'] = self.billing_count
+        if self.predict_result is not None:
+            result['PredictResult'] = self.predict_result
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BillingCount') is not None:
+            self.billing_count = m.get('BillingCount')
+        if m.get('PredictResult') is not None:
+            self.predict_result = m.get('PredictResult')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RunPreTrainServiceNewResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RunPreTrainServiceNewResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RunPreTrainServiceNewResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/alibabacloud_nlp_automl20191111.egg-info/PKG-INFO` & `alibabacloud_nlp-automl20191111-1.0.3/alibabacloud_nlp_automl20191111.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-nlp-automl20191111
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud nlp-automl (20191111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nlp-automl20191111-1.0.2/setup.py` & `alibabacloud_nlp-automl20191111-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_nlp-automl20191111.
 
-Created on 31/01/2023
+Created on 03/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_nlp_automl20191111"
 NAME = "alibabacloud_nlp-automl20191111" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud nlp-automl (20191111) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```


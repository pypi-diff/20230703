# Comparing `tmp/alibabacloud_nlp-automl20191111_py2-1.0.1.tar.gz` & `tmp/alibabacloud_nlp-automl20191111_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_nlp-automl20191111_py2-1.0.1.tar", last modified: Tue Jan 31 09:43:12 2023, max compression
+gzip compressed data, was "dist/alibabacloud_nlp-automl20191111_py2-1.0.2.tar", last modified: Mon Jul  3 03:30:01 2023, max compression
```

## Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1.tar` & `alibabacloud_nlp-automl20191111_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       74 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7081 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111/client.py
--rw-r--r--   0 root         (0) root         (0)    16284 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2023-01-31 09:43:12.000000 alibabacloud_nlp-automl20191111_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9812 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111/client.py
+-rw-r--r--   0 root         (0) root         (0)    26482 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-07-03 03:30:01.000000 alibabacloud_nlp-automl20191111_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/LICENSE` & `alibabacloud_nlp-automl20191111_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/PKG-INFO` & `alibabacloud_nlp-automl20191111_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_nlp-automl20191111_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud nlp-automl (20191111) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/README-CN.md` & `alibabacloud_nlp-automl20191111_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/README.md` & `alibabacloud_nlp-automl20191111_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111/client.py` & `alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,14 +74,50 @@
             self.call_api(params, req, runtime)
         )
 
     def create_async_predict(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_async_predict_with_options(request, runtime)
 
+    def find_user_report_4alinlp_with_options(self, request, runtime):
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
+    def find_user_report_4alinlp(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.find_user_report_4alinlp_with_options(request, runtime)
+
     def get_async_predict_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -167,7 +203,39 @@
             nlp_automl_20191111_models.RunPreTrainServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def run_pre_train_service(self, request):
         runtime = util_models.RuntimeOptions()
         return self.run_pre_train_service_with_options(request, runtime)
+
+    def run_pre_train_service_new_with_options(self, request, runtime):
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
+    def run_pre_train_service_new(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.run_pre_train_service_new_with_options(request, runtime)
```

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111/models.py` & `alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -142,14 +142,183 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAsyncPredictResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class FindUserReport4AlinlpRequest(TeaModel):
+    def __init__(self, begin_time=None, customer_user_parent_id=None, end_time=None, model_type=None, type=None):
+        self.begin_time = begin_time  # type: str
+        self.customer_user_parent_id = customer_user_parent_id  # type: long
+        self.end_time = end_time  # type: str
+        self.model_type = model_type  # type: str
+        self.type = type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(FindUserReport4AlinlpRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, fail_count=None, qps_max=None, rpt_time=None, success_count=None, total_count=None):
+        self.fail_count = fail_count  # type: long
+        self.qps_max = qps_max  # type: int
+        self.rpt_time = rpt_time  # type: str
+        self.success_count = success_count  # type: long
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(FindUserReport4AlinlpResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, data=None, request_id=None):
+        self.code = code  # type: str
+        self.data = data  # type: list[FindUserReport4AlinlpResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(FindUserReport4AlinlpResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: FindUserReport4AlinlpResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(FindUserReport4AlinlpResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, async_predict_id=None):
         self.async_predict_id = async_predict_id  # type: int
 
     def validate(self):
         pass
 
@@ -391,35 +560,40 @@
             self.service_name = m.get('ServiceName')
         if m.get('ServiceVersion') is not None:
             self.service_version = m.get('ServiceVersion')
         return self
 
 
 class RunPreTrainServiceResponseBody(TeaModel):
-    def __init__(self, predict_result=None, request_id=None):
+    def __init__(self, billing_count=None, predict_result=None, request_id=None):
+        self.billing_count = billing_count  # type: int
         self.predict_result = predict_result  # type: str
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RunPreTrainServiceResponseBody, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('BillingCount') is not None:
+            self.billing_count = m.get('BillingCount')
         if m.get('PredictResult') is not None:
             self.predict_result = m.get('PredictResult')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
@@ -458,7 +632,114 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RunPreTrainServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RunPreTrainServiceNewRequest(TeaModel):
+    def __init__(self, predict_content=None, service_name=None, service_version=None):
+        self.predict_content = predict_content  # type: str
+        self.service_name = service_name  # type: str
+        self.service_version = service_version  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RunPreTrainServiceNewRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, billing_count=None, predict_result=None, request_id=None):
+        self.billing_count = billing_count  # type: int
+        self.predict_result = predict_result  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RunPreTrainServiceNewResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RunPreTrainServiceNewResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RunPreTrainServiceNewResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/alibabacloud_nlp_automl20191111_py2.egg-info/PKG-INFO` & `alibabacloud_nlp-automl20191111_py2-1.0.2/alibabacloud_nlp_automl20191111_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-nlp-automl20191111-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud nlp-automl (20191111) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nlp-automl20191111_py2-1.0.1/setup.py` & `alibabacloud_nlp-automl20191111_py2-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_nlp-automl20191111_py2.
 
-Created on 31/01/2023
+Created on 03/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_nlp_automl20191111"
 NAME = "alibabacloud_nlp-automl20191111_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud nlp-automl (20191111) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```


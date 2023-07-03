# Comparing `tmp/tencentcloud-sdk-python-common-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-common-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.925.tar", last modified: Fri Jun 30 02:04:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.926.tar", last modified: Mon Jul  3 00:23:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-common-3.0.925.tar` & `tencentcloud-sdk-python-common-3.0.926.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15666 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/request.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/common_client.py
--rw-r--r--   0 root         (0) root         (0)    18594 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/sign.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      837 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      876 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/sign.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/common_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20283 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/abstract_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/circuit_breaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)     5120 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/http/request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15666 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/credential.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:23:13.000000 tencentcloud-sdk-python-common-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.925'
+__version__ = '3.0.926'
```

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/credential.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/request.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/http/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,50 +52,55 @@
                                 verify=self.certification,
                                 timeout=self.timeout)
 
 
 class ApiRequest(object):
     def __init__(self, host, req_timeout=60, debug=False, proxy=None, is_http=False, certification=None):
         self.conn = ProxyConnection(host, timeout=req_timeout, proxy=proxy, certification=certification, is_http=is_http)
-        url = urlparse(host)
-        if not url.hostname:
-            if is_http:
-                host = "http://" + host
-            else:
-                host = "https://" + host
+        self.is_http = is_http
         self.host = host
         self.req_timeout = req_timeout
         self.keep_alive = False
         self.debug = debug
         self.request_size = 0
         self.response_size = 0
 
+    def _handle_host(self, host):
+        url = urlparse(host)
+        if not url.hostname:
+            if self.is_http:
+                return "http://" + host
+            else:
+                return "https://" + host
+        return host
+
     def set_req_timeout(self, req_timeout):
         self.req_timeout = req_timeout
 
     def is_keep_alive(self):
         return self.keep_alive
 
     def set_keep_alive(self, flag=True):
         self.keep_alive = flag
 
     def set_debug(self, debug):
         self.debug = debug
 
     def _request(self, req_inter):
+        url = self._handle_host(req_inter.host)
         if self.keep_alive:
             req_inter.header["Connection"] = "Keep-Alive"
         if self.debug:
             logger.debug("SendRequest %s" % req_inter)
         if req_inter.method == 'GET':
-            req_inter_url = '%s?%s' % (self.host, req_inter.data)
+            req_inter_url = '%s?%s' % (url, req_inter.data)
             return self.conn.request(req_inter.method, req_inter_url,
                               None, req_inter.header)
         elif req_inter.method == 'POST':
-            return self.conn.request(req_inter.method, self.host,
+            return self.conn.request(req_inter.method, url,
                               req_inter.data, req_inter.header)
         else:
             raise TencentCloudSDKException(
                 "ClientParamsError", 'Method only support (GET, POST)')
 
     def send_request(self, req_inter):
         try:
```

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_model.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/__init__.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/http_profile.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/common_client.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_client.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/abstract_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,16 +32,17 @@
     from urllib import urlencode
 
 import tencentcloud
 from tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tencentcloud.common.exception import TencentCloudSDKException as SDKError
 from tencentcloud.common.http.request import ApiRequest
 from tencentcloud.common.http.request import RequestInternal
-from tencentcloud.common.profile.client_profile import ClientProfile
+from tencentcloud.common.profile.client_profile import ClientProfile, RegionBreakerProfile
 from tencentcloud.common.sign import Sign
+from tencentcloud.common.circuit_breaker import CircuitBreaker
 
 warnings.filterwarnings("ignore", module="tencentcloud", category=UserWarning)
 
 _json_content = 'application/json'
 _multipart_content = 'multipart/form-data'
 _form_urlencoded_content = 'application/x-www-form-urlencoded'
 _octet_stream = "application/octet-stream"
@@ -75,14 +76,19 @@
         self.request = ApiRequest(self._get_endpoint(),
                                   req_timeout=self.profile.httpProfile.reqTimeout,
                                   proxy=self.profile.httpProfile.proxy,
                                   is_http=is_http,
                                   certification=self.profile.httpProfile.certification)
         if self.profile.httpProfile.keepAlive:
             self.request.set_keep_alive()
+        self.circuit_breaker = None
+        if not self.profile.disable_region_breaker:
+            if self.profile.region_breaker_profile is None:
+                self.profile.region_breaker_profile = RegionBreakerProfile()
+            self.circuit_breaker = CircuitBreaker(self.profile.region_breaker_profile)
 
     def _fix_params(self, params):
         if not isinstance(params, (dict,)):
             return params
         return self._format_params(None, params)
 
     def _format_params(self, prefix, params):
@@ -348,26 +354,53 @@
         if "DeprecatedWarning" in resp["Response"]:
             import warnings
             warnings.filterwarnings("default")
             warnings.warn("This action is deprecated, detail: %s" % resp["Response"]["DeprecatedWarning"],
                           DeprecationWarning)
 
     def call(self, action, params, options=None, headers=None):
+        if not self.profile.disable_region_breaker:
+            return self.call_with_region_breaker(action, params, options, headers)
         req = RequestInternal(self._get_endpoint(),
                               self.profile.httpProfile.reqMethod,
                               self._requestPath,
                               header=headers)
         self._build_req_inter(action, params, req, options)
 
         resp_inter = self.request.send_request(req)
         self._check_status(resp_inter)
         data = resp_inter.data
         self._handle_response(data)
         return data
 
+    def call_with_region_breaker(self, action, params, options=None, headers=None):
+        endpoint = self._get_endpoint()
+        generation, need_break = self.circuit_breaker.before_requests()
+        if need_break:
+            endpoint = self._service + "." + self.profile.region_breaker_profile.backup_endpoint
+        req = RequestInternal(endpoint,
+                              self.profile.httpProfile.reqMethod,
+                              self._requestPath,
+                              header=headers)
+        self._build_req_inter(action, params, req, options)
+        data = '{"Response": {}}'
+        try:
+            resp_inter = self.request.send_request(req)
+            self._check_status(resp_inter)
+            data = resp_inter.data
+            self._handle_response(data)
+            self.circuit_breaker.after_requests(generation, True)
+        except TencentCloudSDKException as e:
+            if "RequestId" in data and e.code != "InternalError":
+                self.circuit_breaker.after_requests(generation, True)
+            else:
+                self.circuit_breaker.after_requests(generation, False)
+
+        return data
+
     def call_octet_stream(self, action, headers, body):
         """
         Invoke API with application/ocet-stream content-type.
 
         Note:
         1. only specific API can be invoked in such manner.
         2. only TC3-HMAC-SHA256 signature method can be specified.
```

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/sign.py` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/README.rst` & `tencentcloud-sdk-python-common-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-common-3.0.925/setup.py` & `tencentcloud-sdk-python-common-3.0.926/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-common-3.0.926/tencentcloud_sdk_python_common.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.rst
 setup.cfg
 setup.py
 tencentcloud/__init__.py
 tencentcloud/common/__init__.py
 tencentcloud/common/abstract_client.py
 tencentcloud/common/abstract_model.py
+tencentcloud/common/circuit_breaker.py
 tencentcloud/common/common_client.py
 tencentcloud/common/credential.py
 tencentcloud/common/sign.py
 tencentcloud/common/exception/__init__.py
 tencentcloud/common/exception/tencent_cloud_sdk_exception.py
 tencentcloud/common/http/__init__.py
 tencentcloud/common/http/request.py
```

### Comparing `tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.926/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


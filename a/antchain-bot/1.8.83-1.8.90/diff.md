# Comparing `tmp/antchain_bot-1.8.83.tar.gz` & `tmp/antchain_bot-1.8.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.8.83.tar", last modified: Sun Jun 25 09:02:42 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.8.90.tar", last modified: Mon Jul  3 03:13:27 2023, max compression
```

## Comparing `antchain_bot-1.8.83.tar` & `antchain_bot-1.8.90.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   436652 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)  1161657 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-25 09:02:42.000000 antchain_bot-1.8.83/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-25 09:02:41.000000 antchain_bot-1.8.83/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   444092 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1184117 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 03:13:27.000000 antchain_bot-1.8.90/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-07-03 03:13:26.000000 antchain_bot-1.8.90/setup.py
```

### Comparing `antchain_bot-1.8.83/LICENSE` & `antchain_bot-1.8.90/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.83/PKG-INFO` & `antchain_bot-1.8.90/antchain_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_bot
-Version: 1.8.83
+Name: antchain-bot
+Version: 1.8.90
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.83/README-CN.md` & `antchain_bot-1.8.90/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.83/README.md` & `antchain_bot-1.8.90/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.83/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.8.90/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-bot
-Version: 1.8.83
+Name: antchain_bot
+Version: 1.8.90
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.83/antchain_sdk_bot/client.py` & `antchain_bot-1.8.90/antchain_sdk_bot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.83',
+                    'sdk_version': '1.8.90',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.83',
+                    'sdk_version': '1.8.90',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -9993,14 +9993,182 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.QueryThingmodelEventResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.thingmodel.event.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_entityrelation_jtdevicebycar(
+        self,
+        request: bot_models.QueryEntityrelationJtdevicebycarRequest,
+    ) -> bot_models.QueryEntityrelationJtdevicebycarResponse:
+        """
+        Description: 通过车辆车牌的颜色+号码+场景码，查询关联的部标设备对应的IoT可信平台唯一ID
+        Summary: 车辆关联的部标设备列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_entityrelation_jtdevicebycar_ex(request, headers, runtime)
+
+    async def query_entityrelation_jtdevicebycar_async(
+        self,
+        request: bot_models.QueryEntityrelationJtdevicebycarRequest,
+    ) -> bot_models.QueryEntityrelationJtdevicebycarResponse:
+        """
+        Description: 通过车辆车牌的颜色+号码+场景码，查询关联的部标设备对应的IoT可信平台唯一ID
+        Summary: 车辆关联的部标设备列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_entityrelation_jtdevicebycar_ex_async(request, headers, runtime)
+
+    def query_entityrelation_jtdevicebycar_ex(
+        self,
+        request: bot_models.QueryEntityrelationJtdevicebycarRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryEntityrelationJtdevicebycarResponse:
+        """
+        Description: 通过车辆车牌的颜色+号码+场景码，查询关联的部标设备对应的IoT可信平台唯一ID
+        Summary: 车辆关联的部标设备列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryEntityrelationJtdevicebycarResponse(),
+            self.do_request('1.0', 'blockchain.bot.entityrelation.jtdevicebycar.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_entityrelation_jtdevicebycar_ex_async(
+        self,
+        request: bot_models.QueryEntityrelationJtdevicebycarRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryEntityrelationJtdevicebycarResponse:
+        """
+        Description: 通过车辆车牌的颜色+号码+场景码，查询关联的部标设备对应的IoT可信平台唯一ID
+        Summary: 车辆关联的部标设备列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryEntityrelationJtdevicebycarResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.entityrelation.jtdevicebycar.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_collector_jtflux(
+        self,
+        request: bot_models.QueryCollectorJtfluxRequest,
+    ) -> bot_models.QueryCollectorJtfluxResponse:
+        """
+        Description: 部标设备位置/轨迹/异常数据查询
+        Summary: 部标设备位置/轨迹/异常数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_collector_jtflux_ex(request, headers, runtime)
+
+    async def query_collector_jtflux_async(
+        self,
+        request: bot_models.QueryCollectorJtfluxRequest,
+    ) -> bot_models.QueryCollectorJtfluxResponse:
+        """
+        Description: 部标设备位置/轨迹/异常数据查询
+        Summary: 部标设备位置/轨迹/异常数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_collector_jtflux_ex_async(request, headers, runtime)
+
+    def query_collector_jtflux_ex(
+        self,
+        request: bot_models.QueryCollectorJtfluxRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryCollectorJtfluxResponse:
+        """
+        Description: 部标设备位置/轨迹/异常数据查询
+        Summary: 部标设备位置/轨迹/异常数据查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryCollectorJtfluxResponse(),
+            self.do_request('1.0', 'blockchain.bot.collector.jtflux.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_collector_jtflux_ex_async(
+        self,
+        request: bot_models.QueryCollectorJtfluxRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryCollectorJtfluxResponse:
+        """
+        Description: 部标设备位置/轨迹/异常数据查询
+        Summary: 部标设备位置/轨迹/异常数据查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryCollectorJtfluxResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.collector.jtflux.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_collector_jtmedia(
+        self,
+        request: bot_models.QueryCollectorJtmediaRequest,
+    ) -> bot_models.QueryCollectorJtmediaResponse:
+        """
+        Description: 通过异常事件ID查询部标多媒体文件地址
+        Summary: 通过异常事件ID查询部标多媒体文件地址
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_collector_jtmedia_ex(request, headers, runtime)
+
+    async def query_collector_jtmedia_async(
+        self,
+        request: bot_models.QueryCollectorJtmediaRequest,
+    ) -> bot_models.QueryCollectorJtmediaResponse:
+        """
+        Description: 通过异常事件ID查询部标多媒体文件地址
+        Summary: 通过异常事件ID查询部标多媒体文件地址
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_collector_jtmedia_ex_async(request, headers, runtime)
+
+    def query_collector_jtmedia_ex(
+        self,
+        request: bot_models.QueryCollectorJtmediaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryCollectorJtmediaResponse:
+        """
+        Description: 通过异常事件ID查询部标多媒体文件地址
+        Summary: 通过异常事件ID查询部标多媒体文件地址
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryCollectorJtmediaResponse(),
+            self.do_request('1.0', 'blockchain.bot.collector.jtmedia.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_collector_jtmedia_ex_async(
+        self,
+        request: bot_models.QueryCollectorJtmediaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.QueryCollectorJtmediaResponse:
+        """
+        Description: 通过异常事件ID查询部标多媒体文件地址
+        Summary: 通过异常事件ID查询部标多媒体文件地址
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.QueryCollectorJtmediaResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.collector.jtmedia.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def exec_thingsdid_oneapi(
         self,
         request: bot_models.ExecThingsdidOneapiRequest,
     ) -> bot_models.ExecThingsdidOneapiResponse:
         """
         Description: 信物链oneapi
         Summary: 信物链oneapi
```

### Comparing `antchain_bot-1.8.83/antchain_sdk_bot/models.py` & `antchain_bot-1.8.90/antchain_sdk_bot/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1392,14 +1392,65 @@
         if m.get('point_identification_results') is not None:
             for k in m.get('point_identification_results'):
                 temp_model = GoodsDigitalFingerprintPointIdentificationResult()
                 self.point_identification_results.append(temp_model.from_map(k))
         return self
 
 
+class JtData(TeaModel):
+    def __init__(
+        self,
+        trustiot_id: int = None,
+        trustiot_entity_id: int = None,
+        processed_content: str = None,
+        delta_mileage: int = None,
+    ):
+        # 数据的可信平台唯一ID
+        self.trustiot_id = trustiot_id
+        # IoT可信平台设备唯一ID
+        self.trustiot_entity_id = trustiot_entity_id
+        # 上报原文解析处理之后的数据
+        self.processed_content = processed_content
+        # 和上一次上报数据里程对比，新增的里程数
+        self.delta_mileage = delta_mileage
+
+    def validate(self):
+        self.validate_required(self.trustiot_id, 'trustiot_id')
+        self.validate_required(self.trustiot_entity_id, 'trustiot_entity_id')
+        self.validate_required(self.processed_content, 'processed_content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.trustiot_id is not None:
+            result['trustiot_id'] = self.trustiot_id
+        if self.trustiot_entity_id is not None:
+            result['trustiot_entity_id'] = self.trustiot_entity_id
+        if self.processed_content is not None:
+            result['processed_content'] = self.processed_content
+        if self.delta_mileage is not None:
+            result['delta_mileage'] = self.delta_mileage
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('trustiot_id') is not None:
+            self.trustiot_id = m.get('trustiot_id')
+        if m.get('trustiot_entity_id') is not None:
+            self.trustiot_entity_id = m.get('trustiot_entity_id')
+        if m.get('processed_content') is not None:
+            self.processed_content = m.get('processed_content')
+        if m.get('delta_mileage') is not None:
+            self.delta_mileage = m.get('delta_mileage')
+        return self
+
+
 class RentContractInfo(TeaModel):
     def __init__(
         self,
         contract_id: str = None,
         lease_time: str = None,
         checkin_date: str = None,
         checkout_date: str = None,
@@ -4781,14 +4832,74 @@
         if m.get('identification_message') is not None:
             self.identification_message = m.get('identification_message')
         if m.get('unable_identify_solution') is not None:
             self.unable_identify_solution = m.get('unable_identify_solution')
         return self
 
 
+class JtMedia(TeaModel):
+    def __init__(
+        self,
+        media_id: str = None,
+        name: str = None,
+        url: str = None,
+        gmt_create: int = None,
+        media_type: str = None,
+    ):
+        # 多媒体ID
+        self.media_id = media_id
+        # 文件名称
+        self.name = name
+        # 可访问的url
+        self.url = url
+        # 上传时间
+        self.gmt_create = gmt_create
+        # 多媒体类型枚举：IMAGE 图像；AUDIO 音频；VIDEO视频； UN_KNOW  未知；
+        self.media_type = media_type
+
+    def validate(self):
+        self.validate_required(self.media_id, 'media_id')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.url, 'url')
+        self.validate_required(self.gmt_create, 'gmt_create')
+        self.validate_required(self.media_type, 'media_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.media_id is not None:
+            result['media_id'] = self.media_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.url is not None:
+            result['url'] = self.url
+        if self.gmt_create is not None:
+            result['gmt_create'] = self.gmt_create
+        if self.media_type is not None:
+            result['media_type'] = self.media_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('media_id') is not None:
+            self.media_id = m.get('media_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        if m.get('gmt_create') is not None:
+            self.gmt_create = m.get('gmt_create')
+        if m.get('media_type') is not None:
+            self.media_type = m.get('media_type')
+        return self
+
+
 class BaiGoodsPointCheckRespData(TeaModel):
     def __init__(
         self,
         valid: bool = None,
     ):
         # 图片是否有效，无效则需要提示重拍
         self.valid = valid
@@ -5574,14 +5685,81 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('image_url') is not None:
             self.image_url = m.get('image_url')
         return self
 
 
+class JtDevice(TeaModel):
+    def __init__(
+        self,
+        device_id: str = None,
+        scene: str = None,
+        trustiot_device_id: int = None,
+        gmt_create: int = None,
+        online: bool = None,
+        device_model: str = None,
+    ):
+        # 设备ID
+        self.device_id = device_id
+        # 场景码
+        self.scene = scene
+        # 可信设备ID
+        self.trustiot_device_id = trustiot_device_id
+        # 设备注册时间
+        self.gmt_create = gmt_create
+        # 设备是否在线
+        self.online = online
+        # 设备型号
+        self.device_model = device_model
+
+    def validate(self):
+        self.validate_required(self.device_id, 'device_id')
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.trustiot_device_id, 'trustiot_device_id')
+        self.validate_required(self.gmt_create, 'gmt_create')
+        self.validate_required(self.online, 'online')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.trustiot_device_id is not None:
+            result['trustiot_device_id'] = self.trustiot_device_id
+        if self.gmt_create is not None:
+            result['gmt_create'] = self.gmt_create
+        if self.online is not None:
+            result['online'] = self.online
+        if self.device_model is not None:
+            result['device_model'] = self.device_model
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('trustiot_device_id') is not None:
+            self.trustiot_device_id = m.get('trustiot_device_id')
+        if m.get('gmt_create') is not None:
+            self.gmt_create = m.get('gmt_create')
+        if m.get('online') is not None:
+            self.online = m.get('online')
+        if m.get('device_model') is not None:
+            self.device_model = m.get('device_model')
+        return self
+
+
 class ComputerInfo(TeaModel):
     def __init__(
         self,
         colour: str = None,
         colour_number: str = None,
         computer_model: str = None,
         config_param: str = None,
@@ -7233,14 +7411,58 @@
         if m.get('service_status') is not None:
             self.service_status = m.get('service_status')
         if m.get('screen_status') is not None:
             self.screen_status = m.get('screen_status')
         return self
 
 
+class JtExtraData(TeaModel):
+    def __init__(
+        self,
+        delta_mileage: int = None,
+        max_speed: int = None,
+        avg_speed: int = None,
+    ):
+        # 查询的时间范围内的行驶总里程
+        self.delta_mileage = delta_mileage
+        # 最大车速
+        self.max_speed = max_speed
+        # 平均车速
+        self.avg_speed = avg_speed
+
+    def validate(self):
+        self.validate_required(self.delta_mileage, 'delta_mileage')
+        self.validate_required(self.max_speed, 'max_speed')
+        self.validate_required(self.avg_speed, 'avg_speed')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.delta_mileage is not None:
+            result['delta_mileage'] = self.delta_mileage
+        if self.max_speed is not None:
+            result['max_speed'] = self.max_speed
+        if self.avg_speed is not None:
+            result['avg_speed'] = self.avg_speed
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('delta_mileage') is not None:
+            self.delta_mileage = m.get('delta_mileage')
+        if m.get('max_speed') is not None:
+            self.max_speed = m.get('max_speed')
+        if m.get('avg_speed') is not None:
+            self.avg_speed = m.get('avg_speed')
+        return self
+
+
 class DidBaseQueryResp(TeaModel):
     def __init__(
         self,
         auth_level: int = None,
         cert_public_key: str = None,
         cert_text: str = None,
         did_extension: str = None,
@@ -30511,14 +30733,426 @@
         if m.get('thing_model_event_json') is not None:
             self.thing_model_event_json = m.get('thing_model_event_json')
         if m.get('data_demo') is not None:
             self.data_demo = m.get('data_demo')
         return self
 
 
+class QueryEntityrelationJtdevicebycarRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        device_id: str = None,
+        scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 车辆ID： 车辆车牌颜色+车牌号
+        self.device_id = device_id
+        # 场景码
+        self.scene = scene
+
+    def validate(self):
+        self.validate_required(self.device_id, 'device_id')
+        self.validate_required(self.scene, 'scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        return self
+
+
+class QueryEntityrelationJtdevicebycarResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        device_list: List[JtDevice] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 车辆关联的部标设备列表
+        self.device_list = device_list
+
+    def validate(self):
+        if self.device_list:
+            for k in self.device_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['device_list'] = []
+        if self.device_list is not None:
+            for k in self.device_list:
+                result['device_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.device_list = []
+        if m.get('device_list') is not None:
+            for k in m.get('device_list'):
+                temp_model = JtDevice()
+                self.device_list.append(temp_model.from_map(k))
+        return self
+
+
+class QueryCollectorJtfluxRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        query_type: str = None,
+        query_mode: str = None,
+        scene: str = None,
+        trustiot_device_id_list: List[int] = None,
+        start_time: int = None,
+        end_time: int = None,
+        alarm_types: List[str] = None,
+        page_index: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 查询类型，支持LOCATION, TRACE,  ALARM三类
+        self.query_type = query_type
+        # 查询模式，支持抽样SAMPLE和分页PAGE两类，query_type不是LOCATION时必填
+        self.query_mode = query_mode
+        # 场景码
+        self.scene = scene
+        # 部标设备可信平台唯一ID列表
+        self.trustiot_device_id_list = trustiot_device_id_list
+        # 开始时间，查询TRACE,  ALARM时必填
+        self.start_time = start_time
+        # 结束时间，查询TRACE,  ALARM时必填
+        self.end_time = end_time
+        # 查询ALARM的类型，默认查全部类型，包括ALARM_BASIC,ALARM_ADAS ,ALARM_DSM,ALARM_ACCELEROMETER四类
+        self.alarm_types = alarm_types
+        # 页码
+        self.page_index = page_index
+        # 单页数量
+        self.page_size = page_size
+
+    def validate(self):
+        self.validate_required(self.query_type, 'query_type')
+        self.validate_required(self.scene, 'scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.query_type is not None:
+            result['query_type'] = self.query_type
+        if self.query_mode is not None:
+            result['query_mode'] = self.query_mode
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.trustiot_device_id_list is not None:
+            result['trustiot_device_id_list'] = self.trustiot_device_id_list
+        if self.start_time is not None:
+            result['start_time'] = self.start_time
+        if self.end_time is not None:
+            result['end_time'] = self.end_time
+        if self.alarm_types is not None:
+            result['alarm_types'] = self.alarm_types
+        if self.page_index is not None:
+            result['page_index'] = self.page_index
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('query_type') is not None:
+            self.query_type = m.get('query_type')
+        if m.get('query_mode') is not None:
+            self.query_mode = m.get('query_mode')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('trustiot_device_id_list') is not None:
+            self.trustiot_device_id_list = m.get('trustiot_device_id_list')
+        if m.get('start_time') is not None:
+            self.start_time = m.get('start_time')
+        if m.get('end_time') is not None:
+            self.end_time = m.get('end_time')
+        if m.get('alarm_types') is not None:
+            self.alarm_types = m.get('alarm_types')
+        if m.get('page_index') is not None:
+            self.page_index = m.get('page_index')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class QueryCollectorJtfluxResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        page_index: int = None,
+        page_size: int = None,
+        total_size: int = None,
+        total_pages: int = None,
+        page_data: List[JtData] = None,
+        extra_data: JtExtraData = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 1
+        self.page_index = page_index
+        # 单页数量
+        self.page_size = page_size
+        # 总记录数
+        self.total_size = total_size
+        # 总页数
+        self.total_pages = total_pages
+        # 部标数据列表
+        self.page_data = page_data
+        # 聚合统计指标
+        self.extra_data = extra_data
+
+    def validate(self):
+        if self.page_data:
+            for k in self.page_data:
+                if k:
+                    k.validate()
+        if self.extra_data:
+            self.extra_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.page_index is not None:
+            result['page_index'] = self.page_index
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total_size is not None:
+            result['total_size'] = self.total_size
+        if self.total_pages is not None:
+            result['total_pages'] = self.total_pages
+        result['page_data'] = []
+        if self.page_data is not None:
+            for k in self.page_data:
+                result['page_data'].append(k.to_map() if k else None)
+        if self.extra_data is not None:
+            result['extra_data'] = self.extra_data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('page_index') is not None:
+            self.page_index = m.get('page_index')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total_size') is not None:
+            self.total_size = m.get('total_size')
+        if m.get('total_pages') is not None:
+            self.total_pages = m.get('total_pages')
+        self.page_data = []
+        if m.get('page_data') is not None:
+            for k in m.get('page_data'):
+                temp_model = JtData()
+                self.page_data.append(temp_model.from_map(k))
+        if m.get('extra_data') is not None:
+            temp_model = JtExtraData()
+            self.extra_data = temp_model.from_map(m['extra_data'])
+        return self
+
+
+class QueryCollectorJtmediaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        scene: str = None,
+        alarm_event_id: str = None,
+        media_id_list: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 场景码
+        self.scene = scene
+        # 异常事件ID，由告警事件标识生成，在blockchain.bot.collector.jtflux.query接口中可获取
+        self.alarm_event_id = alarm_event_id
+        # 异常事件媒体文件ID列表
+        self.media_id_list = media_id_list
+
+    def validate(self):
+        self.validate_required(self.scene, 'scene')
+        self.validate_required(self.alarm_event_id, 'alarm_event_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.scene is not None:
+            result['scene'] = self.scene
+        if self.alarm_event_id is not None:
+            result['alarm_event_id'] = self.alarm_event_id
+        if self.media_id_list is not None:
+            result['media_id_list'] = self.media_id_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('scene') is not None:
+            self.scene = m.get('scene')
+        if m.get('alarm_event_id') is not None:
+            self.alarm_event_id = m.get('alarm_event_id')
+        if m.get('media_id_list') is not None:
+            self.media_id_list = m.get('media_id_list')
+        return self
+
+
+class QueryCollectorJtmediaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        media_list: List[JtMedia] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 多媒体文件列表
+        self.media_list = media_list
+
+    def validate(self):
+        if self.media_list:
+            for k in self.media_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['media_list'] = []
+        if self.media_list is not None:
+            for k in self.media_list:
+                result['media_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.media_list = []
+        if m.get('media_list') is not None:
+            for k in m.get('media_list'):
+                temp_model = JtMedia()
+                self.media_list.append(temp_model.from_map(k))
+        return self
+
+
 class ExecThingsdidOneapiRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_content: str = None,
     ):
```

### Comparing `antchain_bot-1.8.83/setup.py` & `antchain_bot-1.8.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 25/06/2023
+Created on 03/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```


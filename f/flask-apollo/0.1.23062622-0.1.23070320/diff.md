# Comparing `tmp/flask_apollo-0.1.23062622-py2.py3-none-any.whl.zip` & `tmp/flask_apollo-0.1.23070320-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5482 bytes, number of entries: 7
--rw-r--r--  2.0 unx      263 b- defN 23-Jun-26 14:40 flask_apollo/__init__.py
--rw-r--r--  2.0 unx     2380 b- defN 23-Jun-25 15:15 flask_apollo/_apollo_app.py
--rw-r--r--  2.0 unx     9100 b- defN 23-Jun-26 14:39 flask_apollo/apollo.py
--rw-r--r--  2.0 unx      559 b- defN 23-Jun-26 14:45 flask_apollo-0.1.23062622.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-26 14:45 flask_apollo-0.1.23062622.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-26 14:45 flask_apollo-0.1.23062622.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      589 b- defN 23-Jun-26 14:45 flask_apollo-0.1.23062622.dist-info/RECORD
-7 files, 13014 bytes uncompressed, 4430 bytes compressed:  66.0%
+Zip file size: 5517 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-03 13:10 flask_apollo/__init__.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-Jul-03 13:10 flask_apollo/_apollo_app.py
+-rw-r--r--  2.0 unx     9378 b- defN 23-Jul-03 13:10 flask_apollo/apollo.py
+-rw-r--r--  2.0 unx      559 b- defN 23-Jul-03 13:18 flask_apollo-0.1.23070320.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-03 13:18 flask_apollo-0.1.23070320.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-03 13:18 flask_apollo-0.1.23070320.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      589 b- defN 23-Jul-03 13:18 flask_apollo-0.1.23070320.dist-info/RECORD
+7 files, 13266 bytes uncompressed, 4465 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: flask_apollo/_apollo_app.py
 Comment: 
 
 Filename: flask_apollo/apollo.py
 Comment: 
 
-Filename: flask_apollo-0.1.23062622.dist-info/METADATA
+Filename: flask_apollo-0.1.23070320.dist-info/METADATA
 Comment: 
 
-Filename: flask_apollo-0.1.23062622.dist-info/WHEEL
+Filename: flask_apollo-0.1.23070320.dist-info/WHEEL
 Comment: 
 
-Filename: flask_apollo-0.1.23062622.dist-info/top_level.txt
+Filename: flask_apollo-0.1.23070320.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_apollo-0.1.23062622.dist-info/RECORD
+Filename: flask_apollo-0.1.23070320.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_apollo/__init__.py

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
 # @Time     : 2021/6/7 上午11:23
 # @Author   : binger
 name = __package__
-version_info = (0, 1, 23062622)
+version_info = (0, 1, 23070320)
 __version__ = ".".join([str(v) for v in version_info])
-__description__ = 'flask apollo apply'
+__description__ = 'Flask Apollo Apply'
 
 from ._apollo_app import FlaskApollo
```

## flask_apollo/_apollo_app.py

```diff
@@ -6,14 +6,16 @@
 
 from flask import Flask
 
 from .apollo import Apollo
 
 
 class FlaskApollo(Apollo):
+    UPDATE_FUNC_CB_FIELD = "cb"
+
     def __init__(self, config_url, app_id, cluster="default", secret=None, request_timeout=None,
                  ip=None, notification_rule: Optional[Dict[str, Dict]] = None):
         self._notification_rule = notification_rule or {"application": {"prefix": ""}}
         super().__init__(config_url, app_id, cluster, secret, keep_hot_update=False, request_timeout=request_timeout,
                          ip=ip, namespaces=self._notification_rule.keys(), change_func=self._handle_data_change)
         self._result_map = {}
         self._sync_all_result_cb = None
@@ -31,27 +33,25 @@
     def _handle_data_change(self, namespace, notification_id, configurations: dict, old_configurations: dict):
         n_info = self._notification_rule.get(namespace, {})
         prefix = n_info.get("prefix")
         if prefix:
             configurations = {key: value for key, value in configurations.items() if key.startswith(prefix)}
 
         callable(self._sync_all_result_cb) and self._sync_all_result_cb(namespace, configurations)
-        func = n_info.get("func")
+        func = n_info.get(self.UPDATE_FUNC_CB_FIELD)
         if callable(func):
             self._result_map[namespace] = func(notification_id, configurations, old_configurations)
         return
 
     def register_for_sync(self, namespace: Optional[str], prefix=None):
-        self._notification_ids.append({self.NAMESPACE_NAME: namespace, self.NOTIFICATION_ID: -1})
-
         # 监听启动后，不允许注册
         # assert not self.is_syncing, "The monitoring has already started, and the current registration is invalid"
 
         def decorator(func):
-            self._notification_rule[namespace] = {"cb": func, "prefix": prefix}
+            self._notification_rule[namespace] = {self.UPDATE_FUNC_CB_FIELD: func, "prefix": prefix}
             self.add_notification_ids((namespace,))
 
             @wraps(func)
             def wrapper(*args, **kwargs):
                 return self._result_map.get(namespace)
 
             return wrapper
```

## flask_apollo/apollo.py

```diff
@@ -42,42 +42,43 @@
 
         self._request_timeout = request_timeout
         self._change_func = change_func
 
         self._stopping = False
         self._hot_syncing = False
         self._namespace_cache = {}
-        self._notification_ids = []
+        self._notification_ids_pool = {}
         if namespaces:
             self.add_notification_ids(namespaces)
         if keep_hot_update:
             self.start()
 
     def get_value(self, key, default_val=None, namespace='application'):
         n_data = self._namespace_cache.get(namespace) or {}
         conf = n_data.get("CONFIGURATIONS") or {}
         return conf.get(key, default_val)
 
     def add_notification_ids(self, namespaces, notification_id=-1):
         for namespace in namespaces:
-            self._notification_ids.append({self.NAMESPACE_NAME: namespace, self.NOTIFICATION_ID: notification_id})
+            self._notification_ids_pool[namespace] = {self.NAMESPACE_NAME: namespace,
+                                                      self.NOTIFICATION_ID: notification_id}
 
     @property
     def is_syncing(self):
         return self._hot_syncing
 
     def stop(self):
         self._stopping = True
         logger.info("Stopping sync...")
 
     def run_forever(self, interval: Optional[int] = None):
         interval = interval or self.LOOP_INTERVAL
         self._hot_syncing = True
-        if not self._namespace_cache:
-            self.sync_for_app(self._notification_ids)
+        # if not self._namespace_cache:
+        #     self.sync_for_app(self._notification_ids_pool)
 
         while not self._stopping:
             time.sleep(interval)
             try:
                 self.sync_for_app()
             except Exception as e:
                 logger.error(f"sync for app: {e.args}")
@@ -157,24 +158,26 @@
             self._namespace_cache[namespace] = n_data
 
             try:
                 # 处理监听推送
                 callable(self._change_func) and self._change_func(namespace=namespace,
                                                                   notification_id=self.NOTIFICATION_ID,
                                                                   configurations=n_data[self.CONFIGURATIONS],
-                                                                  old_configurations=src_n_data.get(self.CONFIGURATIONS))
+                                                                  old_configurations=src_n_data.get(
+                                                                      self.CONFIGURATIONS))
             except Exception as e:
                 logger.warning(f"change notification {namespace}")
 
-    def sync_for_app(self, default_notifications=None):
+    def sync_for_app(self, notifications_pool=None):
         notifications = []  # 通知信息
         for namespace, n_data in self._namespace_cache.items():
             notifications.append({self.NAMESPACE_NAME: namespace, self.NOTIFICATION_ID: -1})
         if not notifications:
-            notifications = default_notifications
+            temp = notifications_pool or self._notification_ids_pool
+            notifications = list(temp.values())
 
         # 查看数据版本是否变化
         url = '{}/notifications/v2'.format(self.config_url)
         params = {
             'appId': self.app_id,
             'cluster': self.cluster,
             'notifications': json.dumps(notifications, ensure_ascii=False)
@@ -190,21 +193,22 @@
                 self._sync_data_from_namespace(namespace=info[self.NAMESPACE_NAME],
                                                notification_id=info[self.NOTIFICATION_ID])
             logger.debug("sync for app: compare end!")
         else:
             logger.warning(f"sync for app: bnormal response http code:{http_code}, text: {res.text}")
         return True
 
-    def sync_for_app_use_now_notifications(self, default_notifications=None):
+    def sync_for_app_use_now_notifications(self, notifications_pool=None):
         notifications = []  # 通知信息
         for namespace, n_data in self._namespace_cache.items():
             notification_id = n_data.get(self.NOTIFICATION_ID, -1)
             notifications.append({self.NAMESPACE_NAME: namespace, self.NOTIFICATION_ID: notification_id})
         if not notifications:
-            notifications = default_notifications
+            temp = notifications_pool or self._notification_ids_pool
+            notifications = list(temp.values())
 
         # 查看数据版本是否变化
         url = '{}/notifications/v2'.format(self.config_url)
         params = {
             'appId': self.app_id,
             'cluster': self.cluster,
             'notifications': json.dumps(notifications, ensure_ascii=False)
@@ -232,8 +236,8 @@
     apollo_config_url = "url"
 
     client = Apollo(app_id="common-config", cluster="default", config_url=apollo_config_url,
                     keep_hot_update=True)
     # val = client.get_value("CHAT_CHATGPT_H5_TIMEOUT", default_val="defaultVal", namespace="CountryCodeBlacklist")
     while client.is_syncing:
         time.sleep(2)
-        print(client._namespace_cache)
+        print(client._namespace_cache)
```

## Comparing `flask_apollo-0.1.23062622.dist-info/METADATA` & `flask_apollo-0.1.23070320.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flask-apollo
-Version: 0.1.23062622
-Summary: flask apollo apply
+Version: 0.1.23070320
+Summary: Flask Apollo Apply
 Home-page: https://github.com/BingerYang/Flask-Apollo
 Author: binger
 Author-email: <xuehen_521@126.com>
 Maintainer: binger
 Maintainer-email: <xuehen_521@126.com>
 Platform: all
 Requires-Python: >=3.4
```

## Comparing `flask_apollo-0.1.23062622.dist-info/RECORD` & `flask_apollo-0.1.23070320.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-flask_apollo/__init__.py,sha256=RstwmhoTU1SA1LVHkTvTFszDoZmKLtmZgk0LN4-_qqE,263
-flask_apollo/_apollo_app.py,sha256=n5PZPmQU51mZ8IX7vg55ZmoANzSn7Yu9HCU0m4-Ifa4,2380
-flask_apollo/apollo.py,sha256=wXdsPAcpPGWlNR44gLb562mV3VBnZLMtGI3QIStlwiw,9100
-flask_apollo-0.1.23062622.dist-info/METADATA,sha256=Ca5ASBf_oulxuI5oHbn-x0bzTkQ1TmZ8AZzlMNhzynA,559
-flask_apollo-0.1.23062622.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-flask_apollo-0.1.23062622.dist-info/top_level.txt,sha256=ILeJ2xv6AgRWzTjXW2D_A-gXTAA-Gw3tftj7P_3o3ds,13
-flask_apollo-0.1.23062622.dist-info/RECORD,,
+flask_apollo/__init__.py,sha256=bO2md5ylSOFJVOGkTOVw8jjvgiVZYRqtOjUsXvtHRbU,263
+flask_apollo/_apollo_app.py,sha256=7RUb03I2isEciAHxgrrvrYIDxCnIMiY6e0Zb1bV6XDM,2354
+flask_apollo/apollo.py,sha256=bP5kKorj16MheOaaENFu4574de73ZWV4T5_KI-SjxSI,9378
+flask_apollo-0.1.23070320.dist-info/METADATA,sha256=rpDkMqfa0tNTs1AYLGDw6UUWWlzCBKEknY8BBsvKTKI,559
+flask_apollo-0.1.23070320.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+flask_apollo-0.1.23070320.dist-info/top_level.txt,sha256=ILeJ2xv6AgRWzTjXW2D_A-gXTAA-Gw3tftj7P_3o3ds,13
+flask_apollo-0.1.23070320.dist-info/RECORD,,
```


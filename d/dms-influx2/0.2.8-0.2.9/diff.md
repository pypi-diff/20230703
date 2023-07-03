# Comparing `tmp/dms-influx2-0.2.8.tar.gz` & `tmp/dms-influx2-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.2.8.tar", last modified: Tue Apr 11 13:25:18 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.2.9.tar", last modified: Mon Jul  3 09:38:48 2023, max compression
```

## Comparing `dms-influx2-0.2.8.tar` & `dms-influx2-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:18.510575 dms-influx2-0.2.8/
--rw-rw-rw-   0        0        0      556 2023-04-11 13:25:18.510575 dms-influx2-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:18.505332 dms-influx2-0.2.8/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.8/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.8/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2384 2023-03-22 11:20:22.000000 dms-influx2-0.2.8/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.8/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    21500 2023-04-11 13:17:17.000000 dms-influx2-0.2.8/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-04-11 05:18:02.000000 dms-influx2-0.2.8/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.8/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.8/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:18.508575 dms-influx2-0.2.8/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-04-11 13:25:18.000000 dms-influx2-0.2.8/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-04-11 13:25:18.000000 dms-influx2-0.2.8/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:25:18.000000 dms-influx2-0.2.8/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-04-11 13:25:18.000000 dms-influx2-0.2.8/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 13:25:18.000000 dms-influx2-0.2.8/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 13:25:18.511575 dms-influx2-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-04-11 13:24:27.000000 dms-influx2-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:18.510575 dms-influx2-0.2.8/tests/
--rw-rw-rw-   0        0        0     2163 2023-03-22 11:20:06.000000 dms-influx2-0.2.8/tests/test_auth.py
--rw-rw-rw-   0        0        0     4894 2023-01-09 21:18:36.000000 dms-influx2-0.2.8/tests/test_buckets.py
--rw-rw-rw-   0        0        0     2212 2023-01-19 07:31:43.000000 dms-influx2-0.2.8/tests/test_copy-values.py
--rw-rw-rw-   0        0        0    10842 2023-01-23 07:03:29.000000 dms-influx2-0.2.8/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.623565 dms-influx2-0.2.9/
+-rw-rw-rw-   0        0        0      556 2023-07-03 09:38:48.623565 dms-influx2-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.611539 dms-influx2-0.2.9/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.9/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.9/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.2.9/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.9/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    21500 2023-04-11 13:17:17.000000 dms-influx2-0.2.9/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-04-11 05:18:02.000000 dms-influx2-0.2.9/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.9/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.9/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.621564 dms-influx2-0.2.9/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 09:38:48.624564 dms-influx2-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-07-03 09:38:14.000000 dms-influx2-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.623565 dms-influx2-0.2.9/tests/
+-rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.2.9/tests/test_auth.py
+-rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.2.9/tests/test_buckets.py
+-rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.2.9/tests/test_copy-values.py
+-rw-rw-rw-   0        0        0    11926 2023-07-03 09:34:27.000000 dms-influx2-0.2.9/tests/test_data.py
```

### Comparing `dms-influx2-0.2.8/PKG-INFO` & `dms-influx2-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.8/dms_influx2/authorizations.py` & `dms-influx2-0.2.9/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/buckets.py` & `dms-influx2-0.2.9/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/checks.py` & `dms-influx2-0.2.9/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/decorators.py` & `dms-influx2-0.2.9/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/delete.py` & `dms-influx2-0.2.9/dms_influx2/delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import itertools
-from datetime import datetime
+from datetime import datetime, timedelta
+from typing import Union
+
 from dateutil.parser import parse
 from influxdb_client import DeleteApi
 
 from dms_influx2.utils import timestamp_to_influx_string
 
 
 class Delete(DeleteApi):
     def __init__(self, client):
         self.org = client.org
         self.time_offset = client.time_offset
         self.query_str = client.query_str
         super().__init__(client)
 
-    def delete_data(self, bucket, measurements=None, device_ids=None, descriptions=None, org=None,
-                    time_range=None, time_from=None, time_to=None) -> dict:
+    def delete_data(self,
+                    bucket,
+                    measurements=None,
+                    device_ids=None,
+                    descriptions=None,
+                    org: str = None,
+                    time_range: str = None,
+                    time_from: Union[str, datetime] = None,
+                    time_to:  Union[str, datetime] = None) -> dict:
 
         # TODO: add time_range
         if time_range is not None:
             pass
 
         if org is None:
             org = self.org
 
         if time_from is None:
             start = "1900-01-01T00:00:00Z"
         else:
             start = timestamp_to_influx_string(time_from, self.time_offset)
 
         if time_to is None:
-            stop = timestamp_to_influx_string(datetime.now(), self.time_offset)
+            # Add some safety timedelta
+            stop_time = datetime.now() + timedelta(days=1)
+            stop = timestamp_to_influx_string(stop_time, self.time_offset)
         else:
             stop = timestamp_to_influx_string(time_to, self.time_offset)
 
         predicates = []
 
         if measurements is not None:
             _predicates = []
```

### Comparing `dms-influx2-0.2.8/dms_influx2/dtv_files.py` & `dms-influx2-0.2.9/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/lib.py` & `dms-influx2-0.2.9/dms_influx2/lib.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/notifications.py` & `dms-influx2-0.2.9/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/organisations.py` & `dms-influx2-0.2.9/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/query.py` & `dms-influx2-0.2.9/dms_influx2/query.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/tasks.py` & `dms-influx2-0.2.9/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2/utils.py` & `dms-influx2-0.2.9/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.2.9/dms_influx2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.8/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.2.9/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.8/setup.py` & `dms-influx2-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `dms-influx2-0.2.8/tests/test_auth.py` & `dms-influx2-0.2.9/tests/test_auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,35 @@
-from datetime import datetime
-from dotenv import dotenv_values
+import os
 import pytest
 from influxdb_client.rest import ApiException
 
 from dms_influx2.lib import DmsInflux2
 
-config = dotenv_values()
-
-host = config['INFLUX_HOST']
-port = config['INFLUX_PORT']
-token = config['DOCKER_INFLUXDB_INIT_ADMIN_TOKEN']
-org = config['DOCKER_INFLUXDB_INIT_ORG']
-url = f'http://{host}:{port}'
-client = DmsInflux2(url=url, token=token, org=org)
-
-bucket = 'test_bucket'
-
-def test_ping():
-    if not client.ping():
-        pytest.exit('Unable to connect to influx database')
+DATABASE_URL = os.environ['DATABASE_URL']
+TOKEN = os.environ['TOKEN']
+ORG = os.environ['ORG']
+BUCKET = 'test_bucket'
+CLIENT = DmsInflux2(url=DATABASE_URL, token=TOKEN, org=ORG)
 
 
 def test_bucket_exists():
-    if client.buckets_api().bucket_exists(bucket):
-        client.buckets_api().delete_bucket_by_name(bucket)
-    client.buckets_api()._create_bucket(bucket_name=bucket)
-    assert client.buckets_api().bucket_exists(bucket)
+    if CLIENT.buckets_api().bucket_exists(BUCKET):
+        CLIENT.buckets_api().delete_bucket_by_name(BUCKET)
+    CLIENT.buckets_api()._create_bucket(bucket_name=BUCKET)
+    assert CLIENT.buckets_api().bucket_exists(BUCKET)
 
 
 def test_delete_authorization():
-    auth = client.authorizations_api().create_bucket_authorization(bucket_name=bucket, org_name=org)
+    auth = CLIENT.authorizations_api().create_bucket_authorization(bucket_name=BUCKET, org_name=ORG)
     assert len(auth.id) > 5
 
-    assert client.authorizations_api().delete_authorization(auth) is None
+    assert CLIENT.authorizations_api().delete_authorization(auth) is None
 
     with pytest.raises(ApiException):
-        client.authorizations_api().find_authorization_by_id(auth_id=auth.id)
-
-
-
+        CLIENT.authorizations_api().find_authorization_by_id(auth_id=auth.id)
 
 # # # TODO fix this test
 # def test_create_bucket_with_token_and_delete_permissions():
 #     """Test create new bucket with auth token and check for writes/reads permissions"""
 #
 #     new_token = client.buckets_api().create_bucket_with_auth(bucket_name=bucket).token
 #
@@ -61,9 +48,7 @@
 #     data = {
 #         "measurement": measurement,
 #         "device_id": "test.ch",
 #         "values": [(datetime.utcnow(), 0)]
 #     }
 #     with pytest.raises(Exception):
 #         client2.save_data(bucket=bucket, data=data)
-
-
```


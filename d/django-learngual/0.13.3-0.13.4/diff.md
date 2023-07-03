# Comparing `tmp/django-learngual-0.13.3.tar.gz` & `tmp/django-learngual-0.13.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.3.tar", last modified: Sat Jul  1 17:36:29 2023, max compression
+gzip compressed data, was "django-learngual-0.13.4.tar", last modified: Mon Jul  3 12:11:02 2023, max compression
```

## Comparing `django-learngual-0.13.3.tar` & `django-learngual-0.13.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-01 17:35:38.000000 django-learngual-0.13.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 17:35:38.000000 django-learngual-0.13.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 17:36:29.346193 django-learngual-0.13.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-01 17:35:38.000000 django-learngual-0.13.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 17:36:29.346193 django-learngual-0.13.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:35:38.000000 django-learngual-0.13.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-03 12:09:56.000000 django-learngual-0.13.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 12:09:56.000000 django-learngual-0.13.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 12:11:02.212942 django-learngual-0.13.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-03 12:09:56.000000 django-learngual-0.13.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.208942 django-learngual-0.13.4/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 12:11:02.000000 django-learngual-0.13.4/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:11:02.212942 django-learngual-0.13.4/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-07-03 12:10:55.000000 django-learngual-0.13.4/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-03 12:11:02.212942 django-learngual-0.13.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:09:56.000000 django-learngual-0.13.4/setup.py
```

### Comparing `django-learngual-0.13.3/LICENSE` & `django-learngual-0.13.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/PKG-INFO` & `django-learngual-0.13.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.3
+Version: 0.13.4
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.3/README.rst` & `django-learngual-0.13.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.4/django_learngual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.3
+Version: 0.13.4
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.3/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.4/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/apps.py` & `django-learngual-0.13.4/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/authentication.py` & `django-learngual-0.13.4/learngual/authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/permissions.py` & `django-learngual-0.13.4/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/tests/request_mock.py` & `django-learngual-0.13.4/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/tests/test_authentication.py` & `django-learngual-0.13.4/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/tests/test_utils.py` & `django-learngual-0.13.4/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.3/learngual/utils.py` & `django-learngual-0.13.4/learngual/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import os
 from typing import Any, Literal
 
 import requests
 from django.conf import settings
 from django.core.cache import cache
-
-# from django.utils import timezone
+from django.utils import timezone
 
 LEARNGUAL_SERVICE_API_KEY = getattr(
     settings, "LEARNGUAL_SERVICE_API_KEY", None
 ) or os.getenv("LEARNGUAL_SERVICE_API_KEY", None)
 
 
 def get_service_request_headers(**kwargs) -> dict:
@@ -418,33 +417,50 @@
             json=permmission_data,
             headers=get_service_request_headers(**headers),
         )
         if not res.ok:
             raise requests.exceptions.RequestException(res.content)
         return res.json()
 
+    def clear_cache(
+        self,
+        *,
+        service: Literal["iam", "payment", "notify", "learn", "media"] = "iam",
+        permission_id: str,
+    ):
+        """clear cache
+
+        Args:
+            permission_id (str): _description_
+            service (Literal["iam", "payment", "notify", "learn", "media"], optional): _description_. Defaults to "iam".
+        """
+        url_path = f"/{service}/v1/service/permission/{permission_id}/"
+        cache.delete(url_path)
+
     def retrieve_permission(
         self,
         *,
         base_url: str,
-        permission_id,
+        permission_id: str,
         service: Literal["iam", "payment", "notify", "learn", "media"] = "iam",
         dot_path: str = None,
         headers: dict = dict(),
         params: str = "",
+        cache_timeout: float = timezone.timedelta(hours=1).total_seconds(),
     ):
         """_summary_
 
         Args:
             permission_id (str): example: '123456', 'sdGh66gGGHgfadsty', 'product:1234567'
             service (_type_): "iam" | "pay" | "notify" | "learn" | "media"
             base_url (str):
             dot_path (str):Default:None, e.g metadata.request_count.value
             headers (dict):Default:{}
             params (str):Default:"", e.g name=ann&age=102
+            cache_timeout (float):Default:timezone.timedelta(hours=1).total_seconds()
         """
         url_path = f"/{service}/v1/service/permission/{permission_id}/"
         data = cache.get(url_path)
 
         params = params.strip("?")
         params = dict([x.split("=") for x in params.split("&") if x])
 
@@ -452,13 +468,12 @@
             res = requests.get(
                 base_url.rstrip("/") + url_path + get_service_request_params(**params),
                 headers=get_service_request_headers(**headers),
             )
             if not res.ok:
                 raise requests.exceptions.RequestException(res.content)
             data = res.json()
-            # TODO fine a way to remove the cache when a new permission is added
-            # cache.set(url_path, data, timeout=timezone.timedelta(hours=1).total_seconds())
+            cache.set(url_path, data, timeout=cache_timeout)
 
         if dot_path:
             return get_nested_value(data, dot_path)
         return data
```

### Comparing `django-learngual-0.13.3/setup.cfg` & `django-learngual-0.13.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.13.3
+version = 0.13.4
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```


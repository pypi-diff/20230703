# Comparing `tmp/nc_py_api-0.0.20.tar.gz` & `tmp/nc_py_api-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.20.tar", last modified: Mon Jul  3 13:27:53 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.21.tar", last modified: Mon Jul  3 20:47:18 2023, max compression
```

## Comparing `nc_py_api-0.0.20.tar` & `nc_py_api-0.0.21.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3620 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:27:53.571613 nc_py_api-0.0.20/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12312 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4016 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3620 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:27:46.000000 nc_py_api-0.0.20/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:47:18.208260 nc_py_api-0.0.21/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12320 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 20:47:10.000000 nc_py_api-0.0.21/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/setup.py
```

### Comparing `nc_py_api-0.0.20/LICENSE` & `nc_py_api-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/PKG-INFO` & `nc_py_api-0.0.21/nc_py_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: nc_py_api
-Version: 0.0.20
+Name: nc-py-api
+Version: 0.0.21
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `nc_py_api-0.0.20/README.md` & `nc_py_api-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/_session.py` & `nc_py_api-0.0.21/nc_py_api/_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             self.dav_url_suffix = options.DAV_URL_SUFFIX
         self.dav_endpoint = self.endpoint + self.dav_url_suffix
 
     @staticmethod
     def _get_value(value_name: str, raise_not_found=True, **kwargs):
         value = kwargs.get(value_name, None)
         if not value:
-            value = environ.get(value_name, None)
+            value = environ.get(value_name.upper(), None)
         if not value and raise_not_found:
             raise ValueError(f"`{value_name}` is not found.")
         return value
 
 
 @dataclass
 class Config(BasicConfig):
```

### Comparing `nc_py_api-0.0.20/nc_py_api/appconfig_preferences_ex.py` & `nc_py_api-0.0.21/nc_py_api/appconfig_preferences_ex.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/apps.py` & `nc_py_api-0.0.21/nc_py_api/apps.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/constants.py` & `nc_py_api-0.0.21/nc_py_api/constants.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/exceptions.py` & `nc_py_api-0.0.21/nc_py_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/files.py` & `nc_py_api-0.0.21/nc_py_api/files.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.21/nc_py_api/integration_fastapi.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/misc.py` & `nc_py_api-0.0.21/nc_py_api/misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/nextcloud.py` & `nc_py_api-0.0.21/nc_py_api/nextcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Nextcloud class providing access to all API endpoints.
 """
 from abc import ABC
 from typing import Optional, Union
 
 from fastapi import Request
 
-from ._session import NcSession, NcSessionApp, NcSessionBasic, ServerVersion
+from ._session import AppConfig, NcSession, NcSessionApp, NcSessionBasic, ServerVersion
 from .appconfig_preferences_ex import AppConfigExAPI, PreferencesExAPI
 from .apps import AppAPI
 from .constants import APP_V2_BASIC_URL, ApiScope, LogLvl
 from .files import FilesAPI
 from .misc import check_capabilities
 from .preferences import PreferencesAPI
 from .theming import ThemingInfo, get_parsed_theme
@@ -110,14 +110,18 @@
 
     @user.setter
     def user(self, value: str):
         if self._session.user != value:
             self._session.user = value
             self._session.update_server_info()
 
+    @property
+    def app_cfg(self) -> AppConfig:
+        return self._session.cfg
+
     def request_sign_check(self, request: Request) -> bool:
         try:
             self._session.sign_check(request)
         except ValueError as e:
             print(e)
             return False
         return True
```

### Comparing `nc_py_api-0.0.20/nc_py_api/preferences.py` & `nc_py_api-0.0.21/nc_py_api/preferences.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/theming.py` & `nc_py_api-0.0.21/nc_py_api/theming.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.21/nc_py_api/ui_files_actions_menu.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/users.py` & `nc_py_api-0.0.21/nc_py_api/users.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/users_groups.py` & `nc_py_api-0.0.21/nc_py_api/users_groups.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/users_status.py` & `nc_py_api-0.0.21/nc_py_api/users_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api/weather_status.py` & `nc_py_api-0.0.21/nc_py_api/weather_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: nc-py-api
-Version: 0.0.20
+Name: nc_py_api
+Version: 0.0.21
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `nc_py_api-0.0.20/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.21/nc_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/pyproject.toml` & `nc_py_api-0.0.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.20/setup.cfg` & `nc_py_api-0.0.21/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 long_description_content_type = text/markdown
 url = https://github.com/cloud-py-api/nc_py_api
 author = Alexander Piskun
 keywords = nextcloud, api, framework
 classifiers = 
 	Development Status :: 1 - Planning
 	Intended Audience :: Developers
+	Topic :: Internet :: WWW/HTTP
+	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: Libraries :: Application Frameworks
+	Topic :: Software Development :: Libraries :: Python Modules
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
```


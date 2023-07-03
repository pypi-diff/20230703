# Comparing `tmp/Bubot_WebServer-0.1.8.tar.gz` & `tmp/Bubot_WebServer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bubot_WebServer-0.1.8.tar", last modified: Sun Mar  5 13:28:05 2023, max compression
+gzip compressed data, was "Bubot_WebServer-0.1.9.tar", last modified: Mon Mar  6 22:45:12 2023, max compression
```

## Comparing `Bubot_WebServer-0.1.8.tar` & `Bubot_WebServer-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.059058 Bubot_WebServer-0.1.8/
--rw-rw-rw-   0        0        0     1088 2021-03-01 14:55:15.000000 Bubot_WebServer-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      817 2023-03-05 13:28:05.058059 Bubot_WebServer-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      290 2021-03-01 22:12:34.000000 Bubot_WebServer-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-05 13:28:05.059058 Bubot_WebServer-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:04.919988 Bubot_WebServer-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:04.919988 Bubot_WebServer-0.1.8/src/BubotObj/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:04.917988 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:04.918988 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:04.980799 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.006550 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/
--rw-rw-rw-   0        0        0     1803 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Device.py
--rw-rw-rw-   0        0        0     2221 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Driver.py
--rw-rw-rw-   0        0        0     3142 2022-03-13 09:52:43.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Resource.py
--rw-rw-rw-   0        0        0      242 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Schema.py
--rw-rw-rw-   0        0        0     1234 2022-03-27 14:03:06.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Store.py
--rw-rw-rw-   0        0        0        2 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/__init__.py
--rw-rw-rw-   0        0        0        0 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/Actions.py
--rw-rw-rw-   0        0        0     1049 2023-01-10 15:56:53.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/ApiHelper.py
--rw-rw-rw-   0        0        0     4778 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/FormHandler.py
--rw-rw-rw-   0        0        0     6788 2023-02-05 20:17:12.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/HttpHandler.py
--rw-rw-rw-   0        0        0     2738 2022-03-13 09:52:43.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/SchemaHandler.py
--rw-rw-rw-   0        0        0     3323 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageApp.py
--rw-rw-rw-   0        0        0     3387 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageMongo.py
--rw-rw-rw-   0        0        0      132 2022-09-03 19:22:55.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WebServer.json
--rw-rw-rw-   0        0        0    10382 2023-02-19 17:57:53.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WebServer.py
--rw-rw-rw-   0        0        0      879 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.md
--rw-rw-rw-   0        0        0     7003 2023-01-18 22:17:17.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.py
--rw-rw-rw-   0        0        0       23 2023-03-05 13:27:34.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.014056 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/i18n/
--rw-rw-rw-   0        0        0     1190 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/i18n/en.json
--rw-rw-rw-   0        0        0     2654 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/i18n/ru.json
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.022056 Bubot_WebServer-0.1.8/src/BubotObj/Session/
--rw-rw-rw-   0        0        0       88 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/Session/Session.dict.json
--rw-rw-rw-   0        0        0     2673 2023-03-02 22:01:39.000000 Bubot_WebServer-0.1.8/src/BubotObj/Session/Session.py
--rw-rw-rw-   0        0        0      313 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/src/BubotObj/Session/Session.schema.json
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.023056 Bubot_WebServer-0.1.8/src/BubotObj/User/
--rw-rw-rw-   0        0        0     4112 2023-02-28 18:02:46.000000 Bubot_WebServer-0.1.8/src/BubotObj/User/User.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.030061 Bubot_WebServer-0.1.8/src/BubotObj/User/form/
--rw-rw-rw-   0        0        0      114 2021-02-28 19:36:45.000000 Bubot_WebServer-0.1.8/src/BubotObj/User/form/AccessRight.form.json
--rw-rw-rw-   0        0        0      107 2021-02-28 19:36:45.000000 Bubot_WebServer-0.1.8/src/BubotObj/User/form/CurrentUser.form.json
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.042061 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/
--rw-rw-rw-   0        0        0      817 2023-03-05 13:28:04.000000 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1737 2023-03-05 13:28:04.000000 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 13:28:04.000000 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-03-01 22:23:34.000000 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       64 2023-03-05 13:28:04.000000 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-05 13:28:04.000000 Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-05 13:28:05.058059 Bubot_WebServer-0.1.8/tests/
--rw-rw-rw-   0        0        0      461 2021-03-01 20:39:23.000000 Bubot_WebServer-0.1.8/tests/TestBasic.py
--rw-rw-rw-   0        0        0        0 2019-08-31 09:27:15.000000 Bubot_WebServer-0.1.8/tests/TestScheduler.py
--rw-rw-rw-   0        0        0     2057 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.8/tests/TestUser.py
--rw-rw-rw-   0        0        0     2523 2021-03-01 20:41:29.000000 Bubot_WebServer-0.1.8/tests/TestWebServer.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.607824 Bubot_WebServer-0.1.9/
+-rw-rw-rw-   0        0        0     1088 2021-03-01 14:55:15.000000 Bubot_WebServer-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      817 2023-03-06 22:45:12.606824 Bubot_WebServer-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2021-03-01 22:12:34.000000 Bubot_WebServer-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-03-06 22:45:12.607824 Bubot_WebServer-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1191 2023-03-06 22:40:47.000000 Bubot_WebServer-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.511822 Bubot_WebServer-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.510823 Bubot_WebServer-0.1.9/src/BubotObj/
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.509823 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.509823 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.549823 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.567823 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/
+-rw-rw-rw-   0        0        0     1803 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Device.py
+-rw-rw-rw-   0        0        0     2221 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Driver.py
+-rw-rw-rw-   0        0        0     3142 2022-03-13 09:52:43.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Resource.py
+-rw-rw-rw-   0        0        0      242 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Schema.py
+-rw-rw-rw-   0        0        0     1234 2022-03-27 14:03:06.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Store.py
+-rw-rw-rw-   0        0        0        2 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/Actions.py
+-rw-rw-rw-   0        0        0     1049 2023-01-10 15:56:53.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/ApiHelper.py
+-rw-rw-rw-   0        0        0     4778 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/FormHandler.py
+-rw-rw-rw-   0        0        0     6788 2023-02-05 20:17:12.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/HttpHandler.py
+-rw-rw-rw-   0        0        0     2738 2022-03-13 09:52:43.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/SchemaHandler.py
+-rw-rw-rw-   0        0        0     3323 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageApp.py
+-rw-rw-rw-   0        0        0     3387 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageMongo.py
+-rw-rw-rw-   0        0        0      132 2022-09-03 19:22:55.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WebServer.json
+-rw-rw-rw-   0        0        0    10638 2023-03-06 21:57:14.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WebServer.py
+-rw-rw-rw-   0        0        0      879 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.md
+-rw-rw-rw-   0        0        0     7003 2023-01-18 22:17:17.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.py
+-rw-rw-rw-   0        0        0       23 2023-03-06 22:38:50.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.568823 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/i18n/
+-rw-rw-rw-   0        0        0     1190 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/i18n/en.json
+-rw-rw-rw-   0        0        0     2654 2021-02-28 19:36:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/i18n/ru.json
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.573824 Bubot_WebServer-0.1.9/src/BubotObj/Session/
+-rw-rw-rw-   0        0        0       88 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/Session/Session.dict.json
+-rw-rw-rw-   0        0        0     2673 2023-03-02 22:01:39.000000 Bubot_WebServer-0.1.9/src/BubotObj/Session/Session.py
+-rw-rw-rw-   0        0        0      313 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.9/src/BubotObj/Session/Session.schema.json
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.574823 Bubot_WebServer-0.1.9/src/BubotObj/User/
+-rw-rw-rw-   0        0        0     4112 2023-02-28 18:02:46.000000 Bubot_WebServer-0.1.9/src/BubotObj/User/User.py
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.580824 Bubot_WebServer-0.1.9/src/BubotObj/User/form/
+-rw-rw-rw-   0        0        0      114 2021-02-28 19:36:45.000000 Bubot_WebServer-0.1.9/src/BubotObj/User/form/AccessRight.form.json
+-rw-rw-rw-   0        0        0      107 2021-02-28 19:36:45.000000 Bubot_WebServer-0.1.9/src/BubotObj/User/form/CurrentUser.form.json
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.592823 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/
+-rw-rw-rw-   0        0        0      817 2023-03-06 22:45:12.000000 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1737 2023-03-06 22:45:12.000000 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-06 22:45:12.000000 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-03-01 22:23:34.000000 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-03-06 22:45:12.000000 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-06 22:45:12.000000 Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-06 22:45:12.605824 Bubot_WebServer-0.1.9/tests/
+-rw-rw-rw-   0        0        0      461 2021-03-01 20:39:23.000000 Bubot_WebServer-0.1.9/tests/TestBasic.py
+-rw-rw-rw-   0        0        0        0 2019-08-31 09:27:15.000000 Bubot_WebServer-0.1.9/tests/TestScheduler.py
+-rw-rw-rw-   0        0        0     2057 2023-01-10 15:56:44.000000 Bubot_WebServer-0.1.9/tests/TestUser.py
+-rw-rw-rw-   0        0        0     2523 2021-03-01 20:41:29.000000 Bubot_WebServer-0.1.9/tests/TestWebServer.py
```

### Comparing `Bubot_WebServer-0.1.8/LICENSE` & `Bubot_WebServer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/PKG-INFO` & `Bubot_WebServer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bubot_WebServer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Web server for Bubot
 Home-page: https://github.com/businka/Bubot_WebServer
 Author: Razgovorov Mikhail
 Author-email: 1338833@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Bubot_WebServer-0.1.8/setup.py` & `Bubot_WebServer-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,12 +25,13 @@
         "Development Status :: 3 - Alpha",
         "Framework :: AsyncIO",
     ],
     python_requires='>=3.7',
     zip_safe=False,
     install_requires=[
         'motor>=3',
+        'aioredis',
         'aiohttp>=3.7,<4',
         'aiohttp-session>=2.9',
-        'Bubot_Core>=0.1.4',
+        'Bubot_Core>=0.1.8',
     ]
 )
```

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Device.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Device.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Driver.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Driver.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Resource.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Resource.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Store.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/APImixin/Store.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/ApiHelper.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/ApiHelper.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/FormHandler.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/FormHandler.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/HttpHandler.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/HttpHandler.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/SchemaHandler.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/SchemaHandler.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageApp.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageApp.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageMongo.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/SessionStorageMongo.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WebServer.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WebServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # from bubot.Client.OcfDevice.OcfDevice import OcfDevice
 import asyncio
 import json
 import os.path
 from uuid import uuid4
-
+import aioredis
 # from bubot.Catalog.Client.WebServer import API
 from Bubot.Core.DataBase.Mongo import Mongo as Storage
 # from bubot.Core.DataBase.SqlLite import SqlLite as Storage
 from Bubot.Core.FastStorage.Simple import SimpleFastStorage as FastStorage
 from Bubot.Helpers.ActionDecorator import async_action
 from Bubot.Helpers.ExtException import ExtException, ResourceNotAvailable
 from Bubot.Helpers.Helper import Helper
@@ -29,39 +29,42 @@
 
 # from bson import ObjectId
 
 
 # _logger = logging.getLogger(__name__)
 
 
-class WebServer(VirtualServer, QueueMixin):
+class WebServer(VirtualServer):#, QueueMixin):
     version = device_version
     file = __file__
     template = False
     forms = dict()
 
     def __init__(self, **kwargs):
         # self.drivers = []
         # self.resources = []
         # self.cache_schemas = {}
         self.schemas_dir = []
         self.net_devices = {}
-        self.request_queue = asyncio.Queue()
-        self.serial_queue_worker = None
+        # self.request_queue = asyncio.Queue()
+        # self.serial_queue_worker = None
         self.ws = {}
         self.runner = None
         self.storage = None
+        self.redis = None
         VirtualServer.__init__(self, **kwargs)
 
     async def on_pending(self):
         # self.serial_queue_worker = asyncio.ensure_future(self.queue_worker(self.request_queue, 'request_queue'))
         await self.run_web_server()
         await super().on_pending()
 
     async def on_cancelled(self):
+        if self.redis:
+            await self.redis.close()
         if self.storage:
             await self.storage.close()
         if self.runner is not None:
             await self.runner.cleanup()
         await super().on_cancelled()
 
     @async_action
@@ -72,14 +75,17 @@
         # self.log.info(f'{self.__class__.__name__} start up')
         app = web.Application(
             # middlewares=[
             #     self.middleware_auth,
             #     self.middleware_index
             # ]
         )
+        redis_url = self.get_param('/oic/con', 'redis_url')
+        if redis_url:
+            self.redis = await aioredis.from_url(redis_url)
         app['device'] = self
         app['sessions'] = {}
         app['fast_storage'] = FastStorage()
         self.storage = await Storage.connect(self)
         app['storage'] = self.storage
         app.middlewares.append(self.middleware_index)
         _session_storage = self.get_session_storage(app, self.get_param('/oic/con', 'session_storage', 'App'))
```

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.md` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.md`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.py` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/WsHandler.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/i18n/en.json` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/i18n/en.json`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/OcfDevice/subtype/WebServer/i18n/ru.json` & `Bubot_WebServer-0.1.9/src/BubotObj/OcfDevice/subtype/WebServer/i18n/ru.json`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/Session/Session.py` & `Bubot_WebServer-0.1.9/src/BubotObj/Session/Session.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/BubotObj/User/User.py` & `Bubot_WebServer-0.1.9/src/BubotObj/User/User.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/PKG-INFO` & `Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bubot-WebServer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Web server for Bubot
 Home-page: https://github.com/businka/Bubot_WebServer
 Author: Razgovorov Mikhail
 Author-email: 1338833@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Bubot_WebServer-0.1.8/src/Bubot_WebServer.egg-info/SOURCES.txt` & `Bubot_WebServer-0.1.9/src/Bubot_WebServer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/tests/TestUser.py` & `Bubot_WebServer-0.1.9/tests/TestUser.py`

 * *Files identical despite different names*

### Comparing `Bubot_WebServer-0.1.8/tests/TestWebServer.py` & `Bubot_WebServer-0.1.9/tests/TestWebServer.py`

 * *Files identical despite different names*


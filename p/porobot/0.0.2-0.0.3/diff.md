# Comparing `tmp/porobot-0.0.2.tar.gz` & `tmp/porobot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porobot-0.0.2.tar", last modified: Thu Jun 29 15:08:53 2023, max compression
+gzip compressed data, was "porobot-0.0.3.tar", last modified: Mon Jul  3 15:15:19 2023, max compression
```

## Comparing `porobot-0.0.2.tar` & `porobot-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.030921 porobot-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-06-29 14:40:45.000000 porobot-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      565 2023-06-29 15:08:53.030921 porobot-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       32 2023-06-29 14:40:45.000000 porobot-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.011276 porobot-0.0.2/porobot/
--rw-rw-rw-   0        0        0       32 2023-06-29 15:02:34.000000 porobot-0.0.2/porobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot/api/
--rw-rw-rw-   0        0        0       15 2023-06-29 15:02:05.000000 porobot-0.0.2/porobot/api/__init__.py
--rw-rw-rw-   0        0        0      338 2023-06-29 15:06:53.000000 porobot-0.0.2/porobot/api/normal.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot/core/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.2/porobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.2/porobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/porobot.egg-info/
--rw-rw-rw-   0        0        0      565 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 14:59:29.000000 porobot-0.0.2/porobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-29 15:08:52.000000 porobot-0.0.2/porobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-06-29 15:08:53.030921 porobot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 porobot-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:53.021328 porobot-0.0.2/tests/
--rw-rw-rw-   0        0        0      268 2023-06-29 15:04:12.000000 porobot-0.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.938723 porobot-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-29 14:40:45.000000 porobot-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      565 2023-07-03 15:15:19.938723 porobot-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2023-06-29 14:40:45.000000 porobot-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.897006 porobot-0.0.3/porobot/
+-rw-rw-rw-   0        0        0       32 2023-06-29 15:02:34.000000 porobot-0.0.3/porobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.932347 porobot-0.0.3/porobot/api/
+-rw-rw-rw-   0        0        0       15 2023-06-29 15:02:05.000000 porobot-0.0.3/porobot/api/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-06-29 15:06:53.000000 porobot-0.0.3/porobot/api/normal.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.933859 porobot-0.0.3/porobot/core/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.3/porobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.935680 porobot-0.0.3/porobot/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 porobot-0.0.3/porobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.928355 porobot-0.0.3/porobot.egg-info/
+-rw-rw-rw-   0        0        0      565 2023-07-03 15:15:19.000000 porobot-0.0.3/porobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-03 15:15:19.000000 porobot-0.0.3/porobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:15:19.000000 porobot-0.0.3/porobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 14:59:29.000000 porobot-0.0.3/porobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-07-03 15:15:19.000000 porobot-0.0.3/porobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 15:15:19.000000 porobot-0.0.3/porobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2023-07-03 15:15:19.941725 porobot-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 porobot-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:15:19.937711 porobot-0.0.3/tests/
+-rw-rw-rw-   0        0        0      268 2023-06-29 15:04:12.000000 porobot-0.0.3/tests/test.py
```

### Comparing `porobot-0.0.2/LICENSE` & `porobot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `porobot-0.0.2/PKG-INFO` & `porobot-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porobot
-Version: 0.0.2
+Version: 0.0.3
 Summary: pip install porobot
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/porobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/porobot/blob/master/README.md
```

### Comparing `porobot-0.0.2/porobot.egg-info/PKG-INFO` & `porobot-0.0.3/porobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porobot
-Version: 0.0.2
+Version: 0.0.3
 Summary: pip install porobot
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/porobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/porobot/blob/master/README.md
```


# Comparing `tmp/aiodanbooru-1.0.6.tar.gz` & `tmp/aiodanbooru-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.6.tar", last modified: Mon Jul  3 15:33:51 2023, max compression
+gzip compressed data, was "aiodanbooru-1.0.7.tar", last modified: Mon Jul  3 15:36:53 2023, max compression
```

## Comparing `aiodanbooru-1.0.6.tar` & `aiodanbooru-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:33:51.980436 aiodanbooru-1.0.6/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-07-03 15:33:51.980436 aiodanbooru-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 15:33:51.968913 aiodanbooru-1.0.6/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.6/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.0.6/aiodanbooru/api.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:33:51.978425 aiodanbooru-1.0.6/aiodanbooru/base/
--rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.6/aiodanbooru/base/__init__.py
--rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.6/aiodanbooru/base/filters.py
--rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.0.6/aiodanbooru/base/handler.py
--rw-rw-rw-   0        0        0     1953 2023-07-03 15:15:24.000000 aiodanbooru-1.0.6/aiodanbooru/dispatcher.py
--rw-rw-rw-   0        0        0     3237 2023-06-29 21:25:14.000000 aiodanbooru-1.0.6/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:33:51.975424 aiodanbooru-1.0.6/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-07-03 15:33:51.000000 aiodanbooru-1.0.6/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-03 15:33:51.000000 aiodanbooru-1.0.6/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:33:51.000000 aiodanbooru-1.0.6/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-03 15:33:51.000000 aiodanbooru-1.0.6/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 15:33:51.000000 aiodanbooru-1.0.6/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 15:33:51.980436 aiodanbooru-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-07-03 15:33:33.000000 aiodanbooru-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:33:51.978929 aiodanbooru-1.0.6/tests/
--rw-rw-rw-   0        0        0     1666 2023-07-03 15:31:10.000000 aiodanbooru-1.0.6/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:36:53.459125 aiodanbooru-1.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-07-03 15:36:53.459125 aiodanbooru-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 15:36:53.448614 aiodanbooru-1.0.7/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.7/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.0.7/aiodanbooru/api.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:36:53.457125 aiodanbooru-1.0.7/aiodanbooru/base/
+-rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.7/aiodanbooru/base/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.7/aiodanbooru/base/filters.py
+-rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.0.7/aiodanbooru/base/handler.py
+-rw-rw-rw-   0        0        0     1953 2023-07-03 15:15:24.000000 aiodanbooru-1.0.7/aiodanbooru/dispatcher.py
+-rw-rw-rw-   0        0        0     3237 2023-06-29 21:25:14.000000 aiodanbooru-1.0.7/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:36:53.454126 aiodanbooru-1.0.7/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-07-03 15:36:53.000000 aiodanbooru-1.0.7/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-03 15:36:53.000000 aiodanbooru-1.0.7/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:36:53.000000 aiodanbooru-1.0.7/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-03 15:36:53.000000 aiodanbooru-1.0.7/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 15:36:53.000000 aiodanbooru-1.0.7/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:36:53.459125 aiodanbooru-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-03 15:35:59.000000 aiodanbooru-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:36:53.458126 aiodanbooru-1.0.7/tests/
+-rw-rw-rw-   0        0        0     1666 2023-07-03 15:31:10.000000 aiodanbooru-1.0.7/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.6/LICENSE` & `aiodanbooru-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/PKG-INFO` & `aiodanbooru-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.6/README.md` & `aiodanbooru-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/aiodanbooru/api.py` & `aiodanbooru-1.0.7/aiodanbooru/api.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/aiodanbooru/base/filters.py` & `aiodanbooru-1.0.7/aiodanbooru/base/filters.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/aiodanbooru/base/handler.py` & `aiodanbooru-1.0.7/aiodanbooru/base/handler.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/aiodanbooru/dispatcher.py` & `aiodanbooru-1.0.7/aiodanbooru/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/aiodanbooru/models.py` & `aiodanbooru-1.0.7/aiodanbooru/models.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.6/aiodanbooru.egg-info/PKG-INFO` & `aiodanbooru-1.0.7/aiodanbooru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.6/setup.py` & `aiodanbooru-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.6",
+    version="1.0.7",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic<2.0.0",
```

### Comparing `aiodanbooru-1.0.6/tests/test_api.py` & `aiodanbooru-1.0.7/tests/test_api.py`

 * *Files identical despite different names*


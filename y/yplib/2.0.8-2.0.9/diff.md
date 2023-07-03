# Comparing `tmp/yplib-2.0.8.tar.gz` & `tmp/yplib-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.0.8.tar", last modified: Fri Jun 30 06:20:14 2023, max compression
+gzip compressed data, was "dist\yplib-2.0.9.tar", last modified: Mon Jul  3 01:28:58 2023, max compression
```

## Comparing `yplib-2.0.8.tar` & `yplib-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 06:20:14.282738 yplib-2.0.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-30 06:20:14.282564 yplib-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 06:20:14.283216 yplib-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-30 06:20:03.000000 yplib-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:20:14.279837 yplib-2.0.8/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.8/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.8/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.8/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.0.8/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.8/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.8/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:20:14.281743 yplib-2.0.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 01:28:58.882624 yplib-2.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-03 01:28:58.882624 yplib-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 01:28:58.882624 yplib-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-03 01:28:43.000000 yplib-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:28:58.879128 yplib-2.0.9/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.9/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.9/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.9/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.9/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.0.9/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.9/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5431 2023-07-03 01:26:23.000000 yplib-2.0.9/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.9/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:28:58.881733 yplib-2.0.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-03 01:28:58.000000 yplib-2.0.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-03 01:28:58.000000 yplib-2.0.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 01:28:58.000000 yplib-2.0.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-03 01:28:58.000000 yplib-2.0.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.0.8/LICENSE` & `yplib-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/setup.py` & `yplib-2.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.0.8",
+  version="2.0.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.0.8/yplib/__init__.py` & `yplib-2.0.9/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/chart.py` & `yplib-2.0.9/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/chart_html.py` & `yplib-2.0.9/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/db.py` & `yplib-2.0.9/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/file.py` & `yplib-2.0.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/http_util.py` & `yplib-2.0.9/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/index.py` & `yplib-2.0.9/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/mail.py` & `yplib-2.0.9/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.8/yplib/mail_html.py` & `yplib-2.0.9/yplib/mail_html.py`

 * *Files identical despite different names*


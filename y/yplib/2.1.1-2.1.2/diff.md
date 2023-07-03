# Comparing `tmp/yplib-2.1.1.tar.gz` & `tmp/yplib-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.1.1.tar", last modified: Mon Jul  3 01:44:12 2023, max compression
+gzip compressed data, was "dist\yplib-2.1.2.tar", last modified: Mon Jul  3 01:48:00 2023, max compression
```

## Comparing `yplib-2.1.1.tar` & `yplib-2.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 01:44:12.118181 yplib-2.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.1.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-03 01:44:12.118181 yplib-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 01:44:12.118181 yplib-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-03 01:43:02.000000 yplib-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 01:44:12.115774 yplib-2.1.1/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.1.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.1.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.1.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.1.1/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.1.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.1.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.1.1/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.1.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.1.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5428 2023-07-03 01:42:31.000000 yplib-2.1.1/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.1.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-03 01:44:12.117420 yplib-2.1.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-03 01:44:12.000000 yplib-2.1.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-03 01:44:12.000000 yplib-2.1.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 01:44:12.000000 yplib-2.1.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-03 01:44:12.000000 yplib-2.1.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 01:48:00.797351 yplib-2.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-03 01:48:00.797351 yplib-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 01:48:00.797351 yplib-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-03 01:47:45.000000 yplib-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:48:00.794394 yplib-2.1.2/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.1.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.1.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.1.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.1.2/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.1.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.1.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.1.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.1.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.1.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.1.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.1.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-03 01:48:00.796798 yplib-2.1.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-03 01:48:00.000000 yplib-2.1.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-03 01:48:00.000000 yplib-2.1.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 01:48:00.000000 yplib-2.1.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-03 01:48:00.000000 yplib-2.1.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.1.1/LICENSE` & `yplib-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/setup.py` & `yplib-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.1.1",
+  version="2.1.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.1.1/yplib/__init__.py` & `yplib-2.1.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/chart.py` & `yplib-2.1.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/chart_html.py` & `yplib-2.1.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/db.py` & `yplib-2.1.2/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/file.py` & `yplib-2.1.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/http_util.py` & `yplib-2.1.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/index.py` & `yplib-2.1.2/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/mail.py` & `yplib-2.1.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/mail_html.py` & `yplib-2.1.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.1.1/yplib/markdown.py` & `yplib-2.1.2/yplib/markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         html_list.append(get_markdown_one(data_obj, no_title=t_i_n, is_error=is_error))
     else:
         if isinstance(data_obj, list) or isinstance(data_obj, set):
             for data_one in data_obj:
                 html_list.append(get_markdown_one(data_one, no_title=no_title, is_error=is_error))
         else:
             html_list.append(get_markdown_one(data_obj, no_title=no_title, is_error=is_error))
-    return ''.join(mail_html(html_list))
+    return ''.join(html_list)
 
 
 # 获得 markdown 的内容信息
 # data_obj =
 # {
 # 	"title": "里面的一份小标题",
 # 	"type": "error",
```


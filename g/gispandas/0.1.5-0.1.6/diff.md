# Comparing `tmp/gispandas-0.1.5.tar.gz` & `tmp/gispandas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.5.tar", last modified: Mon Jul  3 09:22:47 2023, max compression
+gzip compressed data, was "gispandas-0.1.6.tar", last modified: Mon Jul  3 12:45:32 2023, max compression
```

## Comparing `gispandas-0.1.5.tar` & `gispandas-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:22:47.323130 gispandas-0.1.5/
--rw-rw-rw-   0        0        0     1026 2023-07-03 09:22:47.322132 gispandas-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-06-29 09:25:50.000000 gispandas-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 09:22:47.313157 gispandas-0.1.5/gispandas/
--rw-rw-rw-   0        0        0        0 2023-06-29 07:49:45.000000 gispandas-0.1.5/gispandas/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.5/gispandas/gispandas.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:22:47.321135 gispandas-0.1.5/gispandas.egg-info/
--rw-rw-rw-   0        0        0     1026 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 09:22:47.323130 gispandas-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-07-03 09:21:06.000000 gispandas-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 12:45:32.715837 gispandas-0.1.6/
+-rw-rw-rw-   0        0        0     1027 2023-07-03 12:45:32.715837 gispandas-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-07-03 09:54:38.000000 gispandas-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 12:45:32.706862 gispandas-0.1.6/gispandas/
+-rw-rw-rw-   0        0        0       31 2023-07-03 12:41:13.000000 gispandas-0.1.6/gispandas/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.6/gispandas/gispandas.py
+drwxrwxrwx   0        0        0        0 2023-07-03 12:45:32.713842 gispandas-0.1.6/gispandas.egg-info/
+-rw-rw-rw-   0        0        0     1027 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 12:45:32.715837 gispandas-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-07-03 12:43:04.000000 gispandas-0.1.6/setup.py
```

### Comparing `gispandas-0.1.5/PKG-INFO` & `gispandas-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gispandas
-Version: 0.1.5
+Version: 0.1.6
 Summary: gispandas
 Home-page: https://github.com/mxhou/gispandas/
 Author: HMX
 Author-email: kzdhb8023@163.com
 License: MIT
 Keywords: gis,geo,tif,json
 Requires-Python: >=3.6
@@ -14,9 +14,10 @@
 GisPandas是一个为栅格数据处理、分析和可视化而开发的Python包。GisPandas为常见栅格数据进行行政区划统计提供了快速而简洁的方法。GisPandas为遥感影像分类的后处理过程提供高效的处理，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
 栅格数据进行阿尔伯斯等面积投影，根据矢量区划会计算面积导出json。
 # 安装
 pip install gispandas
 # 相关链接
-本项目的github页面：https://github.com/mxhou/gispandas/
+本项目的github页面：https://github.com/mxhou/gispandas
+
 有bug请在这个页面提交：https://github.com/mxhou/gispandas/issues
```

### Comparing `gispandas-0.1.5/README.md` & `gispandas-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,9 +2,10 @@
 GisPandas是一个为栅格数据处理、分析和可视化而开发的Python包。GisPandas为常见栅格数据进行行政区划统计提供了快速而简洁的方法。GisPandas为遥感影像分类的后处理过程提供高效的处理，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
 栅格数据进行阿尔伯斯等面积投影，根据矢量区划会计算面积导出json。
 # 安装
 pip install gispandas
 # 相关链接
-本项目的github页面：https://github.com/mxhou/gispandas/
+本项目的github页面：https://github.com/mxhou/gispandas
+
 有bug请在这个页面提交：https://github.com/mxhou/gispandas/issues
```

### Comparing `gispandas-0.1.5/gispandas/gispandas.py` & `gispandas-0.1.6/gispandas/gispandas.py`

 * *Files identical despite different names*

### Comparing `gispandas-0.1.5/gispandas.egg-info/PKG-INFO` & `gispandas-0.1.6/gispandas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gispandas
-Version: 0.1.5
+Version: 0.1.6
 Summary: gispandas
 Home-page: https://github.com/mxhou/gispandas/
 Author: HMX
 Author-email: kzdhb8023@163.com
 License: MIT
 Keywords: gis,geo,tif,json
 Requires-Python: >=3.6
@@ -14,9 +14,10 @@
 GisPandas是一个为栅格数据处理、分析和可视化而开发的Python包。GisPandas为常见栅格数据进行行政区划统计提供了快速而简洁的方法。GisPandas为遥感影像分类的后处理过程提供高效的处理，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
 栅格数据进行阿尔伯斯等面积投影，根据矢量区划会计算面积导出json。
 # 安装
 pip install gispandas
 # 相关链接
-本项目的github页面：https://github.com/mxhou/gispandas/
+本项目的github页面：https://github.com/mxhou/gispandas
+
 有bug请在这个页面提交：https://github.com/mxhou/gispandas/issues
```

### Comparing `gispandas-0.1.5/setup.py` & `gispandas-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 filepath = path.join(this_directory, 'README.md')
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
     packages=find_packages(),
```


# Comparing `tmp/vgis_log-1.0.3.tar.gz` & `tmp/vgis_log-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_log-1.0.3.tar", last modified: Tue Jun 27 09:34:14 2023, max compression
+gzip compressed data, was "dist\vgis_log-1.0.4.tar", last modified: Mon Jul  3 06:08:12 2023, max compression
```

## Comparing `vgis_log-1.0.3.tar` & `vgis_log-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:34:14.018209 vgis_log-1.0.3/
--rw-rw-rw-   0        0        0     1022 2023-06-27 09:34:14.017238 vgis_log-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-06-27 09:06:27.000000 vgis_log-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:34:14.018209 vgis_log-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2145 2023-06-27 09:34:02.000000 vgis_log-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:34:14.007237 vgis_log-1.0.3/vgis_log/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_log-1.0.3/vgis_log/__init__.py
--rw-rw-rw-   0        0        0     5051 2023-06-27 09:32:45.000000 vgis_log-1.0.3/vgis_log/logTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:34:14.016209 vgis_log-1.0.3/vgis_log.egg-info/
--rw-rw-rw-   0        0        0     1022 2023-06-27 09:34:13.000000 vgis_log-1.0.3/vgis_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-06-27 09:34:13.000000 vgis_log-1.0.3/vgis_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:34:13.000000 vgis_log-1.0.3/vgis_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 09:34:13.000000 vgis_log-1.0.3/vgis_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 09:34:13.000000 vgis_log-1.0.3/vgis_log.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 06:08:12.971490 vgis_log-1.0.4/
+-rw-rw-rw-   0        0        0     1022 2023-07-03 06:08:12.970490 vgis_log-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2023-06-27 09:06:27.000000 vgis_log-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:08:12.971490 vgis_log-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2158 2023-07-03 06:07:50.000000 vgis_log-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:08:12.960513 vgis_log-1.0.4/vgis_log/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_log-1.0.4/vgis_log/__init__.py
+-rw-rw-rw-   0        0        0     5042 2023-07-03 06:07:00.000000 vgis_log-1.0.4/vgis_log/logTools.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:08:12.968490 vgis_log-1.0.4/vgis_log.egg-info/
+-rw-rw-rw-   0        0        0     1022 2023-07-03 06:08:12.000000 vgis_log-1.0.4/vgis_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-07-03 06:08:12.000000 vgis_log-1.0.4/vgis_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:08:12.000000 vgis_log-1.0.4/vgis_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-03 06:08:12.000000 vgis_log-1.0.4/vgis_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 06:08:12.000000 vgis_log-1.0.4/vgis_log.egg-info/top_level.txt
```

### Comparing `vgis_log-1.0.3/PKG-INFO` & `vgis_log-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_log
-Version: 1.0.3
+Version: 1.0.4
 Summary: A libary for log operator
 Home-page: https://github.com/gisfanmachel/vgisLog
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis log lib
```

### Comparing `vgis_log-1.0.3/setup.py` & `vgis_log-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_log",  # Required 项目名称
-    version="1.0.3",  # Required 发布版本号
+    version="1.0.4",  # Required 发布版本号
     description="A libary for log operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisLog",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
@@ -44,14 +44,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
 
     keywords="log,setuptools,development",  # Optional 搜索关键字
 
-    packages=find_packages(),  # Required
+    packages=find_packages(),  # RequiredC
 
     python_requires=">=3.7, <4",  # python 版本要求
 
-    install_requires=["vgis-utils"],  # Optional 第三方依赖库
+    install_requires=["vgis-utils", "logoru"],  # Optional 第三方依赖库
 
-)
+)
```

### Comparing `vgis_log-1.0.3/vgis_log/logTools.py` & `vgis_log-1.0.4/vgis_log/logTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def insert_log_info(SysLog,username, operation, method, params, time, ip, error_info):
         create_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         data = {}
         data["username"] = username
         data["operation"] = operation
         data["method"] = method
         data["params"] = params
-        data["vgis_datetime"] = time
+        data["time"] = time
         data["ip"] = ip
         data["create_date"] = create_time
         data["error_info"] = error_info
         SysLog.objects.create(**data)
 
     @staticmethod
     def set_start_log_info(logger):
```

### Comparing `vgis_log-1.0.3/vgis_log.egg-info/PKG-INFO` & `vgis_log-1.0.4/vgis_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-log
-Version: 1.0.3
+Version: 1.0.4
 Summary: A libary for log operator
 Home-page: https://github.com/gisfanmachel/vgisLog
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis log lib
```


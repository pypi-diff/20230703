# Comparing `tmp/pydatawork-0.17.3.1.tar.gz` & `tmp/pydatawork-0.17.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.3.1.tar", last modified: Mon Jul  3 14:06:18 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.3.2.tar", last modified: Mon Jul  3 14:13:25 2023, max compression
```

## Comparing `pydatawork-0.17.3.1.tar` & `pydatawork-0.17.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18555 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    13980 2023-07-03 13:54:13.000000 pydatawork-0.17.3.1/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18555 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    39093 2023-07-03 14:05:45.000000 pydatawork-0.17.3.1/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 13:54:41.000000 pydatawork-0.17.3.1/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    14084 2023-07-03 14:12:21.000000 pydatawork-0.17.3.2/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    39093 2023-07-03 14:05:45.000000 pydatawork-0.17.3.2/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 14:13:06.000000 pydatawork-0.17.3.2/setup.py
```

### Comparing `pydatawork-0.17.3.1/PKG-INFO` & `pydatawork-0.17.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.1
+Version: 0.17.3.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -489,31 +489,41 @@
         ```
         
         
         
         ## pydatawork升级方法（先卸载，再安装）
         
         ```shell
-        pip3 uninstall pydatawork # 卸载
-        pip3 install pydatawork # 安装
+        # 卸载指令
+        pip3 uninstall pydatawork 
+        或 
+        pip uninstall pydatawork 
+        
+        # 安装指令
+        pip3 install pydatawork 
+        或 
+        pip install pydatawork 
         ```
         
         
         
         ## pydatawork 导入方式
         ```shell
         import pydatawork # 标准导入方式
         import pydatawork as dw # 推荐使用此方式，更简洁
         ```
         
         
         
         ## pydatawork安装
         ```shell
-        pip3 install pydatawork # 安装指令
+        # 安装指令
+        pip3 install pydatawork 
+        或 
+        pip install pydatawork
         ```
         
         
         
         ## 关于pydatawork
         
         数据工作相关的分享、梳理，主要目的是辅助个人开展数据处理、数据分析工作。
```

### Comparing `pydatawork-0.17.3.1/README.md` & `pydatawork-0.17.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -481,31 +481,41 @@
 ```
 
 
 
 ## pydatawork升级方法（先卸载，再安装）
 
 ```shell
-pip3 uninstall pydatawork # 卸载
-pip3 install pydatawork # 安装
+# 卸载指令
+pip3 uninstall pydatawork 
+或 
+pip uninstall pydatawork 
+
+# 安装指令
+pip3 install pydatawork 
+或 
+pip install pydatawork 
 ```
 
 
 
 ## pydatawork 导入方式
 ```shell
 import pydatawork # 标准导入方式
 import pydatawork as dw # 推荐使用此方式，更简洁
 ```
 
 
 
 ## pydatawork安装
 ```shell
-pip3 install pydatawork # 安装指令
+# 安装指令
+pip3 install pydatawork 
+或 
+pip install pydatawork
 ```
 
 
 
 ## 关于pydatawork
 
 数据工作相关的分享、梳理，主要目的是辅助个人开展数据处理、数据分析工作。
```

### Comparing `pydatawork-0.17.3.1/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.3.2/pydatawork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.1
+Version: 0.17.3.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -489,31 +489,41 @@
         ```
         
         
         
         ## pydatawork升级方法（先卸载，再安装）
         
         ```shell
-        pip3 uninstall pydatawork # 卸载
-        pip3 install pydatawork # 安装
+        # 卸载指令
+        pip3 uninstall pydatawork 
+        或 
+        pip uninstall pydatawork 
+        
+        # 安装指令
+        pip3 install pydatawork 
+        或 
+        pip install pydatawork 
         ```
         
         
         
         ## pydatawork 导入方式
         ```shell
         import pydatawork # 标准导入方式
         import pydatawork as dw # 推荐使用此方式，更简洁
         ```
         
         
         
         ## pydatawork安装
         ```shell
-        pip3 install pydatawork # 安装指令
+        # 安装指令
+        pip3 install pydatawork 
+        或 
+        pip install pydatawork
         ```
         
         
         
         ## 关于pydatawork
         
         数据工作相关的分享、梳理，主要目的是辅助个人开展数据处理、数据分析工作。
```

### Comparing `pydatawork-0.17.3.1/pydatawork.py` & `pydatawork-0.17.3.2/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.3.1/setup.py` & `pydatawork-0.17.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.3.1',
+    version='0.17.3.2',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```


# Comparing `tmp/huhangkai-1.2.3.tar.gz` & `tmp/huhangkai-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.2.3.tar", last modified: Mon Jul  3 03:02:41 2023, max compression
+gzip compressed data, was "huhangkai-1.2.4.tar", last modified: Mon Jul  3 11:05:51 2023, max compression
```

## Comparing `huhangkai-1.2.3.tar` & `huhangkai-1.2.4.tar`

### file list

```diff
@@ -1,23 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.244668 huhangkai-1.2.3/
--rw-rw-rw-   0        0        0      228 2023-07-03 03:02:41.243671 huhangkai-1.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.228689 huhangkai-1.2.3/commen/
--rw-rw-rw-   0        0        0      933 2023-06-20 02:22:12.000000 huhangkai-1.2.3/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.232700 huhangkai-1.2.3/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.3/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-06-20 09:33:09.000000 huhangkai-1.2.3/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0    29301 2023-06-20 08:10:42.000000 huhangkai-1.2.3/commen/init_project.py
--rw-rw-rw-   0        0        0    12278 2023-07-03 02:53:24.000000 huhangkai-1.2.3/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.3/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.3/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    23116 2023-06-20 08:00:58.000000 huhangkai-1.2.3/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.3/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.3/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-06-29 01:27:06.000000 huhangkai-1.2.3/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.241677 huhangkai-1.2.3/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 03:02:41.244668 huhangkai-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      643 2023-07-03 03:02:39.000000 huhangkai-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:05:51.955137 huhangkai-1.2.4/
+-rw-rw-rw-   0        0        0      228 2023-07-03 11:05:51.955137 huhangkai-1.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 11:05:51.914247 huhangkai-1.2.4/commen/
+-rw-rw-rw-   0        0        0      933 2023-06-20 02:22:12.000000 huhangkai-1.2.4/commen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:05:51.918200 huhangkai-1.2.4/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.4/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-06-20 09:33:09.000000 huhangkai-1.2.4/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0    29301 2023-06-20 08:10:42.000000 huhangkai-1.2.4/commen/init_project.py
+-rw-rw-rw-   0        0        0      676 2023-07-03 11:05:40.000000 huhangkai-1.2.4/commen/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:05:51.921193 huhangkai-1.2.4/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.4/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:05:51.944132 huhangkai-1.2.4/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.4/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3252 2023-07-03 09:00:44.000000 huhangkai-1.2.4/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-01 21:14:54.000000 huhangkai-1.2.4/commen/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     1348 2023-07-03 08:59:15.000000 huhangkai-1.2.4/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0     1548 2023-07-03 08:59:15.000000 huhangkai-1.2.4/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-03 08:59:24.000000 huhangkai-1.2.4/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-03 08:59:32.000000 huhangkai-1.2.4/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2609 2023-07-03 09:13:27.000000 huhangkai-1.2.4/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-03 09:00:16.000000 huhangkai-1.2.4/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-03 09:00:24.000000 huhangkai-1.2.4/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-03 09:00:34.000000 huhangkai-1.2.4/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    13338 2023-07-03 09:47:06.000000 huhangkai-1.2.4/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.4/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.4/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    23116 2023-06-20 08:00:58.000000 huhangkai-1.2.4/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.4/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.4/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-06-29 01:27:06.000000 huhangkai-1.2.4/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      725 2023-07-03 11:03:49.000000 huhangkai-1.2.4/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:05:51.952138 huhangkai-1.2.4/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-03 11:05:51.000000 huhangkai-1.2.4/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-07-03 11:05:51.000000 huhangkai-1.2.4/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 11:05:51.000000 huhangkai-1.2.4/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-03 11:05:51.000000 huhangkai-1.2.4/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 11:05:51.000000 huhangkai-1.2.4/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 11:05:51.956100 huhangkai-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       28 2023-07-03 11:05:40.000000 huhangkai-1.2.4/setup.py
```

### Comparing `huhangkai-1.2.3/commen/__init__.py` & `huhangkai-1.2.4/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/case_project/base_project.py` & `huhangkai-1.2.4/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/init_project.py` & `huhangkai-1.2.4/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/unit_apache_beam.py` & `huhangkai-1.2.4/commen/unit_apache_beam.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import datetime
-import re
 import time
 
 import apache_beam as beam
 import uuid
 
 from apache_beam import PCollection
 from apache_beam.pvalue import DoOutputsTuple
 from apache_beam.transforms import window
 
 
 class ApacheFun:
     window = window
 
-    def __init__(self, data=None, name="", out=None):
+    def __init__(self, data=None, name="", out=None, data_type=1):
+        """data_type: 1 管道， 2 数据"""
         self.pipeline = beam.Pipeline()
         self.data = data
         self.out = out
         self.value = None
         self.name = name or str(uuid.uuid4())[-12:]
+        self.data_type = data_type
         self._i = 0
         self._tmp_value = None
         if data:
             self.create()
 
     def __str__(self):
         return self.value
@@ -46,19 +47,30 @@
                 print(x)
         if isinstance(self.out, PCollection):
             self.out | self._name() >> beam.Map(lambda x: _print(x))
         elif isinstance(self.out, (list, tuple, DoOutputsTuple)):
             for i in self.out:
                 if isinstance(i, PCollection):
                     i | self._name() >> beam.Map(lambda x: _print(x))
-        self.run()
+                else:
+                    _print(i)
+        if self.data_type == 1:
+            self.run()
+
+    def set_data(self, data):
+        self.data = data
+        self.create(data)
+        self.out = self.value
 
     def create(self, data=None):
         """创建"""
-        self.value = self.pipeline | self._name() >> beam.Create(data or self.data)
+        if self.data_type == 1:
+            self.value = self.pipeline | self._name() >> beam.Create(data or self.data)
+        else:
+            self.value = data or self.data
         if not(data and self.data):
             self.out = self.value
         return self
 
     def par_do(self, fn, *args, **kwargs):
         """ParDo 与 DoFn 方法"""
         self.value = self.out = self.get_out() | self._name() >> beam.ParDo(fn, *args, **kwargs)
@@ -146,23 +158,24 @@
         """基于某些分区函数将每个输入元素路由到特定的输出集合。"""
         self.out = self.get_out() | self._name() >> beam.Partition(fn, num, *args, **kwargs)
         self.value = [ApacheFun(out=x) for x in self.out]
         return self
 
     def pvalue_as_dict(self, data):
         """字典"""
-        return beam.pvalue.AsDict(self.create(data).value)
+        return beam.pvalue.AsDict(self.create(data).value) if self.data_type == 1 else {k: v for k, v in data}
 
     def pvalue_as_iter(self, data):
         """列表"""
-        return beam.pvalue.AsIter(self.create(data).value)
+        return beam.pvalue.AsIter(self.create(data).value) if self.data_type == 1 else data
 
     def pvalue_as_singleton(self, data):
         """单实例"""
-        return beam.pvalue.AsSingleton(self.create(data).value)
+        data = [data] if isinstance(data, str) else data
+        return beam.pvalue.AsSingleton(self.create(data).value) if self.data_type == 1 else data[0]
 
     def keys(self, data=None):
         self.value = self.create(data).value | self._name() >> beam.Keys()
         if not(data and self.data):
             self.out = self.value
         return self
 
@@ -200,18 +213,25 @@
                 elif type == "bj":
                     plant[key] = datetime.datetime.fromtimestamp(timestamp.micros / 1e6).strftime("%Y-%m-%d %H:%M:%S")
                 elif type == "rfc":
                     plant[key] = timestamp.to_rfc3339()
                 elif type == "proto":
                     plant[key] = timestamp.to_proto()
                 yield plant
-
-        self.value = self.out = self.get_out() | self._name() >> beam.Map(
-            lambda plant: self.window.TimestampedValue(plant, plant[key] if key and plant.get(key) else time.time())
-        ) | self._name() >> beam.ParDo(GetTimestamp(key=key))
+        if self.data_type == 1:
+            self.value = self.out = self.get_out() | self._name() >> beam.Map(
+                lambda plant: self.window.TimestampedValue(plant, plant[key] if key and plant.get(key) else time.time())
+            ) | self._name() >> beam.ParDo(GetTimestamp(key=key))
+        else:
+            def get_plant(plant):
+                micros = plant[key] if key and plant.get(key) else time.time()
+                micros = int(int(float(micros)) / (10 ** (len(str(int(float(micros))))-10)))
+                plant[key] = datetime.datetime.fromtimestamp(micros).strftime("%Y-%m-%d %H:%M:%S")
+                return plant
+            self.value = self.out = self.get_out() | beam.Map(lambda plant: get_plant(plant))
         return self
 
     def kvswap(self, data=None):
         """获取一个键值对集合并返回一个键值对集合，其中每个键值对都进行了交换。"""
         self.value = self.create(data).value | self._name() >> beam.KvSwap()
         if not (data and self.data):
             self.out = self.value
```

### Comparing `huhangkai-1.2.3/commen/unit_dict.py` & `huhangkai-1.2.4/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/unit_encryption.py` & `huhangkai-1.2.4/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/unit_fun.py` & `huhangkai-1.2.4/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/unit_logger.py` & `huhangkai-1.2.4/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/unit_request.py` & `huhangkai-1.2.4/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/commen/unit_tasks.py` & `huhangkai-1.2.4/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.3/setup.py` & `huhangkai-1.2.4/commen/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.2.3',  # 版本号
+    version='1.2.4',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
-    package_data={'by': ['常用命令.bat'],},
+    package_data={'by': ['常用命令.py'],},
+    include_package_data=True,
     python_requires=">=3.0",
     install_requires=[
         "faker",
         "openpyxl",
         "apscheduler",
         "rsa",
         "pyDes",
         "pycryptodome",
         "xlsxwriter",
         "pandas",
         "apache-beam",
         "pytest",
     ],
-)
+)
```


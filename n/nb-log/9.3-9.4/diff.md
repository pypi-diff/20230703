# Comparing `tmp/nb_log-9.3.tar.gz` & `tmp/nb_log-9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-9.3.tar", last modified: Mon Jul  3 10:55:48 2023, max compression
+gzip compressed data, was "nb_log-9.4.tar", last modified: Mon Jul  3 14:51:35 2023, max compression
```

## Comparing `nb_log-9.3.tar` & `nb_log-9.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:55:48.000000 nb_log-9.3/
--rw-rw-rw-   0        0        0    30397 2023-07-03 10:55:48.000000 nb_log-9.3/PKG-INFO
--rw-rw-rw-   0        0        0    29460 2023-07-03 03:00:00.000000 nb_log-9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 10:55:48.000000 nb_log-9.3/nb_log/
--rw-rw-rw-   0        0        0     3192 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-07-03 10:45:14.000000 nb_log-9.3/nb_log/file_write.py
--rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-9.3/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-9.3/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    30839 2023-06-29 11:11:21.000000 nb_log-9.3/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     6409 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0      853 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/monkey_std_filter_words.py
--rw-rw-rw-   0        0        0      819 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/monkey_sys_std.py
--rw-rw-rw-   0        0        0    10515 2023-07-03 03:00:00.000000 nb_log-9.3/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     4328 2023-06-30 01:44:40.000000 nb_log-9.3/nb_log/nb_logger.py
--rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-9.3/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:55:48.000000 nb_log-9.3/nb_log.egg-info/
--rw-rw-rw-   0        0        0    30397 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 10:55:48.000000 nb_log-9.3/setup.cfg
--rw-rw-rw-   0        0        0     2376 2023-07-03 10:55:38.000000 nb_log-9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:51:35.779836 nb_log-9.4/
+-rw-rw-rw-   0        0        0    30393 2023-07-03 14:51:35.776835 nb_log-9.4/PKG-INFO
+-rw-rw-rw-   0        0        0    29460 2023-07-03 13:46:53.000000 nb_log-9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 14:51:35.749828 nb_log-9.4/nb_log/
+-rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.4/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     2981 2023-07-03 14:43:01.000000 nb_log-9.4/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    50714 2023-07-03 14:15:08.000000 nb_log-9.4/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.4/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    30839 2023-07-03 14:18:09.000000 nb_log-9.4/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6409 2023-07-02 07:15:56.000000 nb_log-9.4/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.4/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0      819 2023-07-02 07:15:56.000000 nb_log-9.4/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10586 2023-07-03 14:31:09.000000 nb_log-9.4/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     4328 2023-06-30 14:23:45.000000 nb_log-9.4/nb_log/nb_logger.py
+-rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.4/nb_log/set_nb_log_config.py
+-rw-rw-rw-   0        0        0     1854 2023-07-03 14:03:16.000000 nb_log-9.4/nb_log/simple_print.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:51:35.772836 nb_log-9.4/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    30393 2023-07-03 14:51:35.000000 nb_log-9.4/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-03 14:51:35.000000 nb_log-9.4/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:51:35.000000 nb_log-9.4/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-07-03 14:51:35.000000 nb_log-9.4/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 14:51:35.000000 nb_log-9.4/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:51:35.780934 nb_log-9.4/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-03 14:51:32.000000 nb_log-9.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nb_log-9.3/PKG-INFO` & `nb_log-9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 9.3
+Version: 9.4
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -527,9 +527,7 @@
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
 
 <div> </div>
-
-
```

### Comparing `nb_log-9.3/README.md` & `nb_log-9.4/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/__init__.py` & `nb_log-9.4/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/file_write.py` & `nb_log-9.4/nb_log/file_write.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 from functools import wraps
 from pathlib import Path
 from nb_log import nb_log_config_default
 import time
 from chained_mode_time_tool import DatetimeConverter
-
+from nb_log.simple_print import sprint
 
 def singleton(cls):
     """
     单例模式装饰器,新加入线程锁，更牢固的单例模式，主要解决多线程如100线程同时实例化情况下可能会出现三例四例的情况,实测。
     """
     _instance = {}
     singleton.__lock = threading.Lock()  # 这里直接演示了线程安全版单例模式
@@ -22,20 +22,23 @@
 
     return _singleton
 
 
 # @singleton
 class FileWritter:
     _lock = threading.Lock()
-    need_write_2_file = False
+    need_write_2_file = True
 
-    def __init__(self, file_name: str,log_path=nb_log_config_default.LOG_PATH):
+    def __init__(self, file_name: str, log_path=nb_log_config_default.LOG_PATH):
         if self.need_write_2_file:
             self._file_name = file_name
-            Path(log_path).mkdir(exist_ok=True)
+            self.log_path = log_path
+            if not Path(self.log_path).exists():
+                sprint(f'自动创建日志文件夹 {log_path}')
+                Path(self.log_path).mkdir(exist_ok=True)
             self.file_path = Path(log_path) / Path(DatetimeConverter().date_str + '.' + file_name)
             self._open_file()
             self._last_write_ts = time.time()
             self._last_del_old_files_ts = time.time()
 
     def _open_file(self):
         self._f = open(self.file_path, encoding='utf8', mode='a')
@@ -55,17 +58,17 @@
                 self._f.flush()
                 if now_ts - self._last_del_old_files_ts > 300:
                     self._last_del_old_files_ts = time.time()
                     self._delete_old_files()
 
     def _delete_old_files(self):
         for i in range(10, 100):
-            file_path = Path(nb_log_config_default.LOG_PATH) / Path(DatetimeConverter(time.time() - 86400 * i).date_str + '.' + self._file_name)
+            file_path = Path(self.log_path) / Path(DatetimeConverter(time.time() - 86400 * i).date_str + '.' + self._file_name)
             try:
-                file_path.unlink()  # 低版本python 没有missing_ok入参。
+                file_path.unlink()
             except FileNotFoundError:
                 pass
 
 
 class PrintFileWritter(FileWritter):
     _lock = threading.Lock()
     need_write_2_file = False if nb_log_config_default.PRINT_WRTIE_FILE_NAME in (None, '') else True
@@ -73,10 +76,8 @@
 
 class StdFileWritter(FileWritter):
     _lock = threading.Lock()
     need_write_2_file = False if nb_log_config_default.SYS_STD_FILE_NAME in (None, '') else True
 
 
 if __name__ == '__main__':
-    fw = StdFileWritter('testfile',log_path='/pythonlogs333')
-    fw.write_2_file('哈哈哈')
-    fw._delete_old_files()
+    FileWritter('test_file', '/test_dir2').write_2_file('哈哈哈')
```

### Comparing `nb_log-9.3/nb_log/handlers.py` & `nb_log-9.4/nb_log/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from queue import Queue, Empty
 # noinspection PyPackageRequirements
 from kafka import KafkaProducer
 # from elasticsearch import Elasticsearch, helpers  # 性能导入时间消耗2秒,实例化时候再导入。
 from threading import Lock, Thread
 import pymongo
+from elasticsearch import Elasticsearch
 import requests
 import logging
 from logging import handlers
 from concurrent_log_handler import ConcurrentRotatingFileHandler  # 需要安装。concurrent-log-handler==0.9.1
 # noinspection PyUnresolvedReferences
 from logging.handlers import WatchedFileHandler
 # noinspection PyPackageRequirements
@@ -326,15 +327,15 @@
     def __init__(self, elastic_hosts: list, elastic_port, index_prefix='pylog-'):
         """
         :param elastic_hosts:  es的ip地址，数组类型
         :param elastic_port：  es端口
         :param index_prefix: index名字前缀。
         """
         logging.Handler.__init__(self)
-        self._es_client = Elasticsearch(elastic_hosts, port=elastic_port)
+        self._es_client = Elasticsearch(elastic_hosts,)
         self._index_prefix = index_prefix
         t = Thread(target=self._do_bulk_op)
         t.setDaemon(True)
         t.start()
 
     @classmethod
     def __add_task_to_bulk(cls, task):
```

### Comparing `nb_log-9.3/nb_log/handlers0000.py` & `nb_log-9.4/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/log_manager.py` & `nb_log-9.4/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/monkey_print.py` & `nb_log-9.4/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/monkey_std_filter_words.py` & `nb_log-9.4/nb_log/monkey_std_filter_words.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/monkey_sys_std.py` & `nb_log-9.4/nb_log/monkey_sys_std.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log/nb_log_config_default.py` & `nb_log-9.4/nb_log/nb_log_config_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf8
 """
 此文件nb_log_config.py是自动生成到python项目的根目录的。
-在这里面写的变量会覆盖此文件nb_log_config_default中的值。对nb_log包进行默认的配置。
+在这里面写的变量会覆盖此文件nb_log_config_default中的值。对nb_log包进行默认的配置。用户是无需修改nb_log安装包位置里面的配置文件的。
+
 但最终配置方式是由get_logger_and_add_handlers方法的各种传参决定，如果方法相应的传参为None则使用这里面的配置。
 """
 
 """
 如果反对日志有各种彩色，可以设置 DEFAULUT_USE_COLOR_HANDLER = False
 如果反对日志有块状背景彩色，可以设置 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = False
 如果想屏蔽nb_log包对怎么设置pycahrm的颜色的提示，可以设置 WARNING_PYCHARM_COLOR_SETINGS = False
```

### Comparing `nb_log-9.3/nb_log/nb_logger.py` & `nb_log-9.4/nb_log/nb_logger.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.3/nb_log.egg-info/PKG-INFO` & `nb_log-9.4/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 9.3
+Version: 9.4
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -527,9 +527,7 @@
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
 
 <div> </div>
-
-
```

### Comparing `nb_log-9.3/setup.py` & `nb_log-9.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="9.3",
+    version="9.4",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -63,14 +63,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-9.3.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.4.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```


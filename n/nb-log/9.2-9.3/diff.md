# Comparing `tmp/nb_log-9.2.tar.gz` & `tmp/nb_log-9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_log-9.2.tar", last modified: Mon Jul  3 06:49:24 2023, max compression
+gzip compressed data, was "dist\nb_log-9.3.tar", last modified: Mon Jul  3 10:55:48 2023, max compression
```

## Comparing `nb_log-9.2.tar` & `nb_log-9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:49:24.000000 nb_log-9.2/
--rw-rw-rw-   0        0        0    30397 2023-07-03 06:49:24.000000 nb_log-9.2/PKG-INFO
--rw-rw-rw-   0        0        0    29460 2023-07-03 03:00:00.000000 nb_log-9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 06:49:24.000000 nb_log-9.2/nb_log/
--rw-rw-rw-   0        0        0     3192 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/__init__.py
--rw-rw-rw-   0        0        0     2838 2023-07-03 06:48:38.000000 nb_log-9.2/nb_log/file_write.py
--rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-9.2/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-9.2/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    30839 2023-06-29 11:11:21.000000 nb_log-9.2/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     6409 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0      853 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/monkey_std_filter_words.py
--rw-rw-rw-   0        0        0      819 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/monkey_sys_std.py
--rw-rw-rw-   0        0        0    10515 2023-07-03 03:00:00.000000 nb_log-9.2/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     4328 2023-06-30 01:44:40.000000 nb_log-9.2/nb_log/nb_logger.py
--rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-9.2/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:49:24.000000 nb_log-9.2/nb_log.egg-info/
--rw-rw-rw-   0        0        0    30397 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 06:49:24.000000 nb_log-9.2/setup.cfg
--rw-rw-rw-   0        0        0     2376 2023-07-03 06:49:18.000000 nb_log-9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:55:48.000000 nb_log-9.3/
+-rw-rw-rw-   0        0        0    30397 2023-07-03 10:55:48.000000 nb_log-9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    29460 2023-07-03 03:00:00.000000 nb_log-9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 10:55:48.000000 nb_log-9.3/nb_log/
+-rw-rw-rw-   0        0        0     3192 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     2896 2023-07-03 10:45:14.000000 nb_log-9.3/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-9.3/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-9.3/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    30839 2023-06-29 11:11:21.000000 nb_log-9.3/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6409 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0      819 2023-07-03 02:35:14.000000 nb_log-9.3/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10515 2023-07-03 03:00:00.000000 nb_log-9.3/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     4328 2023-06-30 01:44:40.000000 nb_log-9.3/nb_log/nb_logger.py
+-rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-9.3/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:55:48.000000 nb_log-9.3/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    30397 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 10:55:47.000000 nb_log-9.3/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:55:48.000000 nb_log-9.3/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-03 10:55:38.000000 nb_log-9.3/setup.py
```

### Comparing `nb_log-9.2/PKG-INFO` & `nb_log-9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 9.2
+Version: 9.3
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-9.2/README.md` & `nb_log-9.3/README.md`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/__init__.py` & `nb_log-9.3/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/file_write.py` & `nb_log-9.3/nb_log/file_write.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 
 
 # @singleton
 class FileWritter:
     _lock = threading.Lock()
     need_write_2_file = False
 
-    def __init__(self, file_name: str):
+    def __init__(self, file_name: str,log_path=nb_log_config_default.LOG_PATH):
         if self.need_write_2_file:
             self._file_name = file_name
-            self.file_path = Path(nb_log_config_default.LOG_PATH) / Path(DatetimeConverter().date_str + '.' + file_name)
+            Path(log_path).mkdir(exist_ok=True)
+            self.file_path = Path(log_path) / Path(DatetimeConverter().date_str + '.' + file_name)
             self._open_file()
             self._last_write_ts = time.time()
             self._last_del_old_files_ts = time.time()
 
     def _open_file(self):
         self._f = open(self.file_path, encoding='utf8', mode='a')
 
@@ -71,12 +72,11 @@
 
 
 class StdFileWritter(FileWritter):
     _lock = threading.Lock()
     need_write_2_file = False if nb_log_config_default.SYS_STD_FILE_NAME in (None, '') else True
 
 
-
 if __name__ == '__main__':
-    fw = StdFileWritter(nb_log_config_default.PRINT_WRTIE_FILE_NAME)
+    fw = StdFileWritter('testfile',log_path='/pythonlogs333')
     fw.write_2_file('哈哈哈')
     fw._delete_old_files()
```

### Comparing `nb_log-9.2/nb_log/handlers.py` & `nb_log-9.3/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/handlers0000.py` & `nb_log-9.3/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/log_manager.py` & `nb_log-9.3/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/monkey_print.py` & `nb_log-9.3/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/monkey_std_filter_words.py` & `nb_log-9.3/nb_log/monkey_std_filter_words.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/monkey_sys_std.py` & `nb_log-9.3/nb_log/monkey_sys_std.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/nb_log_config_default.py` & `nb_log-9.3/nb_log/nb_log_config_default.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/nb_logger.py` & `nb_log-9.3/nb_log/nb_logger.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log/set_nb_log_config.py` & `nb_log-9.3/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.2/nb_log.egg-info/PKG-INFO` & `nb_log-9.3/nb_log.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 9.2
+Version: 9.3
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `nb_log-9.2/setup.py` & `nb_log-9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="9.2",
+    version="9.3",
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
-python setup.py sdist & python -m  twine upload dist/nb_log-9.2.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.3.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```


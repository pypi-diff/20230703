# Comparing `tmp/LogTranslate-1.2.1.tar.gz` & `tmp/LogTranslate-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.2.1.tar", last modified: Fri Jun 30 11:22:28 2023, max compression
+gzip compressed data, was "LogTranslate-1.2.2.tar", last modified: Mon Jul  3 13:32:32 2023, max compression
```

## Comparing `LogTranslate-1.2.1.tar` & `LogTranslate-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:22:28.881977 LogTranslate-1.2.1/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 11:22:28.861039 LogTranslate-1.2.1/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3183 2023-06-30 11:22:28.000000 LogTranslate-1.2.1/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-06-30 11:22:28.000000 LogTranslate-1.2.1/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:22:28.000000 LogTranslate-1.2.1/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-30 11:22:28.000000 LogTranslate-1.2.1/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 11:22:28.000000 LogTranslate-1.2.1/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3183 2023-06-30 11:22:28.880525 LogTranslate-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 11:22:28.872664 LogTranslate-1.2.1/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:22:28.877367 LogTranslate-1.2.1/log_translate/business/
--rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.1/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/config_default.py
--rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/data_struct.py
--rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/gloable.py
--rw-rw-rw-   0        0        0     4443 2023-06-29 14:49:11.000000 LogTranslate-1.2.1/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:22:28.878364 LogTranslate-1.2.1/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     7386 2023-06-29 14:53:32.000000 LogTranslate-1.2.1/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7374 2023-06-29 14:53:32.000000 LogTranslate-1.2.1/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 11:22:28.881977 LogTranslate-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2199 2023-06-30 11:22:23.000000 LogTranslate-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.297102 LogTranslate-1.2.2/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.272016 LogTranslate-1.2.2/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3183 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-03 13:32:32.000000 LogTranslate-1.2.2/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3183 2023-07-03 13:32:32.296104 LogTranslate-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.285707 LogTranslate-1.2.2/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.291121 LogTranslate-1.2.2/log_translate/business/
+-rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.2/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.2/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:32:32.293114 LogTranslate-1.2.2/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     7386 2023-06-29 14:53:32.000000 LogTranslate-1.2.2/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7374 2023-06-29 14:53:32.000000 LogTranslate-1.2.2/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 13:32:32.297102 LogTranslate-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2199 2023-07-03 13:32:14.000000 LogTranslate-1.2.2/setup.py
```

### Comparing `LogTranslate-1.2.1/LICENSE.txt` & `LogTranslate-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.2.2/LogTranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.1/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.2.2/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/PKG-INFO` & `LogTranslate-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.1/README.md` & `LogTranslate-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.2.2/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.2.2/log_translate/business/bluetooth_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/data_struct.py` & `LogTranslate-1.2.2/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/log_translator.py` & `LogTranslate-1.2.2/log_translate/log_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def __init__(self, father, tag_from_str_fun, tag_translators):
         super().__init__({
             father: self.translate_sub_tag
         })
         self.tag_from_str_fun = tag_from_str_fun
         self.tag_translators = tag_translators
 
-    def translate_sub_tag(self, msg):
+    def translate_sub_tag(self, tag, msg):
         log = self.tag_from_str_fun(msg)
         if log:
             sec_tag = log.group("tag")
             sec_msg = log.group("msg")
             for translator in self.tag_translators:
                 result = translator.translate(sec_tag, sec_msg)
                 if result:
```

### Comparing `LogTranslate-1.2.1/log_translate/read_log_file.py` & `LogTranslate-1.2.2/log_translate/read_log_file.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/res/log_logo.ico` & `LogTranslate-1.2.2/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/ui_pyqt6.py` & `LogTranslate-1.2.2/log_translate/ui_pyqt6.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/log_translate/ui_pyside2.py` & `LogTranslate-1.2.2/log_translate/ui_pyside2.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.1/setup.py` & `LogTranslate-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
 ICON_PATH = 'res/*.ico'
 
 setup(
     name='LogTranslate',
-    version='1.2.1',
+    version='1.2.2',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
```


# Comparing `tmp/processingtools-0.3.1.tar.gz` & `tmp/processingtools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\processingtools-0.3.1.tar", last modified: Mon Jun 26 12:31:16 2023, max compression
+gzip compressed data, was "dist\processingtools-0.3.2.tar", last modified: Mon Jul  3 11:23:32 2023, max compression
```

## Comparing `processingtools-0.3.1.tar` & `processingtools-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 12:31:16.225997 processingtools-0.3.1/
--rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1800 2023-06-26 12:31:16.225997 processingtools-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 12:31:16.216997 processingtools-0.3.1/ProcessingTools/
--rw-rw-rw-   0        0        0     7903 2023-06-26 12:30:59.000000 processingtools-0.3.1/ProcessingTools/EnvReco.py
--rw-rw-rw-   0        0        0     4347 2023-06-21 11:29:03.000000 processingtools-0.3.1/ProcessingTools/PrgressBar.py
--rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.1/ProcessingTools/__init__.py
--rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.1/ProcessingTools/functions.py
--rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.1/ProcessingTools/torch_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-26 12:31:16.214997 processingtools-0.3.1/ProcessingTools.egg-info/
--rw-rw-rw-   0        0        0     1800 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-26 12:31:15.000000 processingtools-0.3.1/ProcessingTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1321 2023-06-26 12:30:59.000000 processingtools-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 12:31:16.225997 processingtools-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-06-26 12:30:59.000000 processingtools-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:23:32.938592 processingtools-0.3.2/
+-rw-rw-rw-   0        0        0     1085 2022-04-02 13:28:58.000000 processingtools-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2667 2023-07-03 11:23:32.937593 processingtools-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 11:23:32.928592 processingtools-0.3.2/ProcessingTools/
+-rw-rw-rw-   0        0        0     8085 2023-07-03 11:22:43.000000 processingtools-0.3.2/ProcessingTools/EnvReco.py
+-rw-rw-rw-   0        0        0     4566 2023-07-03 11:22:43.000000 processingtools-0.3.2/ProcessingTools/PrgressBar.py
+-rw-rw-rw-   0        0        0      122 2023-06-23 14:29:11.000000 processingtools-0.3.2/ProcessingTools/__init__.py
+-rw-rw-rw-   0        0        0     8357 2023-06-14 13:17:42.000000 processingtools-0.3.2/ProcessingTools/functions.py
+-rw-rw-rw-   0        0        0    16364 2023-06-23 16:05:03.000000 processingtools-0.3.2/ProcessingTools/torch_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:23:32.926592 processingtools-0.3.2/ProcessingTools.egg-info/
+-rw-rw-rw-   0        0        0     2667 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 11:23:32.000000 processingtools-0.3.2/ProcessingTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2190 2023-07-03 11:22:43.000000 processingtools-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 11:23:32.938592 processingtools-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-07-03 11:22:43.000000 processingtools-0.3.2/setup.py
```

### Comparing `processingtools-0.3.1/LICENSE` & `processingtools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.1/PKG-INFO` & `processingtools-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,94 @@
-Metadata-Version: 2.1
-Name: processingtools
-Version: 0.3.1
-Summary: https://github.com/ysy9997/ProcessingTools.git
-Home-page: https://github.com/ysy9997/ProcessingTools.git
-Author: syy
-Author-email: ysy9997@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Python 3.6](https://img.shields.io/badge/python-3.6-green.svg)
 
 [![PyPI version](https://badge.fury.io/py/ProcessingTools.svg)](https://badge.fury.io/py/ProcessingTools)
 [![Downloads](https://pepy.tech/badge/processingtools)](https://pepy.tech/project/processingtools)
 
 # ProcessionTools
 
 - You can install this package using pip. 
 
 ```pip install processingtools```
 
-## usage
+## ProgressBar
 
 ```
 import processingtools as pt
 import time
 
+
 for i in pt.ProgressBar(range(50)):
     time.sleep(0.1)
 ```
 or
 ```
 import processingtools as pt
 import time
 
+
 for i in pt.ProgressBar(range(50), bar_length=40, start_mark=None, finish_mark='progress done!', total=False):
     time.sleep(0.1)
 ```
 Then, 
 ```
 |████████████████████████████████████████| 100.0% | 50/50 | 0s |  
 progress finished!(5311ms)
 ```
 
 ### parameters
-**class**　pt.ProgressBar(*in_loop, bar_length: int = 40, start_mark: str = None, finish_mark='progress done!', max=False*)
+**class**　pt.ProgressBar(*in_loop, bar_length: int = 40, start_mark: str = None, finish_mark='progress done!', total: int = None, detail_func: callable = None*)
 
 - **in_loop**: the input loop
 - **bar_length**: bar length
 - **start_mark**: print string when the progress start
 - **finish_mark**: print string what you want when progress finish
-- **max**: max value. If you do not fill this, it will calculate automatically, but it may be slow
+- **total**: total value. If you do not fill this, it will calculate automatically, but it may be slow
+- **detail_func**: write detail using detail_func
+- **remove_last**: If True, remove last progressbar
+
+
+## EnvRecoder
+```
+import processingtools as pt
+import argparse
+
+
+parser = argparse.ArgumentParser()
+parser.add_argument('--save_path', type=str)
+args = parser.parse_args()
+
+recoder = pt.EnvReco('/save/path')
+
+args = recoder.arg2abs(args)
+recoder.record_arg(args)
+recoder.record_code()
+recoder.record_os()
+recoder.record_gpu()
+recoder.put_space()
+recoder.print('record logs')
+```
+
+Then, record information in the log file
+```commandline
+Args: 
+{
+    save_path: None
+}
+
+OS Env: 
+{
+    ALLUSERSPROFILE: ...
+    APPDATA: ...
+    COMMONPROGRAMFILES: ...
+    ⋮
+}
+
+GPU Info: 
+{
+    cuda: True
+    num: 1
+    names: ['...']
+}
+
+[2023-7-3 19:50:9.78]: record logs
+
+```
```

### Comparing `processingtools-0.3.1/ProcessingTools/EnvReco.py` & `processingtools-0.3.2/ProcessingTools/EnvReco.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,28 +154,30 @@
 
         self.log_dict(gpu, keys, print_console)
         self.gpu = gpu
 
         return self.gpu
 
     @file_opener
-    def print(self, log: str) -> True:
+    def print(self, log: str, console: bool = True, file: bool = True) -> None:
         """
         write and print log with present time
         :param log: log
+        :param console: if True, print in the console
+        :param file: if True, write in the logs file
         return True
         """
 
         now = self.present.now()
-        print(f'\033[95m[{now.year}-{now.month}-{now.day} '
-              f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]\033[0m: {log}')
-        print(f'[{now.year}-{now.month}-{now.day} '
-              f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]: {log}', file=self.logs)
-
-        return True
+        if console:
+            print(f'\033[32m[{now.year}-{now.month}-{now.day} '
+                  f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]\033[0m: {log}')
+        if file:
+            print(f'[{now.year}-{now.month}-{now.day} '
+                  f'{now.hour}:{now.minute}:{now.second}.{round(now.microsecond / 10000):02d}]: {log}', file=self.logs)
 
     @file_opener
     def put_space(self, print_console: bool = True) -> bool:
         """
         insert space in the logs
         :param print_console: if True you can see logs in the console as well
         :return: True or False
```

### Comparing `processingtools-0.3.1/ProcessingTools/PrgressBar.py` & `processingtools-0.3.2/ProcessingTools/PrgressBar.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,36 +11,38 @@
     example:
         for x in ProgressBar(100)
         for x in ProgressBar(range(0, 100))
         for x in ProgressBar([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
     """
 
     def __init__(self, in_loop, bar_length: int = 40, start_mark: str = None, finish_mark='progress done!',
-                 max: int = None, total: int = None, detail_func: callable = None):
+                 max: int = None, total: int = None, detail_func: callable = None, remove_last: bool = False):
         """
         The initial function
         :param in_loop: the input loop
         :param bar_length: bar length
         :param start_mark: print string when the progress start
         :param finish_mark: print string what you want when progress finish
         :param total: total value. If you do not fill this, it will calculate automatically, but it may be slow
         :param detail_func: write detail using detail_func
+        :param remove_last: if True, remove progressbar when process is end
         """
 
         print(start_mark) if start_mark is not None else None
 
         self.take = np.zeros(10, float)
         T = time.time()
         for i in range(10): self.take[i] = T
 
         self.start = time.time() * 1000  # for the total take time
         self.bar_length = bar_length
         self.finish_mark = finish_mark
         self.index = 0
         self.detail_func = detail_func
+        self.remove_last = remove_last
 
         self.it = iter([i for i in range(in_loop)]) if type(in_loop) == int else iter(in_loop)
 
         if total: self.length = total
         elif max:
             warnings.warn('parameter max will be deprecated in the next version. Use total instead.')
             self.length = max
@@ -53,14 +55,16 @@
         return self
 
     def print_info(self, bar, space, progress_per_str, left, out, end=False):
         if self.detail_func and not end:
             print(f'\r\033[2K|{bar}{space}| \033[38;5;208m{progress_per_str}%\033[0m |'
                   f' \033[38;5;177m{self.index}/{self.length}\033[0m | \033[38;5;43m{left}\033[0m\033[0m |'
                   f' {self.detail_func(out)} |', end='')
+        elif end and self.remove_last:
+            print('\r', end='\r')
         else:
             print(f'\r\033[2K|{bar}{space}| \033[38;5;208m{progress_per_str}%\033[0m |'
                   f' \033[38;5;177m{self.index}/{self.length}\033[0m | \033[38;5;43m{left}\033[0m\033[0m |', end='')
 
     def __next__(self):
         """
         the iteration phase
```

### Comparing `processingtools-0.3.1/ProcessingTools/functions.py` & `processingtools-0.3.2/ProcessingTools/functions.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.1/ProcessingTools/torch_tools.py` & `processingtools-0.3.2/ProcessingTools/torch_tools.py`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.1/ProcessingTools.egg-info/SOURCES.txt` & `processingtools-0.3.2/ProcessingTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processingtools-0.3.1/setup.py` & `processingtools-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="processingtools",
-    version="0.3.1",
+    version="0.3.2",
     install_requires=['opencv-python>=4.5.5.62',
                       'numpy>=1.19.4',
                       'matplotlib>=3.3.3'],
     license='MIT',
     author="syy",
     author_email="ysy9997@gmail.com",
     description="https://github.com/ysy9997/ProcessingTools.git",
```


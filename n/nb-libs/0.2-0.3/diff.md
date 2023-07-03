# Comparing `tmp/nb_libs-0.2.tar.gz` & `tmp/nb_libs-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_libs-0.2.tar", last modified: Wed Mar 15 02:38:47 2023, max compression
+gzip compressed data, was "dist\nb_libs-0.3.tar", last modified: Mon Jul  3 07:49:13 2023, max compression
```

## Comparing `nb_libs-0.2.tar` & `nb_libs-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 02:38:47.000000 nb_libs-0.2/
--rw-rw-rw-   0        0        0      837 2023-03-15 02:38:47.000000 nb_libs-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-03-15 02:37:01.000000 nb_libs-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 02:38:47.000000 nb_libs-0.2/nb_libs.egg-info/
--rw-rw-rw-   0        0        0      837 2023-03-15 02:38:47.000000 nb_libs-0.2/nb_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-03-15 02:38:47.000000 nb_libs-0.2/nb_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 02:38:47.000000 nb_libs-0.2/nb_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-15 02:38:47.000000 nb_libs-0.2/nb_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 02:38:47.000000 nb_libs-0.2/nb_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 02:38:47.000000 nb_libs-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-03-15 02:38:39.000000 nb_libs-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 07:49:13.000000 nb_libs-0.3/
+-rw-rw-rw-   0        0        0     1212 2023-07-03 07:49:13.000000 nb_libs-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-03-15 02:45:38.000000 nb_libs-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 07:49:13.000000 nb_libs-0.3/nb_libs.egg-info/
+-rw-rw-rw-   0        0        0     1212 2023-07-03 07:49:12.000000 nb_libs-0.3/nb_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-07-03 07:49:12.000000 nb_libs-0.3/nb_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 07:49:12.000000 nb_libs-0.3/nb_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-03 07:49:12.000000 nb_libs-0.3/nb_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 07:49:12.000000 nb_libs-0.3/nb_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 07:49:13.000000 nb_libs-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2023-07-03 07:49:05.000000 nb_libs-0.3/setup.py
```

### Comparing `nb_libs-0.2/PKG-INFO` & `nb_libs-0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_libs
-Version: 0.2
+Version: 0.3
 Summary: nb_libs
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -24,9 +24,26 @@
 
 # 安装
 
 pip install nb_libs
 
 # 1. restart_program每隔多久重启代码自身。
 
+```python
+import time
+import datetime
+from nb_libs.restart_programe_by_interval import restart_program
+
+
+def _run():
+    print(datetime.datetime.now(), '开始运行程序')
+    for i in range(1000):
+        time.sleep(0.5)
+        print(datetime.datetime.now(), i)
+
+
+if __name__ == '__main__':
+    restart_program(10)  # 每隔10秒重启。
+    _run()
+```
```

### Comparing `nb_libs-0.2/nb_libs.egg-info/PKG-INFO` & `nb_libs-0.3/nb_libs.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-libs
-Version: 0.2
+Version: 0.3
 Summary: nb_libs
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -24,9 +24,26 @@
 
 # 安装
 
 pip install nb_libs
 
 # 1. restart_program每隔多久重启代码自身。
 
+```python
+import time
+import datetime
+from nb_libs.restart_programe_by_interval import restart_program
+
+
+def _run():
+    print(datetime.datetime.now(), '开始运行程序')
+    for i in range(1000):
+        time.sleep(0.5)
+        print(datetime.datetime.now(), i)
+
+
+if __name__ == '__main__':
+    restart_program(10)  # 每隔10秒重启。
+    _run()
+```
```

### Comparing `nb_libs-0.2/setup.py` & `nb_libs-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='nb_libs',  #
-    version="0.2",
+    version="0.3",
     description=('nb_libs'),
     keywords=["nb_libs",],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
@@ -35,20 +35,22 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: 3.6',
         'Topic :: Software Development :: Libraries'
     ],
     install_requires=[
         'nb_log',
+        'tzlocal',
+        'pytz',
     ]
 )
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
-python setup.py sdist & twine upload dist/nb_libs-0.2.tar.gz
+python setup.py sdist & twine upload dist/nb_libs-0.3.tar.gz
 twine upload dist/*
 
 
 python -m pip install mysql_pool --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```


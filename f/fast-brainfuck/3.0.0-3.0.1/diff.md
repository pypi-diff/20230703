# Comparing `tmp/fast-brainfuck-3.0.0.tar.gz` & `tmp/fast-brainfuck-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast-brainfuck-3.0.0.tar", last modified: Sat Jul  1 07:06:18 2023, max compression
+gzip compressed data, was "dist\fast-brainfuck-3.0.1.tar", last modified: Mon Jul  3 05:19:27 2023, max compression
```

## Comparing `fast-brainfuck-3.0.0.tar` & `fast-brainfuck-3.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:06:18.077971 fast-brainfuck-3.0.0/
--rw-rw-rw-   0        0        0     4255 2023-07-01 07:06:18.076969 fast-brainfuck-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2898 2023-07-01 07:05:46.000000 fast-brainfuck-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 07:06:18.076464 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/
--rw-rw-rw-   0        0        0     4255 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4733 2023-07-01 06:58:47.000000 fast-brainfuck-3.0.0/fastbf.py
--rw-rw-rw-   0        0        0       42 2023-07-01 07:06:18.077971 fast-brainfuck-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1189 2023-07-01 07:01:06.000000 fast-brainfuck-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 05:19:27.667045 fast-brainfuck-3.0.1/
+-rw-rw-rw-   0        0        0     4255 2023-07-03 05:19:27.666035 fast-brainfuck-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2898 2023-07-01 07:05:46.000000 fast-brainfuck-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 05:19:27.665030 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/
+-rw-rw-rw-   0        0        0     4255 2023-07-03 05:19:27.000000 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-03 05:19:27.000000 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 05:19:27.000000 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-03 05:19:27.000000 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-03 05:19:27.000000 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 05:19:27.000000 fast-brainfuck-3.0.1/fast_brainfuck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4733 2023-07-03 05:19:20.000000 fast-brainfuck-3.0.1/fastbf.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 05:19:27.667045 fast-brainfuck-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1189 2023-07-03 05:19:23.000000 fast-brainfuck-3.0.1/setup.py
```

### Comparing `fast-brainfuck-3.0.0/PKG-INFO` & `fast-brainfuck-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-brainfuck
-Version: 3.0.0
+Version: 3.0.1
 Summary: Brainfuck "compiler" for Python (fast)
 Home-page: https://github.com/none-None1/fast-bf
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         # A big bugfix is applied to this package due to the technique Python uses to import modules.
```

### Comparing `fast-brainfuck-3.0.0/README.md` & `fast-brainfuck-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fast-brainfuck-3.0.0/fast_brainfuck.egg-info/PKG-INFO` & `fast-brainfuck-3.0.1/fast_brainfuck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-brainfuck
-Version: 3.0.0
+Version: 3.0.1
 Summary: Brainfuck "compiler" for Python (fast)
 Home-page: https://github.com/none-None1/fast-bf
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         # A big bugfix is applied to this package due to the technique Python uses to import modules.
```

### Comparing `fast-brainfuck-3.0.0/fastbf.py` & `fast-brainfuck-3.0.1/fastbf.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,10 +144,10 @@
     ap.add_argument('-c','--cellsize',help='Number of cells, default is 300000.',default='300000')
     args=ap.parse_args()
     with open(args.filename) as f:
         code=f.read()
     func=brainfuck_to_function(code,int(args.cellsize))
     func()
 __all__=['brainfuck_to_function','dist_brainfuck']
-__version__='2.0.9'
+__version__='3.0.1'
 if __name__=='__main__':
     _fastbf_inter()
```

### Comparing `fast-brainfuck-3.0.0/setup.py` & `fast-brainfuck-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 def readme():
     with open('README.md','r') as f:
         return f.read()
 setup(
     name='fast-brainfuck',
     py_modules=['fastbf'],
-    version='3.0.0',
+    version='3.0.1',
     entry_points={
         'console_scripts':[
             'fastbf=fastbf:_fastbf_inter'
         ]
     },
     description='Brainfuck "compiler" for Python (fast)',
     long_description=readme(),
```


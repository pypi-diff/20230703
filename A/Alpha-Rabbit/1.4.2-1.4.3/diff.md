# Comparing `tmp/Alpha_Rabbit-1.4.2.tar.gz` & `tmp/Alpha_Rabbit-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.4.2.tar", last modified: Mon Jul  3 02:12:44 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.4.3.tar", last modified: Mon Jul  3 02:14:49 2023, max compression
```

## Comparing `Alpha_Rabbit-1.4.2.tar` & `Alpha_Rabbit-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 02:12:44.095500 Alpha_Rabbit-1.4.2/
-drwxrwxrwx   0        0        0        0 2023-07-03 02:12:44.088195 Alpha_Rabbit-1.4.2/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    42314 2023-07-03 02:12:17.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-03 02:12:44.094509 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-07-03 02:12:43.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-07-03 02:12:43.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 02:12:43.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-03 02:12:43.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 02:12:43.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-07-03 02:12:44.095500 Alpha_Rabbit-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.2/README.md
--rw-rw-rw-   0        0        0       85 2023-07-03 02:12:44.095500 Alpha_Rabbit-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-07-03 02:12:27.000000 Alpha_Rabbit-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 02:14:49.067777 Alpha_Rabbit-1.4.3/
+drwxrwxrwx   0        0        0        0 2023-07-03 02:14:49.061931 Alpha_Rabbit-1.4.3/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    42315 2023-07-03 02:14:23.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-07-03 02:14:49.067777 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 02:14:49.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-07-03 02:14:49.068778 Alpha_Rabbit-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.3/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-03 02:14:49.068778 Alpha_Rabbit-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-07-03 02:14:32.000000 Alpha_Rabbit-1.4.3/setup.py
```

### Comparing `Alpha_Rabbit-1.4.2/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.4.3/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,15 @@
         xlist = ['circulation_A','beta']   
         # 不dropna会报错
         self.barrafactor[y[0]] = self.barrafactor[[y[0]]+xlist].dropna().groupby(level = 0, group_keys = False).apply(lambda x: orthog(x,y[0],xlist))
         self.barrafactor[y[1]] = self.barrafactor[[y[1]]+xlist[:1]].dropna().groupby(level = 0, group_keys = False).apply(lambda x: orthog(x,y[1],xlist[:1]))
         self.barrafactor[y[2]] = self.barrafactor[[y[2]]+xlist[:1]].dropna().groupby(level = 0, group_keys = False).apply(lambda x: orthog(x,y[2],xlist[:1]))
         # 标准化
     
-    def return_barra_factor(self,rank_normalize:bool)
+    def return_barra_factor(self,rank_normalize:bool):
         mft = multi_factor_test()
         if rank_normalize:
             return mft.mat_ranknormlize(self.barrafactor)
         else:
             return mft.mat_normlize(self.barrafactor)
 
     def barra_compose(self,factordata):
```

### Comparing `Alpha_Rabbit-1.4.2/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Calculator.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.2/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.4.3/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.2/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.4.3/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.2/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.4.3/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.4.2
+Version: 1.4.3
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.2/LICENSE.txt` & `Alpha_Rabbit-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.2/PKG-INFO` & `Alpha_Rabbit-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.4.2
+Version: 1.4.3
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.2/setup.py` & `Alpha_Rabbit-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.4.2",
+    version="1.4.3",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```


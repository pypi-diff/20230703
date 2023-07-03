# Comparing `tmp/ANBUtils-1.6.4.tar.gz` & `tmp/ANBUtils-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.6.4.tar", last modified: Mon Jun 26 08:04:37 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.6.5.tar", last modified: Mon Jul  3 10:33:18 2023, max compression
```

## Comparing `ANBUtils-1.6.4.tar` & `ANBUtils-1.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-26 08:04:37.237027 ANBUtils-1.6.4/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-26 08:04:37.235877 ANBUtils-1.6.4/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      817 2023-06-20 13:05:30.000000 ANBUtils-1.6.4/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-06-20 12:35:47.000000 ANBUtils-1.6.4/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    12409 2023-06-16 06:57:29.000000 ANBUtils-1.6.4/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.4/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      890 2023-06-13 10:59:29.000000 ANBUtils-1.6.4/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.4/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.4/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.4/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-26 08:04:37.236637 ANBUtils-1.6.4/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5286 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)      108 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5286 2023-06-26 08:04:37.236853 ANBUtils-1.6.4/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.4/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-26 08:04:37.237083 ANBUtils-1.6.4/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      844 2023-06-26 08:04:19.000000 ANBUtils-1.6.4/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-07-03 10:33:18.262606 ANBUtils-1.6.5/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-07-03 10:33:18.261445 ANBUtils-1.6.5/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      849 2023-07-03 10:31:48.000000 ANBUtils-1.6.5/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-06-20 12:35:47.000000 ANBUtils-1.6.5/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)    12407 2023-06-26 10:50:44.000000 ANBUtils-1.6.5/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.5/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1092 2023-07-03 10:30:53.000000 ANBUtils-1.6.5/ANBUtils/environ.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.5/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.5/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.5/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-07-03 10:33:18.262232 ANBUtils-1.6.5/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5286 2023-07-03 10:33:18.000000 ANBUtils-1.6.5/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      337 2023-07-03 10:33:18.000000 ANBUtils-1.6.5/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-07-03 10:33:18.000000 ANBUtils-1.6.5/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      108 2023-07-03 10:33:18.000000 ANBUtils-1.6.5/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-07-03 10:33:18.000000 ANBUtils-1.6.5/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5286 2023-07-03 10:33:18.262440 ANBUtils-1.6.5/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.5/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-07-03 10:33:18.262668 ANBUtils-1.6.5/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      844 2023-07-03 10:32:06.000000 ANBUtils-1.6.5/setup.py
```

### Comparing `ANBUtils-1.6.4/ANBUtils/__init__.py` & `ANBUtils-1.6.5/ANBUtils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
-from .environ_cheker import environment_checker as _checker
+from .environ import environment_checker as _checker
 _checker()
 
-
+from .environ import(
+    set_environ
+)
 
 from .a import (
     print_rate_progress, set_date_index, digit, count, value, count2int, data_browser
 )
 
 from .db_worker import (
     DBWorker, crawler_starter, log_db, read_log, dblink, dblink_add, dblink_remove, dblink_update, collection_show,
```

### Comparing `ANBUtils-1.6.4/ANBUtils/a.py` & `ANBUtils-1.6.5/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.4/ANBUtils/db_worker.py` & `ANBUtils-1.6.5/ANBUtils/db_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,16 +196,15 @@
             limit (int, optional): The maximum number of documents to return. Defaults to 0.
 
         Returns:
             pandas.DataFrame: The DataFrame created from the collection data.
         """
 
         if sort is None and skip == 0 and limit == 0:
-            return self._to_df_large( col, match, projection )
-
+            return self._to_df_large( col, match, projection)
         else:
             return self._to_df_base( col, match, projection, sort, skip, limit )
 
     def to_df_many(self, cols, match=None, projection=None):
         """
          Convert multiple collections into a single DataFrame.
```

### Comparing `ANBUtils-1.6.4/ANBUtils/easy_pickle.py` & `ANBUtils-1.6.5/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.4/ANBUtils/environ_cheker.py` & `ANBUtils-1.6.5/ANBUtils/environ.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import os
 import warnings
+import configparser
+
+def set_environ(f='config.ini'):
+    config = configparser.ConfigParser()
+    config.read( f )
+    for k in config['environ']:
+        os.environ[k.upper()] = config['environ'][k]
 
 
 def environment_checker():
     """
     检查环境变量是否设置。
 
     检查以下环境变量是否在系统环境变量中设置：
@@ -23,7 +30,8 @@
     for k in ['MONGODB_URL', 'MONGODB_PUB_URI', 'DINGTALK_WEBHOOK','QYWECHAT_WEBHOOK']:
         if k not in os.environ:
             if k == 'MONGODB_URL':
                 print('see <Setting Up DBWorker> https://second-cloche-446.notion.site/ANBUtils-Wiki-f3ba5d99b6904a56a3335aff927492ee' )
             warnings.warn( '\nPlease set %s in environment variable' % k )
 
 
+
```

### Comparing `ANBUtils-1.6.4/ANBUtils/id_work.py` & `ANBUtils-1.6.5/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.4/ANBUtils/messenger.py` & `ANBUtils-1.6.5/ANBUtils/messenger.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.4/ANBUtils/tbox.py` & `ANBUtils-1.6.5/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.4/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.6.5/ANBUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.4
+Version: 1.6.5
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ANBUtils-1.6.4/PKG-INFO` & `ANBUtils-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.4
+Version: 1.6.5
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ANBUtils-1.6.4/README.md` & `ANBUtils-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.4/setup.py` & `ANBUtils-1.6.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ANBUtils",
-    version='1.6.4',
+    version='1.6.5',
     packages=find_packages(),
     author='Yafei Hou',
     author_email='redbson@gmail.com',
     url= 'https://github.com/redbson/ANBUtils',
     description = "ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```


# Comparing `tmp/tibis-1.0.7.tar.gz` & `tmp/tibis-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibis-1.0.7.tar", max compression
+gzip compressed data, was "tibis-1.0.8.tar", max compression
```

## Comparing `tibis-1.0.7.tar` & `tibis-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.7/LICENSE
--rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.7/README.md
--rw-r--r--   0        0        0      517 2023-06-26 08:40:39.216624 tibis-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1582 2023-06-26 08:37:09.179153 tibis-1.0.7/tibis/lib/args_parser.py
--rw-r--r--   0        0        0     7881 2023-06-07 17:23:03.849883 tibis-1.0.7/tibis/lib/common.py
--rw-r--r--   0        0        0      542 2023-06-05 05:21:48.691631 tibis-1.0.7/tibis/lib/config.py
--rw-r--r--   0        0        0     2956 2022-11-15 15:00:41.092868 tibis-1.0.7/tibis/lib/create.py
--rw-r--r--   0        0        0      935 2022-05-04 07:11:06.355861 tibis-1.0.7/tibis/lib/delete.py
--rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.7/tibis/lib/first_time.py
--rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.7/tibis/lib/list.py
--rw-r--r--   0        0        0     1431 2023-06-05 07:02:14.055365 tibis-1.0.7/tibis/lib/lock.py
--rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.7/tibis/lib/logger.py
--rw-r--r--   0        0        0     1203 2023-06-26 08:40:28.923238 tibis-1.0.7/tibis/lib/static.py
--rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.7/tibis/lib/unlock.py
--rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.7/tibis/tibis.py
--rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 tibis-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.8/LICENSE
+-rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.8/README.md
+-rw-r--r--   0        0        0      517 2023-07-03 12:45:15.426787 tibis-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1582 2023-06-26 08:37:09.179153 tibis-1.0.8/tibis/lib/args_parser.py
+-rw-r--r--   0        0        0     7881 2023-07-03 12:44:33.559982 tibis-1.0.8/tibis/lib/common.py
+-rw-r--r--   0        0        0      632 2023-07-03 12:42:59.349671 tibis-1.0.8/tibis/lib/config.py
+-rw-r--r--   0        0        0     2956 2022-11-15 15:00:41.092868 tibis-1.0.8/tibis/lib/create.py
+-rw-r--r--   0        0        0      935 2022-05-04 07:11:06.355861 tibis-1.0.8/tibis/lib/delete.py
+-rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.8/tibis/lib/first_time.py
+-rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.8/tibis/lib/list.py
+-rw-r--r--   0        0        0     1431 2023-06-05 07:02:14.055365 tibis-1.0.8/tibis/lib/lock.py
+-rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.8/tibis/lib/logger.py
+-rw-r--r--   0        0        0     1203 2023-07-03 12:44:23.373282 tibis-1.0.8/tibis/lib/static.py
+-rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.8/tibis/lib/unlock.py
+-rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.8/tibis/tibis.py
+-rw-r--r--   0        0        0     4094 1970-01-01 00:00:00.000000 tibis-1.0.8/PKG-INFO
```

### Comparing `tibis-1.0.7/LICENSE` & `tibis-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/README.md` & `tibis-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/pyproject.toml` & `tibis-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibis"
-version = "1.0.7"
+version = "1.0.8"
 description = "Tibis is a secure storage manager"
 authors = ["shoxxdj <shoxx@shoxxdj.fr>"]
 readme = "README.md"
 homepage = "https://github.com/shoxxdj/tibis"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
```

### Comparing `tibis-1.0.7/tibis/lib/args_parser.py` & `tibis-1.0.8/tibis/lib/args_parser.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/common.py` & `tibis-1.0.8/tibis/lib/common.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/config.py` & `tibis-1.0.8/tibis/lib/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import yaml 
 import tibis.lib.static as static
+import sys
 
 def storage_path():
     with open(static.tibis_full_config_location) as file:
         p = yaml.load(file,Loader=yaml.FullLoader)
         return p['storage_path']
 
 def pgp_infos():
     with open(static.tibis_full_config_location) as file:
         p = yaml.load(file,Loader=yaml.FullLoader)
         return p['pgp_infos']
 
 def check_integrity_status():
     with open(static.tibis_full_config_location) as file:
         p = yaml.load(file,Loader=yaml.FullLoader)
-        return p['check_integrity']
+        if('check_integrity' in p ):
+            return p['check_integrity']
+        else:
+            return True
```

### Comparing `tibis-1.0.7/tibis/lib/create.py` & `tibis-1.0.8/tibis/lib/create.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/delete.py` & `tibis-1.0.8/tibis/lib/delete.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/first_time.py` & `tibis-1.0.8/tibis/lib/first_time.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/list.py` & `tibis-1.0.8/tibis/lib/list.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/lock.py` & `tibis-1.0.8/tibis/lib/lock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/logger.py` & `tibis-1.0.8/tibis/lib/logger.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/lib/static.py` & `tibis-1.0.8/tibis/lib/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-version  = '1.0.7'
+version  = '1.0.8'
 codename = "Ibis is born"
 
 tibis_config_file="config.yml"
 tibis_config_location=str(Path.home())+"/.config/tibis/"
 tibis_full_config_location=tibis_config_location+tibis_config_file
 
 tibis_keys_location=tibis_config_location+"keys"
```

### Comparing `tibis-1.0.7/tibis/lib/unlock.py` & `tibis-1.0.8/tibis/lib/unlock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/tibis/tibis.py` & `tibis-1.0.8/tibis/tibis.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.7/PKG-INFO` & `tibis-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibis
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tibis is a secure storage manager
 Home-page: https://github.com/shoxxdj/tibis
 Author: shoxxdj
 Author-email: shoxx@shoxxdj.fr
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```


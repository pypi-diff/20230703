# Comparing `tmp/afgutils-1.0.6.tar.gz` & `tmp/afgutils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afgutils-1.0.6.tar", last modified: Mon Jul  3 20:01:03 2023, max compression
+gzip compressed data, was "afgutils-1.0.7.tar", last modified: Mon Jul  3 20:34:10 2023, max compression
```

## Comparing `afgutils-1.0.6.tar` & `afgutils-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 20:01:03.074235 afgutils-1.0.6/
--rw-rw-rw-   0        0        0      224 2023-07-03 20:01:03.073237 afgutils-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 20:01:03.047230 afgutils-1.0.6/afgutils/
--rw-rw-rw-   0        0        0      264 2023-04-13 10:38:48.000000 afgutils-1.0.6/afgutils/__init__.py
--rw-rw-rw-   0        0        0      882 2023-05-04 15:08:56.000000 afgutils-1.0.6/afgutils/advanceai_util.py
--rw-rw-rw-   0        0        0     2634 2023-04-13 11:41:11.000000 afgutils-1.0.6/afgutils/credolab.py
--rw-rw-rw-   0        0        0     2950 2023-04-06 17:38:51.000000 afgutils-1.0.6/afgutils/db.py
--rw-rw-rw-   0        0        0      757 2023-04-06 17:33:13.000000 afgutils-1.0.6/afgutils/email.py
--rw-rw-rw-   0        0        0     1677 2023-04-13 11:41:11.000000 afgutils-1.0.6/afgutils/s3.py
--rw-rw-rw-   0        0        0     3903 2023-04-06 17:33:13.000000 afgutils-1.0.6/afgutils/trandata.py
--rw-rw-rw-   0        0        0     4241 2023-07-03 19:07:25.000000 afgutils-1.0.6/afgutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 20:01:03.071267 afgutils-1.0.6/afgutils.egg-info/
--rw-rw-rw-   0        0        0      224 2023-07-03 20:01:02.000000 afgutils-1.0.6/afgutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-03 20:01:02.000000 afgutils-1.0.6/afgutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 20:01:02.000000 afgutils-1.0.6/afgutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-03 20:01:02.000000 afgutils-1.0.6/afgutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 20:01:02.000000 afgutils-1.0.6/afgutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 20:01:03.074235 afgutils-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      633 2023-07-03 19:58:59.000000 afgutils-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:10.786712 afgutils-1.0.7/
+-rw-rw-rw-   0        0        0      224 2023-07-03 20:34:10.785710 afgutils-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:10.764711 afgutils-1.0.7/afgutils/
+-rw-rw-rw-   0        0        0      264 2023-04-13 10:38:48.000000 afgutils-1.0.7/afgutils/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-05-04 15:08:56.000000 afgutils-1.0.7/afgutils/advanceai_util.py
+-rw-rw-rw-   0        0        0     2634 2023-04-13 11:41:11.000000 afgutils-1.0.7/afgutils/credolab.py
+-rw-rw-rw-   0        0        0     2950 2023-04-06 17:38:51.000000 afgutils-1.0.7/afgutils/db.py
+-rw-rw-rw-   0        0        0      757 2023-04-06 17:33:13.000000 afgutils-1.0.7/afgutils/email.py
+-rw-rw-rw-   0        0        0     1677 2023-04-13 11:41:11.000000 afgutils-1.0.7/afgutils/s3.py
+-rw-rw-rw-   0        0        0     3903 2023-04-06 17:33:13.000000 afgutils-1.0.7/afgutils/trandata.py
+-rw-rw-rw-   0        0        0     4200 2023-07-03 20:31:04.000000 afgutils-1.0.7/afgutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 20:34:10.784711 afgutils-1.0.7/afgutils.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-03 20:34:10.000000 afgutils-1.0.7/afgutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:34:10.786712 afgutils-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      633 2023-07-03 20:33:44.000000 afgutils-1.0.7/setup.py
```

### Comparing `afgutils-1.0.6/afgutils/advanceai_util.py` & `afgutils-1.0.7/afgutils/advanceai_util.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.6/afgutils/credolab.py` & `afgutils-1.0.7/afgutils/credolab.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.6/afgutils/db.py` & `afgutils-1.0.7/afgutils/db.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.6/afgutils/email.py` & `afgutils-1.0.7/afgutils/email.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.6/afgutils/s3.py` & `afgutils-1.0.7/afgutils/s3.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.6/afgutils/trandata.py` & `afgutils-1.0.7/afgutils/trandata.py`

 * *Files identical despite different names*

### Comparing `afgutils-1.0.6/afgutils/utils.py` & `afgutils-1.0.7/afgutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,14 @@
         result_sql = column_names_insert_text
     else:
         raise TypeError("data_vector_to_sql_insert: insert_sql_tpl must be a string or None")
 
     return result_items, result_sql
 
 
-def _convert_string_to_boolean(s: str) -> bool:
-    if s.lower() in ('true', 't', '1', 'y', 'yes'):
+def _convert_string_to_boolean(s: str) -> bool | str:
+    if s.lower() == 'true':
         return True
-    elif s.lower() in ('false', 'f', '0', 'n', 'no'):
+    elif s.lower() == 'false':
         return False
     else:
         return s
```

### Comparing `afgutils-1.0.6/setup.py` & `afgutils-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 DESCRIPTION = 'Shared support functions'
 LONG_DESCRIPTION = 'Shared support functions'
 
 setup(
     name="afgutils",
     version=VERSION,
     description=DESCRIPTION,
```


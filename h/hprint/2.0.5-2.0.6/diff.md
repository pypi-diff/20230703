# Comparing `tmp/hprint-2.0.5.tar.gz` & `tmp/hprint-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hprint-2.0.5.tar", last modified: Wed May 17 10:00:12 2023, max compression
+gzip compressed data, was "hprint-2.0.6.tar", last modified: Mon Jul  3 08:49:53 2023, max compression
```

## Comparing `hprint-2.0.5.tar` & `hprint-2.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-05-17 10:00:12.783317 hprint-2.0.5/
--rw-r--r--   0 haoru      (501) staff       (20)     1065 2022-12-17 06:41:01.000000 hprint-2.0.5/LICENSE
--rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-05-17 10:00:12.783472 hprint-2.0.5/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)     4211 2022-12-24 13:51:04.000000 hprint-2.0.5/README.md
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-05-17 10:00:12.780314 hprint-2.0.5/hprint/
--rw-r--r--   0 haoru      (501) staff       (20)     5204 2023-04-15 04:09:13.000000 hprint-2.0.5/hprint/__init__.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-05-17 10:00:12.782779 hprint-2.0.5/hprint.egg-info/
--rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)      204 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/SOURCES.txt
--rw-r--r--   0 haoru      (501) staff       (20)        1 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/dependency_links.txt
--rw-r--r--   0 haoru      (501) staff       (20)        9 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/requires.txt
--rw-r--r--   0 haoru      (501) staff       (20)        7 2023-05-17 10:00:12.000000 hprint-2.0.5/hprint.egg-info/top_level.txt
--rw-r--r--   0 haoru      (501) staff       (20)      235 2023-05-17 10:00:12.784134 hprint-2.0.5/setup.cfg
--rw-r--r--   0 haoru      (501) staff       (20)     1506 2023-05-17 09:59:30.000000 hprint-2.0.5/setup.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-07-03 08:49:53.060536 hprint-2.0.6/
+-rw-r--r--   0 haoru      (501) staff       (20)     1065 2022-12-17 06:41:01.000000 hprint-2.0.6/LICENSE
+-rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-07-03 08:49:53.060658 hprint-2.0.6/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)     4211 2022-12-24 13:51:04.000000 hprint-2.0.6/README.md
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-07-03 08:49:53.058268 hprint-2.0.6/hprint/
+-rw-r--r--   0 haoru      (501) staff       (20)     5230 2023-07-03 07:22:22.000000 hprint-2.0.6/hprint/__init__.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-07-03 08:49:53.060234 hprint-2.0.6/hprint.egg-info/
+-rw-r--r--   0 haoru      (501) staff       (20)     5274 2023-07-03 08:49:53.000000 hprint-2.0.6/hprint.egg-info/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)      204 2023-07-03 08:49:53.000000 hprint-2.0.6/hprint.egg-info/SOURCES.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        1 2023-07-03 08:49:53.000000 hprint-2.0.6/hprint.egg-info/dependency_links.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        9 2023-07-03 08:49:53.000000 hprint-2.0.6/hprint.egg-info/requires.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        7 2023-07-03 08:49:53.000000 hprint-2.0.6/hprint.egg-info/top_level.txt
+-rw-r--r--   0 haoru      (501) staff       (20)      235 2023-07-03 08:49:53.061183 hprint-2.0.6/setup.cfg
+-rw-r--r--   0 haoru      (501) staff       (20)     1506 2023-07-03 08:48:38.000000 hprint-2.0.6/setup.py
```

### Comparing `hprint-2.0.5/LICENSE` & `hprint-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hprint-2.0.5/PKG-INFO` & `hprint-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hprint
-Version: 2.0.5
+Version: 2.0.6
 Summary: Print python object in table/json format
 Home-page: https://github.com/ruanhao/hprint
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: utils,print,json
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hprint-2.0.5/README.md` & `hprint-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hprint-2.0.5/hprint/__init__.py` & `hprint-2.0.6/hprint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 def _pprint(obj):
     _print(pformat(obj, indent=4))
 
 
 def json_print(data):
     if isinstance(data, dict):
-        _print(json.dumps(data, indent=4, sort_keys=True))
+        _print(json.dumps(data, indent=4, sort_keys=True, default=str))
     elif isinstance(data, list):
         try:
-            _print(json.dumps([dict(d) for d in data], indent=4, sort_keys=True))
+            _print(json.dumps([dict(d) for d in data], indent=4, sort_keys=True), default=str)
         except Exception:
             try:
                 _pprint([dict(d) for d in data])
             except Exception:
                 _pprint(data)
     else:
         _pprint(data)
```

### Comparing `hprint-2.0.5/hprint.egg-info/PKG-INFO` & `hprint-2.0.6/hprint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hprint
-Version: 2.0.5
+Version: 2.0.6
 Summary: Print python object in table/json format
 Home-page: https://github.com/ruanhao/hprint
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: utils,print,json
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hprint-2.0.5/setup.py` & `hprint-2.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'license': 'MIT',
     "long_description": long_description,
     "long_description_content_type": 'text/markdown',
     'description': 'Print python object in table/json format',
     'author' : 'Hao Ruan',
     'author_email': 'ruanhao1116@gmail.com',
     'keywords': ['utils', 'print', 'json'],
-    'version': '2.0.5',
+    'version': '2.0.6',
     'packages': ['hprint'],
     'install_requires': [
         'tabulate',
     ],
     'python_requires': ">=3.7, <4",
     'setup_requires': ['wheel'],
     'classifiers': [
```


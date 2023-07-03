# Comparing `tmp/flageval_serving-0.1.3.tar.gz` & `tmp/flageval_serving-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flageval_serving-0.1.3.tar", max compression
+gzip compressed data, was "flageval_serving-0.1.4.tar", max compression
```

## Comparing `flageval_serving-0.1.3.tar` & `flageval_serving-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.3/flageval/serving/__init__.py
--rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.3/flageval/serving/app.py
--rw-r--r--   0        0        0     3903 2023-06-05 00:31:36.366312 flageval_serving-0.1.3/flageval/serving/cli.py
--rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.3/flageval/serving/extensions.py
--rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.3/flageval/serving/finder.py
--rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.3/flageval/serving/flagenv.py
--rw-r--r--   0        0        0     4710 2023-06-05 06:43:26.434926 flageval_serving-0.1.3/flageval/serving/flageval.py
--rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.3/flageval/serving/guniconf.py
--rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.3/flageval/serving/service/__init__.py
--rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.3/flageval/serving/service/base.py
--rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.3/flageval/serving/service/demo_service.py
--rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.3/flageval/serving/service/guniconf.py
--rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.3/flageval/serving/service/nlp.py
--rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.3/flageval/serving/service/settings.py
--rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.3/flageval/serving/service/views.py
--rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.3/flageval/serving/signals.py
--rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.3/flageval/serving/util.py
--rw-r--r--   0        0        0      567 2023-06-05 06:46:25.845592 flageval_serving-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1289 2023-05-29 08:11:29.020506 flageval_serving-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 07:08:57.310781 flageval_serving-0.1.4/flageval/serving/__init__.py
+-rw-r--r--   0        0        0      791 2023-05-29 07:09:21.686007 flageval_serving-0.1.4/flageval/serving/app.py
+-rw-r--r--   0        0        0     3911 2023-07-03 11:16:59.833034 flageval_serving-0.1.4/flageval/serving/cli.py
+-rw-r--r--   0        0        0       26 2023-05-29 07:08:57.326678 flageval_serving-0.1.4/flageval/serving/extensions.py
+-rw-r--r--   0        0        0     2649 2023-05-23 13:32:07.184516 flageval_serving-0.1.4/flageval/serving/finder.py
+-rw-r--r--   0        0        0     2290 2023-05-29 07:09:33.651902 flageval_serving-0.1.4/flageval/serving/flagenv.py
+-rw-r--r--   0        0        0     4710 2023-06-05 06:43:26.434926 flageval_serving-0.1.4/flageval/serving/flageval.py
+-rw-r--r--   0        0        0     1973 2023-05-29 07:14:10.771889 flageval_serving-0.1.4/flageval/serving/guniconf.py
+-rw-r--r--   0        0        0      174 2023-05-23 13:32:07.186126 flageval_serving-0.1.4/flageval/serving/service/__init__.py
+-rw-r--r--   0        0        0      944 2023-05-23 13:32:07.186579 flageval_serving-0.1.4/flageval/serving/service/base.py
+-rw-r--r--   0        0        0      512 2023-05-23 13:32:07.187004 flageval_serving-0.1.4/flageval/serving/service/demo_service.py
+-rw-r--r--   0        0        0      336 2023-05-23 13:32:07.187325 flageval_serving-0.1.4/flageval/serving/service/guniconf.py
+-rw-r--r--   0        0        0     2344 2023-05-23 13:32:07.187853 flageval_serving-0.1.4/flageval/serving/service/nlp.py
+-rw-r--r--   0        0        0      265 2023-05-23 13:32:07.188185 flageval_serving-0.1.4/flageval/serving/service/settings.py
+-rw-r--r--   0        0        0      190 2023-05-23 13:32:07.188576 flageval_serving-0.1.4/flageval/serving/service/views.py
+-rw-r--r--   0        0        0      928 2023-05-29 07:10:10.100369 flageval_serving-0.1.4/flageval/serving/signals.py
+-rw-r--r--   0        0        0     2664 2023-05-29 07:08:57.342203 flageval_serving-0.1.4/flageval/serving/util.py
+-rw-r--r--   0        0        0      567 2023-07-03 11:20:15.072663 flageval_serving-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 flageval_serving-0.1.4/PKG-INFO
```

### Comparing `flageval_serving-0.1.3/README.md` & `flageval_serving-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/app.py` & `flageval_serving-0.1.4/flageval/serving/app.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/cli.py` & `flageval_serving-0.1.4/flageval/serving/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
     f = finder.get()
     settings.ENV = stage
     click.echo(f"[LOCAL] Merge ENV = {getattr(settings, 'ENV')}")
 
     try:
         for key, val in f.local_settings.__dict__.items():
             if not key.startswith("_") and key.isupper():
-                setattr(base, key, val)
-                click.echo(f"[LOCAL] Merge {key} = {getattr(base, key)}")
+                setattr(settings, key, val)
+                click.echo(f"[LOCAL] Merge {key} = {getattr(settings, key)}")
     except ImportError as e:
         click.echo(f"Merge local settings failed due to {e.args[0]}")
 
 
 def guess_project():
     if settings.DEFAULT_PROJECT_NAME != settings.PROJECT_NAME:
         return
```

### Comparing `flageval_serving-0.1.3/flageval/serving/finder.py` & `flageval_serving-0.1.4/flageval/serving/finder.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/flagenv.py` & `flageval_serving-0.1.4/flageval/serving/flagenv.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/flageval.py` & `flageval_serving-0.1.4/flageval/serving/flageval.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/guniconf.py` & `flageval_serving-0.1.4/flageval/serving/guniconf.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/service/base.py` & `flageval_serving-0.1.4/flageval/serving/service/base.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/service/demo_service.py` & `flageval_serving-0.1.4/flageval/serving/service/demo_service.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/service/nlp.py` & `flageval_serving-0.1.4/flageval/serving/service/nlp.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/signals.py` & `flageval_serving-0.1.4/flageval/serving/signals.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/flageval/serving/util.py` & `flageval_serving-0.1.4/flageval/serving/util.py`

 * *Files identical despite different names*

### Comparing `flageval_serving-0.1.3/pyproject.toml` & `flageval_serving-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flageval-serving"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["FlagEval <flageval@baai.ac.cn>"]
 readme = "README.md"
 packages = [{ include = "flageval" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `flageval_serving-0.1.3/PKG-INFO` & `flageval_serving-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flageval-serving
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: FlagEval
 Author-email: flageval@baai.ac.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/webexception-1.0.3.tar.gz` & `tmp/webexception-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexception-1.0.3.tar", max compression
+gzip compressed data, was "webexception-1.0.4.tar", max compression
```

## Comparing `webexception-1.0.3.tar` & `webexception-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6185 2023-06-20 15:11:48.458636 webexception-1.0.3/README.md
--rw-r--r--   0        0        0      566 2023-07-03 12:40:18.092931 webexception-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 15:13:03.845839 webexception-1.0.3/webexception/__init__.py
--rw-r--r--   0        0        0      740 2023-07-03 12:32:30.343680 webexception-1.0.3/webexception/webexception.py
--rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 webexception-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6185 2023-06-20 15:11:48.458636 webexception-1.0.4/README.md
+-rw-r--r--   0        0        0      566 2023-07-03 12:45:09.159457 webexception-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 15:13:03.845839 webexception-1.0.4/webexception/__init__.py
+-rw-r--r--   0        0        0      643 2023-07-03 12:45:03.967482 webexception-1.0.4/webexception/webexception.py
+-rw-r--r--   0        0        0     6478 1970-01-01 00:00:00.000000 webexception-1.0.4/PKG-INFO
```

### Comparing `webexception-1.0.3/README.md` & `webexception-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `webexception-1.0.3/pyproject.toml` & `webexception-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webexception"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `webexception-1.0.3/PKG-INFO` & `webexception-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexception
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```


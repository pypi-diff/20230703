# Comparing `tmp/rdfind2-0.0.8.tar.gz` & `tmp/rdfind2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.8.tar", max compression
+gzip compressed data, was "rdfind2-0.0.9.tar", max compression
```

## Comparing `rdfind2-0.0.8.tar` & `rdfind2-0.0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      411 2023-07-03 17:38:35.677176 rdfind2-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10716 2023-07-03 17:30:37.776172 rdfind2-0.0.8/rdfind2.py
--rw-r--r--   0        0        0      698 2023-07-03 17:30:37.776172 rdfind2-0.0.8/readme.md
--rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 rdfind2-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      415 2023-07-03 17:41:00.429816 rdfind2-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10716 2023-07-03 17:30:37.776172 rdfind2-0.0.9/rdfind2.py
+-rw-r--r--   0        0        0      698 2023-07-03 17:30:37.776172 rdfind2-0.0.9/readme.md
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 rdfind2-0.0.9/PKG-INFO
```

### Comparing `rdfind2-0.0.8/rdfind2.py` & `rdfind2-0.0.9/rdfind2.py`

 * *Files identical despite different names*

### Comparing `rdfind2-0.0.8/readme.md` & `rdfind2-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `rdfind2-0.0.8/PKG-INFO` & `rdfind2-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfind2
-Version: 0.0.8
+Version: 0.0.9
 Summary: Find duplicated files very fast
 License: MIT
 Author: trim21
 Author-email: trim21.me@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


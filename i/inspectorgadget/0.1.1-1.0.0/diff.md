# Comparing `tmp/inspectorgadget-0.1.1.tar.gz` & `tmp/inspectorgadget-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectorgadget-0.1.1.tar", max compression
+gzip compressed data, was "inspectorgadget-1.0.0.tar", max compression
```

## Comparing `inspectorgadget-0.1.1.tar` & `inspectorgadget-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/LICENSE
--rw-r--r--   0        0        0     1324 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/README.md
--rw-r--r--   0        0        0     4843 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/inspectorgadget/__init__.py
--rw-r--r--   0        0        0     2170 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 inspectorgadget-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1324 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/README.md
+-rw-r--r--   0        0        0     4843 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/inspectorgadget/__init__.py
+-rw-r--r--   0        0        0     2170 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 inspectorgadget-1.0.0/PKG-INFO
```

### Comparing `inspectorgadget-0.1.1/LICENSE` & `inspectorgadget-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inspectorgadget-0.1.1/README.md` & `inspectorgadget-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `inspectorgadget-0.1.1/inspectorgadget/__init__.py` & `inspectorgadget-1.0.0/inspectorgadget/__init__.py`

 * *Files identical despite different names*

### Comparing `inspectorgadget-0.1.1/pyproject.toml` & `inspectorgadget-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspectorgadget"
-version = "0.1.1"
+version = "1.0.0"
 description = "Inspector Gadget - Extended Python Inspection"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `inspectorgadget-0.1.1/PKG-INFO` & `inspectorgadget-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectorgadget
-Version: 0.1.1
+Version: 1.0.0
 Summary: Inspector Gadget - Extended Python Inspection
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


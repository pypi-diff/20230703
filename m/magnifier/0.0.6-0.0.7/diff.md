# Comparing `tmp/magnifier-0.0.6.tar.gz` & `tmp/magnifier-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnifier-0.0.6.tar", max compression
+gzip compressed data, was "magnifier-0.0.7.tar", max compression
```

## Comparing `magnifier-0.0.6.tar` & `magnifier-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2022-09-02 10:21:14.523868 magnifier-0.0.6/LICENSE
--rw-r--r--   0        0        0      151 2022-09-02 10:21:14.523868 magnifier-0.0.6/README.md
--rw-r--r--   0        0        0        0 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/__init__.py
--rw-r--r--   0        0        0      932 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/base.py
--rw-r--r--   0        0        0        0 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/evaluation/__init__.py
--rw-r--r--   0        0        0     1351 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/evaluation/classification.py
--rw-r--r--   0        0        0      413 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/io.py
--rw-r--r--   0        0        0     1614 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/model_experiment.py
--rw-r--r--   0        0        0        0 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/transformer/__init__.py
--rw-r--r--   0        0        0     2081 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/transformer/compressing.py
--rw-r--r--   0        0        0     6427 2022-09-02 10:21:14.523868 magnifier-0.0.6/magnifier/transformer/time_series.py
--rw-r--r--   0        0        0     1035 2022-09-02 10:21:31.459938 magnifier-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 magnifier-0.0.6/setup.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 magnifier-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 10:07:46.410694 magnifier-0.0.7/LICENSE
+-rw-r--r--   0        0        0      151 2023-07-03 10:07:46.410694 magnifier-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/base.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/evaluation/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/evaluation/classification.py
+-rw-r--r--   0        0        0      413 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/io.py
+-rw-r--r--   0        0        0     1614 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/model_experiment.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/transformer/__init__.py
+-rw-r--r--   0        0        0     2081 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/transformer/compressing.py
+-rw-r--r--   0        0        0      756 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/transformer/resampling.py
+-rw-r--r--   0        0        0     6427 2023-07-03 10:07:46.410694 magnifier-0.0.7/magnifier/transformer/time_series.py
+-rw-r--r--   0        0        0     1035 2023-07-03 10:08:06.611188 magnifier-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 magnifier-0.0.7/PKG-INFO
```

### Comparing `magnifier-0.0.6/LICENSE` & `magnifier-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `magnifier-0.0.6/magnifier/base.py` & `magnifier-0.0.7/magnifier/base.py`

 * *Files identical despite different names*

### Comparing `magnifier-0.0.6/magnifier/evaluation/classification.py` & `magnifier-0.0.7/magnifier/evaluation/classification.py`

 * *Files identical despite different names*

### Comparing `magnifier-0.0.6/magnifier/model_experiment.py` & `magnifier-0.0.7/magnifier/model_experiment.py`

 * *Files identical despite different names*

### Comparing `magnifier-0.0.6/magnifier/transformer/compressing.py` & `magnifier-0.0.7/magnifier/transformer/compressing.py`

 * *Files identical despite different names*

### Comparing `magnifier-0.0.6/magnifier/transformer/time_series.py` & `magnifier-0.0.7/magnifier/transformer/time_series.py`

 * *Files identical despite different names*

### Comparing `magnifier-0.0.6/pyproject.toml` & `magnifier-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnifier"
-version = "0.0.6"  # using poetry-dynamic-versioning
+version = "0.0.7"  # using poetry-dynamic-versioning
 description = "精度検証やパラメータチューニングで使用する関数群のライブラリ"
 license = "MIT"
 authors = ["koreander2001 <neokamiyama@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/koreander2001/magnifier"
 documentation = "https://koreander2001.github.io/magnifier/"
```

### Comparing `magnifier-0.0.6/PKG-INFO` & `magnifier-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnifier
-Version: 0.0.6
+Version: 0.0.7
 Summary: 精度検証やパラメータチューニングで使用する関数群のライブラリ
 Home-page: https://github.com/koreander2001/magnifier
 License: MIT
 Author: koreander2001
 Author-email: neokamiyama@gmail.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
```


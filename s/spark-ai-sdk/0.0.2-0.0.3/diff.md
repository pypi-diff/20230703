# Comparing `tmp/spark-ai-sdk-0.0.2.tar.gz` & `tmp/spark-ai-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark-ai-sdk-0.0.2.tar", last modified: Mon Jul  3 13:02:23 2023, max compression
+gzip compressed data, was "spark-ai-sdk-0.0.3.tar", last modified: Mon Jul  3 13:07:45 2023, max compression
```

## Comparing `spark-ai-sdk-0.0.2.tar` & `spark-ai-sdk-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 13:02:23.532643 spark-ai-sdk-0.0.2/
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)     1419 2023-07-03 13:02:23.532643 spark-ai-sdk-0.0.2/PKG-INFO
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)      942 2023-07-03 12:47:28.000000 spark-ai-sdk-0.0.2/README.md
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)      531 2023-07-03 13:01:20.000000 spark-ai-sdk-0.0.2/pyproject.toml
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)       38 2023-07-03 13:02:23.532643 spark-ai-sdk-0.0.2/setup.cfg
-drwxrwxr-x   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 13:02:23.532643 spark-ai-sdk-0.0.2/spark_ai_sdk/
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 12:30:28.000000 spark-ai-sdk-0.0.2/spark_ai_sdk/__init__.py
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)     5081 2023-07-03 12:32:18.000000 spark-ai-sdk-0.0.2/spark_ai_sdk/spark_ai.py
-drwxrwxr-x   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 13:02:23.532643 spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)     1419 2023-07-03 13:02:23.000000 spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)      253 2023-07-03 13:02:23.000000 spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)        1 2023-07-03 13:02:23.000000 spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)       24 2023-07-03 13:02:23.000000 spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/requires.txt
--rw-rw-r--   0 tlntin    (1000) tlntin    (1000)       13 2023-07-03 13:02:23.000000 spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 13:07:45.797339 spark-ai-sdk-0.0.3/
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)     1335 2023-07-03 13:07:45.797339 spark-ai-sdk-0.0.3/PKG-INFO
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)      858 2023-07-03 13:05:52.000000 spark-ai-sdk-0.0.3/README.md
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)      531 2023-07-03 13:07:18.000000 spark-ai-sdk-0.0.3/pyproject.toml
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)       38 2023-07-03 13:07:45.797339 spark-ai-sdk-0.0.3/setup.cfg
+drwxrwxr-x   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 13:07:45.797339 spark-ai-sdk-0.0.3/spark_ai_sdk/
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 12:30:28.000000 spark-ai-sdk-0.0.3/spark_ai_sdk/__init__.py
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)     5081 2023-07-03 12:32:18.000000 spark-ai-sdk-0.0.3/spark_ai_sdk/spark_ai.py
+drwxrwxr-x   0 tlntin    (1000) tlntin    (1000)        0 2023-07-03 13:07:45.797339 spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)     1335 2023-07-03 13:07:45.000000 spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)      253 2023-07-03 13:07:45.000000 spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)        1 2023-07-03 13:07:45.000000 spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)       24 2023-07-03 13:07:45.000000 spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/requires.txt
+-rw-rw-r--   0 tlntin    (1000) tlntin    (1000)       13 2023-07-03 13:07:45.000000 spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/top_level.txt
```

### Comparing `spark-ai-sdk-0.0.2/PKG-INFO` & `spark-ai-sdk-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: spark-ai-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: python api for XunFei (iFLYTEK) Spark AI
 Author: Tlntin
 Project-URL: Homepage, https://github.com/Tlntin/spark-ai-sdk
 Project-URL: Bug Tracker, https://github.com/Tlntin/spark-ai-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-## English | [中文](README_zh.md)
+## English | [中文](https://github.com/Tlntin/spark-ai-sdk/blob/main/README_zh.md)
 
 ## what is?
 - python sdk for XunFei (iFLYTEK) Spark AI
 
 ## how to use
 1. get Spark AI api in https://www.xfyun.cn/
 
 2. install
 ```bash
-git clone https://github.com/Tlntin/spark-ai-sdk.git
-cd spark-ai-sdk
-python setup.py install
-
-# or
-pip install git+https://github.com/Tlntin/spark-ai-sdk.git
+pip install spark-ai-sdk
 ```
 
 3. use
 
 ```python
 from spark_ai_sdk.spark_ai import SparkAI
```

### Comparing `spark-ai-sdk-0.0.2/README.md` & `spark-ai-sdk-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-## English | [中文](README_zh.md)
+## English | [中文](https://github.com/Tlntin/spark-ai-sdk/blob/main/README_zh.md)
 
 ## what is?
 - python sdk for XunFei (iFLYTEK) Spark AI
 
 ## how to use
 1. get Spark AI api in https://www.xfyun.cn/
 
 2. install
 ```bash
-git clone https://github.com/Tlntin/spark-ai-sdk.git
-cd spark-ai-sdk
-python setup.py install
-
-# or
-pip install git+https://github.com/Tlntin/spark-ai-sdk.git
+pip install spark-ai-sdk
 ```
 
 3. use
 
 ```python
 from spark_ai_sdk.spark_ai import SparkAI
```

### Comparing `spark-ai-sdk-0.0.2/pyproject.toml` & `spark-ai-sdk-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spark-ai-sdk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Tlntin" },
 ]
 description = "python api for XunFei (iFLYTEK) Spark AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spark-ai-sdk-0.0.2/spark_ai_sdk/spark_ai.py` & `spark-ai-sdk-0.0.3/spark_ai_sdk/spark_ai.py`

 * *Files identical despite different names*

### Comparing `spark-ai-sdk-0.0.2/spark_ai_sdk.egg-info/PKG-INFO` & `spark-ai-sdk-0.0.3/spark_ai_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: spark-ai-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: python api for XunFei (iFLYTEK) Spark AI
 Author: Tlntin
 Project-URL: Homepage, https://github.com/Tlntin/spark-ai-sdk
 Project-URL: Bug Tracker, https://github.com/Tlntin/spark-ai-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-## English | [中文](README_zh.md)
+## English | [中文](https://github.com/Tlntin/spark-ai-sdk/blob/main/README_zh.md)
 
 ## what is?
 - python sdk for XunFei (iFLYTEK) Spark AI
 
 ## how to use
 1. get Spark AI api in https://www.xfyun.cn/
 
 2. install
 ```bash
-git clone https://github.com/Tlntin/spark-ai-sdk.git
-cd spark-ai-sdk
-python setup.py install
-
-# or
-pip install git+https://github.com/Tlntin/spark-ai-sdk.git
+pip install spark-ai-sdk
 ```
 
 3. use
 
 ```python
 from spark_ai_sdk.spark_ai import SparkAI
```


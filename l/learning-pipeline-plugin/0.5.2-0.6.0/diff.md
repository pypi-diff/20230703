# Comparing `tmp/learning_pipeline_plugin-0.5.2.tar.gz` & `tmp/learning_pipeline_plugin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning_pipeline_plugin-0.5.2.tar", max compression
+gzip compressed data, was "learning_pipeline_plugin-0.6.0.tar", max compression
```

## Comparing `learning_pipeline_plugin-0.5.2.tar` & `learning_pipeline_plugin-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     2538 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/README.md
--rw-r--r--   0        0        0      164 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/__init__.py
--rw-r--r--   0        0        0     2242 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/actfw_utils.py
--rw-r--r--   0        0        0       90 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/__init__.py
--rw-r--r--   0        0        0     5857 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/stream_al.py
--rw-r--r--   0        0        0    10929 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_diversity.py
--rw-r--r--   0        0        0     2405 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_utils.py
--rw-r--r--   0        0        0      802 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/type_helper.py
--rw-r--r--   0        0        0     2250 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/uncertainty.py
--rw-r--r--   0        0        0     3118 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/collect_pipe.py
--rw-r--r--   0        0        0      881 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/notifier.py
--rw-r--r--   0        0        0     3986 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/select_task.py
--rw-r--r--   0        0        0    12048 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/sender_task.py
--rw-r--r--   0        0        0      707 2023-05-17 05:44:28.139762 learning_pipeline_plugin-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/README.md
+-rw-r--r--   0        0        0      164 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/actfw_utils/__init__.py
+-rw-r--r--   0        0        0     2242 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/actfw_utils/isolated_task.py
+-rw-r--r--   0        0        0     1150 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/actfw_utils/pseudo_pipe.py
+-rw-r--r--   0        0        0       90 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/__init__.py
+-rw-r--r--   0        0        0     5857 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/stream_al.py
+-rw-r--r--   0        0        0    10929 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/submodular_diversity.py
+-rw-r--r--   0        0        0     2405 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/submodular_utils.py
+-rw-r--r--   0        0        0      802 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/type_helper.py
+-rw-r--r--   0        0        0     2250 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/uncertainty.py
+-rw-r--r--   0        0        0     3118 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/collect_pipe.py
+-rw-r--r--   0        0        0      881 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/notifier.py
+-rw-r--r--   0        0        0     3986 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/select_task.py
+-rw-r--r--   0        0        0    12048 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/sender_task.py
+-rw-r--r--   0        0        0      788 2023-07-03 02:26:26.553689 learning_pipeline_plugin-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 learning_pipeline_plugin-0.6.0/PKG-INFO
```

### Comparing `learning_pipeline_plugin-0.5.2/README.md` & `learning_pipeline_plugin-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/actfw_utils.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/actfw_utils/isolated_task.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/stream_al.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/stream_al.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_diversity.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/submodular_diversity.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/submodular_utils.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/submodular_utils.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/type_helper.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/type_helper.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/algorithms/uncertainty.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/algorithms/uncertainty.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/collect_pipe.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/collect_pipe.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/notifier.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/notifier.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/select_task.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/select_task.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/learning_pipeline_plugin/sender_task.py` & `learning_pipeline_plugin-0.6.0/learning_pipeline_plugin/sender_task.py`

 * *Files identical despite different names*

### Comparing `learning_pipeline_plugin-0.5.2/pyproject.toml` & `learning_pipeline_plugin-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "learning-pipeline-plugin"
-version = "0.5.2"
+version = "0.6.0"
 description = ""
 authors = ["Idein Inc."]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "learning_pipeline_plugin"}]
 repository = "https://github.com/Idein/learning-pipeline-plugin"
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.0, <3.8"
+python = ">=3.7.0, <3.11"
 actfw-core = "^2.2.0"
 requests = {extras = ["socks"], version = "^2.28.1"}
 numpy = "~1"
 typing-extensions = "^4.4.0"
-pillow = "<6"
+pillow = [
+    {version = "^5", python = "< 3.8"},
+    {version = "^8", python = ">= 3.8"},
+]
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 pytest = "^7.2.0"
 pycodestyle = "^2.10.0"
 types-requests = "^2.28.11.7"
```

### Comparing `learning_pipeline_plugin-0.5.2/PKG-INFO` & `learning_pipeline_plugin-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: learning-pipeline-plugin
-Version: 0.5.2
+Version: 0.6.0
 Summary: 
 Home-page: https://github.com/Idein/learning-pipeline-plugin
 License: MIT
 Author: Idein Inc.
-Requires-Python: >=3.7.0,<3.8
+Requires-Python: >=3.7.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: actfw-core (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1,<2)
-Requires-Dist: pillow (<6)
+Requires-Dist: pillow (>=5,<6) ; python_version < "3.8"
+Requires-Dist: pillow (>=8,<9) ; python_version >= "3.8"
 Requires-Dist: requests[socks] (>=2.28.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Repository, https://github.com/Idein/learning-pipeline-plugin
 Description-Content-Type: text/markdown
 
 # learning-pipeline-plugin
```


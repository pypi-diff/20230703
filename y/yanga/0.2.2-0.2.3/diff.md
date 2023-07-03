# Comparing `tmp/yanga-0.2.2.tar.gz` & `tmp/yanga-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-0.2.2.tar", max compression
+gzip compressed data, was "yanga-0.2.3.tar", max compression
```

## Comparing `yanga-0.2.2.tar` & `yanga-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-07-03 11:17:44.712369 yanga-0.2.2/LICENSE
--rw-r--r--   0        0        0     4695 2023-07-03 11:17:44.712369 yanga-0.2.2/README.md
--rw-r--r--   0        0        0     2384 2023-07-03 11:17:45.992377 yanga-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-03 11:17:45.952377 yanga-0.2.2/src/yanga/__init__.py
--rw-r--r--   0        0        0      347 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/_yrun.py
--rw-r--r--   0        0        0        0 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/__init__.py
--rw-r--r--   0        0        0     1802 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/build.py
--rw-r--r--   0        0        0     2298 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/init.py
--rw-r--r--   0        0        0      412 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/cookiecutter.json
--rw-r--r--   0        0        0        7 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
--rw-r--r--   0        0        0     5389 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1
--rw-r--r--   0        0        0     3853 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
--rw-r--r--   0        0        0      785 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
--rw-r--r--   0        0        0      157 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
--rw-r--r--   0        0        0       34 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
--rw-r--r--   0        0        0      247 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
--rw-r--r--   0        0        0      110 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
--rw-r--r--   0        0        0        0 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/core/__init__.py
--rw-r--r--   0        0        0     4221 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/core/docs_utils.py
--rw-r--r--   0        0        0      278 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/core/exceptions.py
--rw-r--r--   0        0        0     1583 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/core/logger.py
--rw-r--r--   0        0        0     2910 2023-07-03 11:17:44.716369 yanga-0.2.2/src/yanga/core/scoop_wrapper.py
--rw-r--r--   0        0        0     1349 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/core/subprocess.py
--rw-r--r--   0        0        0        0 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/__init__.py
--rw-r--r--   0        0        0      851 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/build_main.py
--rw-r--r--   0        0        0      965 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/config.py
--rw-r--r--   0        0        0      477 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/environment.py
--rw-r--r--   0        0        0     3141 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/pipeline.py
--rw-r--r--   0        0        0      864 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/project.py
--rw-r--r--   0        0        0      670 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/stages.py
--rw-r--r--   0        0        0      886 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ybuild/variant.py
--rw-r--r--   0        0        0      790 2023-07-03 11:17:44.720369 yanga-0.2.2/src/yanga/ymain.py
--rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-03 16:56:32.184599 yanga-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4695 2023-07-03 16:56:32.184599 yanga-0.2.3/README.md
+-rw-r--r--   0        0        0     2384 2023-07-03 16:56:33.040606 yanga-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-03 16:56:33.008606 yanga-0.2.3/src/yanga/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/_yrun.py
+-rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/build.py
+-rw-r--r--   0        0        0     2493 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/init.py
+-rw-r--r--   0        0        0      412 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/cookiecutter.json
+-rw-r--r--   0        0        0        7 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
+-rw-r--r--   0        0        0     5389 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1
+-rw-r--r--   0        0        0     3853 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
+-rw-r--r--   0        0        0      785 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
+-rw-r--r--   0        0        0      157 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
+-rw-r--r--   0        0        0       34 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
+-rw-r--r--   0        0        0      247 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
+-rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/__init__.py
+-rw-r--r--   0        0        0     4221 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/exceptions.py
+-rw-r--r--   0        0        0     1583 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/logger.py
+-rw-r--r--   0        0        0     2910 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     1349 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/subprocess.py
+-rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/__init__.py
+-rw-r--r--   0        0        0      851 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/build_main.py
+-rw-r--r--   0        0        0      965 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/config.py
+-rw-r--r--   0        0        0      477 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/environment.py
+-rw-r--r--   0        0        0     3141 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/pipeline.py
+-rw-r--r--   0        0        0      864 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/project.py
+-rw-r--r--   0        0        0      670 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/stages.py
+-rw-r--r--   0        0        0      886 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/variant.py
+-rw-r--r--   0        0        0      790 2023-07-03 16:56:32.188599 yanga-0.2.3/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.2.3/PKG-INFO
```

### Comparing `yanga-0.2.2/LICENSE` & `yanga-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/README.md` & `yanga-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/pyproject.toml` & `yanga-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "0.2.2"
+version = "0.2.3"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
```

### Comparing `yanga-0.2.2/src/yanga/commands/build.py` & `yanga-0.2.3/src/yanga/commands/build.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1` & `yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py` & `yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1` & `yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/core/cmd_line.py` & `yanga-0.2.3/src/yanga/core/cmd_line.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/core/docs_utils.py` & `yanga-0.2.3/src/yanga/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/core/logger.py` & `yanga-0.2.3/src/yanga/core/logger.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/core/scoop_wrapper.py` & `yanga-0.2.3/src/yanga/core/scoop_wrapper.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/core/subprocess.py` & `yanga-0.2.3/src/yanga/core/subprocess.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ybuild/build_main.py` & `yanga-0.2.3/src/yanga/ybuild/build_main.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ybuild/config.py` & `yanga-0.2.3/src/yanga/ybuild/config.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ybuild/pipeline.py` & `yanga-0.2.3/src/yanga/ybuild/pipeline.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ybuild/project.py` & `yanga-0.2.3/src/yanga/ybuild/project.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ybuild/stages.py` & `yanga-0.2.3/src/yanga/ybuild/stages.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ybuild/variant.py` & `yanga-0.2.3/src/yanga/ybuild/variant.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/src/yanga/ymain.py` & `yanga-0.2.3/src/yanga/ymain.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.2/PKG-INFO` & `yanga-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 0.2.2
+Version: 0.2.3
 Summary: Yet another ninja generator to build C/CPP projects.
 Home-page: https://github.com/cuinixam/yanga
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yanga Version: 0.2.2 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 0.2.3 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```


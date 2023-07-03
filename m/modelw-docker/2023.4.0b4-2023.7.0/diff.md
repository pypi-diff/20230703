# Comparing `tmp/modelw_docker-2023.4.0b4.tar.gz` & `tmp/modelw_docker-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_docker-2023.4.0b4.tar", max compression
+gzip compressed data, was "modelw_docker-2023.7.0.tar", max compression
```

## Comparing `modelw_docker-2023.4.0b4.tar` & `modelw_docker-2023.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-05-04 15:27:48.554730 modelw_docker-2023.4.0b4/LICENSE
--rw-r--r--   0        0        0     4666 2023-05-04 15:27:48.554730 modelw_docker-2023.4.0b4/README.md
--rw-r--r--   0        0        0     1201 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/__init__.py
--rw-r--r--   0        0        0     2753 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/__main__.py
--rw-r--r--   0        0        0     1494 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/build.py
--rw-r--r--   0        0        0     7307 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/config.py
--rw-r--r--   0        0        0      209 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/exceptions.py
--rw-r--r--   0        0        0     5229 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/install.py
--rw-r--r--   0        0        0     7755 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/output.py
--rw-r--r--   0        0        0     1662 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/platform.py
--rw-r--r--   0        0        0        0 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/py.typed
--rw-r--r--   0        0        0     2580 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/run.py
--rw-r--r--   0        0        0     5865 2023-05-04 15:27:48.558730 modelw_docker-2023.4.0b4/src/model_w/docker/serve.py
--rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 modelw_docker-2023.4.0b4/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     4666 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/README.md
+-rw-r--r--   0        0        0     1199 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/src/model_w/docker/__init__.py
+-rw-r--r--   0        0        0     2753 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/__main__.py
+-rw-r--r--   0        0        0     1494 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/build.py
+-rw-r--r--   0        0        0     7307 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/config.py
+-rw-r--r--   0        0        0      209 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/exceptions.py
+-rw-r--r--   0        0        0     5229 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/install.py
+-rw-r--r--   0        0        0     7755 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/output.py
+-rw-r--r--   0        0        0     1662 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/platform.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/py.typed
+-rw-r--r--   0        0        0     2580 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/run.py
+-rw-r--r--   0        0        0     5865 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/serve.py
+-rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 modelw_docker-2023.7.0/PKG-INFO
```

### Comparing `modelw_docker-2023.4.0b4/README.md` & `modelw_docker-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/pyproject.toml` & `modelw_docker-2023.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-docker"
-version = "2023.4.0b4"
+version = "2023.7.0"
 description = "Utility to simplify Dockerfiles"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 packages = [{include = "model_w/docker", from = "src"}]
 repository = "https://github.com/ModelW/docker/"
 documentation = "https://github.com/ModelW/docker/"
```

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/__main__.py` & `modelw_docker-2023.7.0/src/model_w/docker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/build.py` & `modelw_docker-2023.7.0/src/model_w/docker/build.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/config.py` & `modelw_docker-2023.7.0/src/model_w/docker/config.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/install.py` & `modelw_docker-2023.7.0/src/model_w/docker/install.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/output.py` & `modelw_docker-2023.7.0/src/model_w/docker/output.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/platform.py` & `modelw_docker-2023.7.0/src/model_w/docker/platform.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/run.py` & `modelw_docker-2023.7.0/src/model_w/docker/run.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/src/model_w/docker/serve.py` & `modelw_docker-2023.7.0/src/model_w/docker/serve.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.4.0b4/PKG-INFO` & `modelw_docker-2023.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-docker
-Version: 2023.4.0b4
+Version: 2023.7.0
 Summary: Utility to simplify Dockerfiles
 Home-page: https://github.com/ModelW/docker/
 License: WTFPL
 Keywords: docker,django,nuxt,dockerfile
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
@@ -13,16 +13,14 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: typefit (>=0.4.2,<0.5.0)
```


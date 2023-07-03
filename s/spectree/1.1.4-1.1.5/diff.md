# Comparing `tmp/spectree-1.1.4.tar.gz` & `tmp/spectree-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectree-1.1.4.tar", last modified: Sat Jul  1 07:34:41 2023, max compression
+gzip compressed data, was "spectree-1.1.5.tar", last modified: Mon Jul  3 11:49:39 2023, max compression
```

## Comparing `spectree-1.1.4.tar` & `spectree-1.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-01 07:34:30.000000 spectree-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 07:34:30.000000 spectree-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-01 07:34:41.414464 spectree-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-07-01 07:34:30.000000 spectree-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-01 07:34:30.000000 spectree-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:34:41.414464 spectree-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-01 07:34:30.000000 spectree-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/spectree/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/spectree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/falcon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/flask_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/quart_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/plugins/starlette_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-07-01 07:34:30.000000 spectree-1.1.4/spectree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/spectree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 07:34:41.000000 spectree-1.1.4/spectree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:34:41.414464 spectree-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_falcon_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_flask_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_flask_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_quart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_plugin_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-01 07:34:30.000000 spectree-1.1.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.403936 spectree-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-03 11:49:27.000000 spectree-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 11:49:27.000000 spectree-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-03 11:49:39.403936 spectree-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-07-03 11:49:27.000000 spectree-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-03 11:49:27.000000 spectree-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:49:39.403936 spectree-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 11:49:27.000000 spectree-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.399936 spectree-1.1.5/spectree/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.403936 spectree-1.1.5/spectree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/falcon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/flask_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/quart_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/starlette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.399936 spectree-1.1.5/spectree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.403936 spectree-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_falcon_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_flask_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_flask_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_quart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_utils.py
```

### Comparing `spectree-1.1.4/LICENSE` & `spectree-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/PKG-INFO` & `spectree-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.4
+Version: 1.1.5
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
```

### Comparing `spectree-1.1.4/README.md` & `spectree-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/pyproject.toml` & `spectree-1.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spectree"
-version = "1.1.4"
+version = "1.1.5"
 dynamic = []
 description = "generate OpenAPI document and validate request&response with Python annotations."
 readme = "README.md"
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
     { name = "Keming Yang", email = "kemingy94@gmail.com" },
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "pydantic>=1.9.1",
+    "pydantic>=1.2,<2",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autoflake>=1.4,<3.0",
     "black>=22.3,<24.0",
     "flake8>=4,<7",
```

### Comparing `spectree-1.1.4/setup.py` & `spectree-1.1.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 # this file is kept for GitHub's dependency graph
 
 setup(
     name="spectree",
     install_requires=[
-        "pydantic>=1.2",
+        "pydantic>=1.2,<2",
     ],
     extras_require={
         "email": ["pydantic[email]>=1.2,<2"],
         "flask": ["flask"],
         "quart": ["quart"],
         "falcon": ["falcon>=3.0.0"],
         "starlette": ["starlette[full]"],
```

### Comparing `spectree-1.1.4/spectree/_types.py` & `spectree-1.1.5/spectree/_types.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/config.py` & `spectree-1.1.5/spectree/config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/models.py` & `spectree-1.1.5/spectree/models.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/page.py` & `spectree-1.1.5/spectree/page.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/plugins/__init__.py` & `spectree-1.1.5/spectree/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/plugins/base.py` & `spectree-1.1.5/spectree/plugins/base.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/plugins/falcon_plugin.py` & `spectree-1.1.5/spectree/plugins/falcon_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/plugins/flask_plugin.py` & `spectree-1.1.5/spectree/plugins/flask_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/plugins/quart_plugin.py` & `spectree-1.1.5/spectree/plugins/quart_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/plugins/starlette_plugin.py` & `spectree-1.1.5/spectree/plugins/starlette_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/response.py` & `spectree-1.1.5/spectree/response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/spec.py` & `spectree-1.1.5/spectree/spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree/utils.py` & `spectree-1.1.5/spectree/utils.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/spectree.egg-info/PKG-INFO` & `spectree-1.1.5/spectree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.4
+Version: 1.1.5
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
```

### Comparing `spectree-1.1.4/spectree.egg-info/SOURCES.txt` & `spectree-1.1.5/spectree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_config.py` & `spectree-1.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin.py` & `spectree-1.1.5/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_falcon.py` & `spectree-1.1.5/tests/test_plugin_falcon.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_falcon_asgi.py` & `spectree-1.1.5/tests/test_plugin_falcon_asgi.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_flask.py` & `spectree-1.1.5/tests/test_plugin_flask.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_flask_blueprint.py` & `spectree-1.1.5/tests/test_plugin_flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_flask_view.py` & `spectree-1.1.5/tests/test_plugin_flask_view.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_quart.py` & `spectree-1.1.5/tests/test_plugin_quart.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_plugin_starlette.py` & `spectree-1.1.5/tests/test_plugin_starlette.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_response.py` & `spectree-1.1.5/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_spec.py` & `spectree-1.1.5/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.4/tests/test_utils.py` & `spectree-1.1.5/tests/test_utils.py`

 * *Files identical despite different names*


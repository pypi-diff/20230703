# Comparing `tmp/cmem_plugin_base-4.0.0.tar.gz` & `tmp/cmem_plugin_base-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_base-4.0.0.tar", max compression
+gzip compressed data, was "cmem_plugin_base-4.0.0rc1.tar", max compression
```

## Comparing `cmem_plugin_base-4.0.0.tar` & `cmem_plugin_base-4.0.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11334 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/LICENSE
--rw-r--r--   0        0        0      246 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/README-public.md
--rw-r--r--   0        0        0       73 2023-07-03 13:07:24.905320 cmem_plugin_base-4.0.0/cmem_plugin_base/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/__init__.py
--rw-r--r--   0        0        0     3992 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/context.py
--rw-r--r--   0        0        0     8897 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/description.py
--rw-r--r--   0        0        0     2765 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/discovery.py
--rw-r--r--   0        0        0     1370 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/entity.py
--rw-r--r--   0        0        0       37 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/__init__.py
--rw-r--r--   0        0        0     1557 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/choice.py
--rw-r--r--   0        0        0     2243 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/dataset.py
--rw-r--r--   0        0        0     3629 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/graph.py
--rw-r--r--   0        0        0      334 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/multiline.py
--rw-r--r--   0        0        0     1739 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/password.py
--rw-r--r--   0        0        0     2625 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/plugins.py
--rw-r--r--   0        0        0     8501 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/types.py
--rw-r--r--   0        0        0     3429 2023-07-03 13:07:01.200910 cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/utils.py
--rw-r--r--   0        0        0     2084 2023-07-03 13:07:24.905320 cmem_plugin_base-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 cmem_plugin_base-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2022-02-21 20:33:41.000000 cmem_plugin_base-4.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      246 2022-04-01 14:58:42.645640 cmem_plugin_base-4.0.0rc1/README-public.md
+-rw-r--r--   0        0        0       76 2023-06-22 12:52:05.577458 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-22 01:06:38.000000 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/__init__.py
+-rw-r--r--   0        0        0     3992 2023-03-15 08:18:43.081458 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/context.py
+-rw-r--r--   0        0        0     8897 2023-03-15 08:18:43.081597 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/description.py
+-rw-r--r--   0        0        0     2765 2023-04-27 12:51:39.614863 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/discovery.py
+-rw-r--r--   0        0        0     1370 2022-02-22 12:38:14.000000 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/entity.py
+-rw-r--r--   0        0        0       37 2022-05-04 12:15:39.899212 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/__init__.py
+-rw-r--r--   0        0        0     1557 2023-03-15 08:18:43.081854 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py
+-rw-r--r--   0        0        0     2243 2023-03-15 08:18:43.081961 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py
+-rw-r--r--   0        0        0     3629 2023-03-15 08:18:43.082069 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py
+-rw-r--r--   0        0        0      334 2022-06-15 11:32:12.636378 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/multiline.py
+-rw-r--r--   0        0        0     1739 2023-03-15 08:18:43.082177 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/password.py
+-rw-r--r--   0        0        0     2625 2023-03-15 08:18:43.082282 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/plugins.py
+-rw-r--r--   0        0        0     8501 2023-03-15 08:18:43.082793 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/types.py
+-rw-r--r--   0        0        0     3429 2023-03-15 08:18:43.082970 cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/utils.py
+-rw-r--r--   0        0        0     2059 2023-06-22 12:52:05.576580 cmem_plugin_base-4.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 cmem_plugin_base-4.0.0rc1/PKG-INFO
```

### Comparing `cmem_plugin_base-4.0.0/LICENSE` & `cmem_plugin_base-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/context.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/context.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/description.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/description.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/discovery.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/discovery.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/entity.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/entity.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/choice.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/choice.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/dataset.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/graph.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/parameter/password.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/parameter/password.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/plugins.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/plugins.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/types.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/types.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/cmem_plugin_base/dataintegration/utils.py` & `cmem_plugin_base-4.0.0rc1/cmem_plugin_base/dataintegration/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_base-4.0.0/pyproject.toml` & `cmem_plugin_base-4.0.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "cmem-plugin-base"
-version = "4.0.0"
+version = "4.0.0rc1"
 license = "Apache-2.0"
 description = "Base classes for developing eccenca Coporate Memory plugins."
 authors = ["eccenca <cmempy-developer@eccenca.com>"]
 maintainers = [
     "Sebastian Tramp <sebastian.tramp@eccenca.com>",
     "Robert Isele <robert.isele@eccenca.com>"
 ]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugins", "DataIntegration"
 ]
@@ -25,23 +25,22 @@
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.7"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
 genbadge = "^1.1.0"
-mypy = "^1.4.1"
-pillow = "9.5.0"
+mypy = "^1.4.0"
 pylint-junit = "^0.3.2"
-pytest = "^7.4.0"
+pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 pytest-memray = "^1.4.1"
 safety = "^1.10.3"
 typed-ast = "^1.5.4"
-types-requests = "^2.31.0.1"
+types-requests = "^2.28.11.15"
 wheel = "^0.38.4"
 # added in order to have something to discover (>=0.0.0 <1.0.0)
 # cmem-plugin-examples = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cmem_plugin_base-4.0.0/PKG-INFO` & `cmem_plugin_base-4.0.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-base
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Base classes for developing eccenca Coporate Memory plugins.
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugins,DataIntegration
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
 Requires-Python: >=3.11,<4.0
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cmem-cmempy (==23.1)
 Description-Content-Type: text/markdown
```


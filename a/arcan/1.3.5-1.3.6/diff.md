# Comparing `tmp/arcan-1.3.5.tar.gz` & `tmp/arcan-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.3.5.tar", max compression
+gzip compressed data, was "arcan-1.3.6.tar", max compression
```

## Comparing `arcan-1.3.5.tar` & `arcan-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1711 2023-07-02 08:54:16.705825 arcan-1.3.5/LICENSE
--rw-r--r--   0        0        0     2888 2023-07-02 08:54:16.705825 arcan-1.3.5/README.md
--rw-r--r--   0        0        0      907 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/agent/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/session/__init__.py
--rw-r--r--   0        0        0       31 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/storage/__init__.py
--rw-r--r--   0        0        0       62 2023-07-02 08:54:16.709826 arcan-1.3.5/main.py
--rw-r--r--   0        0        0      753 2023-07-02 08:54:16.709826 arcan-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 arcan-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-07-03 14:31:27.672241 arcan-1.3.6/LICENSE
+-rw-r--r--   0        0        0     2888 2023-07-03 14:31:27.672241 arcan-1.3.6/README.md
+-rw-r--r--   0        0        0      907 2023-07-03 14:31:27.672241 arcan-1.3.6/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.672241 arcan-1.3.6/arcan/agent/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.672241 arcan-1.3.6/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/session/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-03 14:31:27.676241 arcan-1.3.6/arcan/storage/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-03 14:31:27.676241 arcan-1.3.6/main.py
+-rw-r--r--   0        0        0      753 2023-07-03 14:31:27.676241 arcan-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 arcan-1.3.6/PKG-INFO
```

### Comparing `arcan-1.3.5/LICENSE` & `arcan-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.3.5/README.md` & `arcan-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `arcan-1.3.5/arcan/__init__.py` & `arcan-1.3.6/arcan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # %%
 from modal import Stub, web_endpoint
 from modal import Image, Stub, web_endpoint
 
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 
 
 # %%
 # %%
 def get_arcan_version():
     try:
         import arcan
```

### Comparing `arcan-1.3.5/pyproject.toml` & `arcan-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcan"
-version = "1.3.5"
+version = "1.3.6"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "arcan.ai Non-Commercial Open Source License"
 readme = "README.md"
 packages = [
     {include = "arcan"},
     {include = "main.py"}
```

### Comparing `arcan-1.3.5/PKG-INFO` & `arcan-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.3.5
+Version: 1.3.6
 Summary: A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools
 License: arcan.ai Non-Commercial Open Source License
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arcan Version: 1.3.5 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.3.6 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
 modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
 License Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: black (>=23.3.0,<24.0.0) Requires-
```


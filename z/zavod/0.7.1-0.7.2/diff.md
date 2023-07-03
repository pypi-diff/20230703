# Comparing `tmp/zavod-0.7.1.tar.gz` & `tmp/zavod-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zavod-0.7.1.tar", last modified: Thu Jun 29 07:46:26 2023, max compression
+gzip compressed data, was "zavod-0.7.2.tar", last modified: Mon Jul  3 10:09:51 2023, max compression
```

## Comparing `zavod-0.7.1.tar` & `zavod-0.7.2.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-29 07:44:20.000000 zavod-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 07:44:20.000000 zavod-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 07:46:26.196416 zavod-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 07:44:20.000000 zavod-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:46:26.196416 zavod-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-29 07:44:20.000000 zavod-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.192416 zavod-0.7.1/zavod/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/zavod/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/zavod/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/json_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/json_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/pack_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/zavod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:46:07.000000 zavod-0.7.1/zavod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.432818 zavod-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 10:07:53.000000 zavod-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 10:07:53.000000 zavod-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 10:09:51.432818 zavod-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-03 10:07:53.000000 zavod-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:09:51.432818 zavod-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-03 10:07:53.000000 zavod-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.428818 zavod-0.7.2/zavod/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.428818 zavod-0.7.2/zavod/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.432818 zavod-0.7.2/zavod/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/json_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.428818 zavod-0.7.2/zavod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:09:35.000000 zavod-0.7.2/zavod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/top_level.txt
```

### Comparing `zavod-0.7.1/LICENSE` & `zavod-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/PKG-INFO` & `zavod-0.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.7.1
+Version: 0.7.2
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
+
```

### Comparing `zavod-0.7.1/setup.py` & `zavod-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="zavod",
-    version="0.7.1",
+    version="0.7.2",
     description="Data factory for followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney etl parsing",
     author="Friedrich Lindenberg",
     author_email="friedrich@opensanctions.org",
     url="https://github.com/opensanctions/zavod",
@@ -18,15 +18,15 @@
     packages=find_packages(exclude=["ez_setup", "examples", "tests"]),
     namespace_packages=[],
     include_package_data=True,
     package_data={"": ["zavod/data/*", "zavod/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.2.0, < 4.0.0",
-        "nomenklatura >= 3.0.2, < 4.0.0",
+        "nomenklatura >= 3.1.0, < 4.0.0",
         "addressformatting >= 1.3.0, < 2.0.0",
         "datapatch >= 0.2.1",
         "click >= 8.0.0, < 8.2.0",
         "requests",
         "structlog",
         "lxml",
     ],
```

### Comparing `zavod-0.7.1/zavod/__init__.py` & `zavod-0.7.2/zavod/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from zavod import settings
 from zavod.context import GenericZavod
 from zavod.dataset import ZavodDataset, ZD
 from zavod.logs import configure_logging, get_logger
 from zavod.sinks.common import Sink
 from zavod.sinks.json_entity import JSONEntitySink
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 __all__ = [
     "init",
     "context",
     "Zavod",
     "ZavodDataset",
     "ZD",
     "PathLike",
```

### Comparing `zavod-0.7.1/zavod/audit.py` & `zavod-0.7.2/zavod/audit.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/context.py` & `zavod-0.7.2/zavod/context.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/dataset.py` & `zavod-0.7.2/zavod/dataset.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/http.py` & `zavod-0.7.2/zavod/http.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/logs.py` & `zavod-0.7.2/zavod/logs.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/parse/addresses.py` & `zavod-0.7.2/zavod/parse/addresses.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/parse/names.py` & `zavod-0.7.2/zavod/parse/names.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/parse/xml.py` & `zavod-0.7.2/zavod/parse/xml.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/sinks/common.py` & `zavod-0.7.2/zavod/sinks/common.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod/util.py` & `zavod-0.7.2/zavod/util.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.1/zavod.egg-info/PKG-INFO` & `zavod-0.7.2/zavod.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.7.1
+Version: 0.7.2
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
+
```

### Comparing `zavod-0.7.1/zavod.egg-info/SOURCES.txt` & `zavod-0.7.2/zavod.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 zavod/parse/__init__.py
 zavod/parse/addresses.py
 zavod/parse/names.py
 zavod/parse/xml.py
 zavod/sinks/__init__.py
 zavod/sinks/common.py
 zavod/sinks/json_entity.py
-zavod/sinks/json_statement.py
-zavod/sinks/pack_statement.py
+zavod/sinks/statement.py
```


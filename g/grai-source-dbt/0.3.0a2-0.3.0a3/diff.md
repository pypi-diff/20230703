# Comparing `tmp/grai_source_dbt-0.3.0a2.tar.gz` & `tmp/grai_source_dbt-0.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.3.0a2.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.3.0a3.tar", max compression
```

## Comparing `grai_source_dbt-0.3.0a2.tar` & `grai_source_dbt-0.3.0a3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      124 2023-05-02 08:01:59.695588 grai_source_dbt-0.3.0a2/README.md
--rw-r--r--   0        0        0     1077 2023-06-30 11:55:54.393959 grai_source_dbt-0.3.0a2/pyproject.toml
--rw-r--r--   0        0        0      217 2023-06-30 11:56:07.161987 grai_source_dbt-0.3.0a2/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-22 09:54:48.652302 grai_source_dbt-0.3.0a2/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     8357 2023-06-29 12:17:12.998756 grai_source_dbt-0.3.0a2/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      695 2023-06-06 17:35:16.802940 grai_source_dbt-0.3.0a2/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      934 2023-06-29 12:55:58.962310 grai_source_dbt-0.3.0a2/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-02-14 12:06:39.089774 grai_source_dbt-0.3.0a2/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-02-14 12:06:39.090263 grai_source_dbt-0.3.0a2/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      995 2023-06-06 17:35:16.803842 grai_source_dbt-0.3.0a2/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     2043 2023-06-06 17:35:16.804153 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      985 2023-06-06 17:35:16.804291 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      288 2023-06-06 17:35:16.804400 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     6197 2023-06-16 16:15:18.431432 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-22 09:54:48.653526 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-22 09:54:48.653655 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-22 09:54:48.653765 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653884 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653991 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2423 2023-06-06 17:35:16.804770 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-24 17:33:29.685755 grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-22 09:54:48.654363 grai_source_dbt-0.3.0a2/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2501 2023-06-16 16:15:18.431554 grai_source_dbt-0.3.0a2/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2584 2023-06-06 17:35:16.805007 grai_source_dbt-0.3.0a2/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      189 2023-06-06 17:35:16.805133 grai_source_dbt-0.3.0a2/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     2631 2023-06-29 13:30:53.867579 grai_source_dbt-0.3.0a2/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.090850 grai_source_dbt-0.3.0a2/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0     1243 2023-06-06 17:35:16.805384 grai_source_dbt-0.3.0a2/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-05-02 08:01:59.695588 grai_source_dbt-0.3.0a3/README.md
+-rw-r--r--   0        0        0     1078 2023-07-03 12:48:28.221746 grai_source_dbt-0.3.0a3/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-07-03 12:48:33.081215 grai_source_dbt-0.3.0a3/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-22 09:54:48.652302 grai_source_dbt-0.3.0a3/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     8357 2023-06-29 12:17:12.998756 grai_source_dbt-0.3.0a3/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      695 2023-06-06 17:35:16.802940 grai_source_dbt-0.3.0a3/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0      929 2023-06-30 17:13:40.673550 grai_source_dbt-0.3.0a3/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-02-14 12:06:39.089774 grai_source_dbt-0.3.0a3/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-02-14 12:06:39.090263 grai_source_dbt-0.3.0a3/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      995 2023-06-06 17:35:16.803842 grai_source_dbt-0.3.0a3/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     2043 2023-06-06 17:35:16.804153 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-06 17:35:16.804291 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      288 2023-06-06 17:35:16.804400 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     6197 2023-06-16 16:15:18.431432 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-22 09:54:48.653526 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-22 09:54:48.653655 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-22 09:54:48.653765 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653884 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653991 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2423 2023-06-06 17:35:16.804770 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-24 17:33:29.685755 grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-22 09:54:48.654363 grai_source_dbt-0.3.0a3/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2501 2023-06-16 16:15:18.431554 grai_source_dbt-0.3.0a3/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2584 2023-06-06 17:35:16.805007 grai_source_dbt-0.3.0a3/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      189 2023-06-06 17:35:16.805133 grai_source_dbt-0.3.0a3/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     2631 2023-06-29 13:30:53.867579 grai_source_dbt-0.3.0a3/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.090850 grai_source_dbt-0.3.0a3/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0     1243 2023-06-06 17:35:16.805384 grai_source_dbt-0.3.0a3/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.0a3/PKG-INFO
```

### Comparing `grai_source_dbt-0.3.0a2/pyproject.toml` & `grai_source_dbt-0.3.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt"
-version = "0.3.0-alpha2"
+version = "0.3.0-alpha3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt", from = "src" },
 ]
 readme = "README.md"
@@ -12,15 +12,15 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a7", allow-prereleases = true}
+grai-client = {version = "^0.3.0a10", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 dbt-artifacts-parser = "^0.2.4"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.991"
```

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/adapters/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/adapters/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/base.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import List, Optional, Tuple
 
-from grai_client.endpoints.client import BaseClient
 from grai_client.integrations.base import (
     CombinedNodesAndEdgesMixin,
-    GraiIntegrationImplementationV1,
+    GraiIntegrationImplementation,
 )
 from grai_schemas.base import SourcedEdge, SourcedNode
+from grai_schemas.v1.source import SourceV1
 
 from grai_source_dbt.processor import ManifestProcessor
 
 
-class DbtIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementationV1):
+class DbtIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementation):
     def __init__(
         self,
-        client: BaseClient,
-        source_name: str,
         manifest_file: str,
+        source: SourceV1,
+        version: Optional[str] = None,
         namespace: Optional[str] = "default",
     ):
-        super().__init__(client, source_name)
+        super().__init__(source, version)
 
         self.manifest_file = manifest_file
         self.namespace = namespace
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         manifest = ManifestProcessor.load(self.manifest_file, self.namespace, self.source)
         return manifest.adapted_nodes, manifest.adapted_edges
```

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v1.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/processor.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/processor.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.3.0a3/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a2/PKG-INFO` & `grai_source_dbt-0.3.0a3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.3.0a2
+Version: 0.3.0a3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbt-artifacts-parser (>=0.2.4,<0.3.0)
-Requires-Dist: grai-client (>=0.3.0a7,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt
 Description-Content-Type: text/markdown
 
 # Grai dbt Integration
```


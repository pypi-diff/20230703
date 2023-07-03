# Comparing `tmp/grai_source_dbt_cloud-0.1.0a1.tar.gz` & `tmp/grai_source_dbt_cloud-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.1.0a1.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.1.0a2.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.1.0a1.tar` & `grai_source_dbt_cloud-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a1/README.md
--rw-r--r--   0        0        0     1124 2023-06-30 11:11:10.320468 grai_source_dbt_cloud-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-30 11:11:16.371161 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0     1089 2023-06-29 12:55:58.976435 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0     4549 2023-06-06 17:35:16.800994 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a2/README.md
+-rw-r--r--   0        0        0     1125 2023-07-03 14:03:37.813368 grai_source_dbt_cloud-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-30 11:56:24.311647 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     1090 2023-07-03 13:56:25.099263 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     4549 2023-06-06 17:35:16.800994 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a2/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.1.0a1/pyproject.toml` & `grai_source_dbt_cloud-0.1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt_cloud"
-version = "0.1.0-alpha1"
+version = "0.1.0-alpha2"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt_cloud", from = "src" },
 ]
 readme = "README.md"
@@ -12,15 +12,15 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt-cloud"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a3", allow-prereleases = true}
+grai-client = {version = "^0.3.0a11", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 grai-source-dbt = {version = "^0.3.0a1", allow-prereleases = true}
 dbtc = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.0"
```

### Comparing `grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/base.py` & `grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from typing import List, Optional, Tuple
 
-from grai_client.endpoints.client import BaseClient
 from grai_client.integrations.base import (
     CombinedNodesAndEdgesMixin,
     EventMixin,
-    GraiIntegrationImplementationV1,
+    GraiIntegrationImplementation,
 )
 from grai_schemas.base import SourcedEdge, SourcedNode
+from grai_schemas.v1.source import SourceV1
 from grai_source_dbt_cloud.loader import DbtCloudConnector
 
 
-class DbtCloudIntegration(EventMixin, CombinedNodesAndEdgesMixin, GraiIntegrationImplementationV1):
+class DbtCloudIntegration(
+    CombinedNodesAndEdgesMixin, EventMixin, GraiIntegrationImplementation
+):
     def __init__(
         self,
-        client: BaseClient,
-        source_name: str,
         api_key: str,
+        source: SourceV1,
+        version: Optional[str] = None,
         namespace: Optional[str] = "default",
     ):
-        super().__init__(client, source_name)
+        super().__init__(source, version)
 
         self.connector = DbtCloudConnector(
             namespace=namespace,
             api_key=api_key,
         )
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
```

### Comparing `grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/loader.py` & `grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt_cloud-0.1.0a1/PKG-INFO` & `grai_source_dbt_cloud-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbtc (>=0.4.2,<0.5.0)
-Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a11,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: grai-source-dbt (>=0.3.0a1,<0.4.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt-cloud
 Description-Content-Type: text/markdown
```


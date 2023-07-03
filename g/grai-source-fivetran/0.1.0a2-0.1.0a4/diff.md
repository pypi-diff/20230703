# Comparing `tmp/grai_source_fivetran-0.1.0a2.tar.gz` & `tmp/grai_source_fivetran-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.1.0a2.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.1.0a4.tar", max compression
```

## Comparing `grai_source_fivetran-0.1.0a2.tar` & `grai_source_fivetran-0.1.0a4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      420 2023-05-30 08:16:23.842412 grai_source_fivetran-0.1.0a2/README.md
--rw-r--r--   0        0        0     1177 2023-06-30 11:56:33.316623 grai_source_fivetran-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      149 2023-06-30 11:56:36.571657 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     9094 2023-06-29 12:38:00.323844 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     2569 2023-06-30 13:20:02.466161 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-17 18:10:50.922218 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   451222 2023-06-06 17:35:16.808504 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    69211 2023-06-06 17:35:16.809499 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    16866 2023-06-06 17:35:16.809718 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     2173 2023-06-06 17:35:16.809859 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     5452 2023-06-06 17:35:16.809979 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.810077 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-17 18:10:50.924423 grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-30 08:16:23.842412 grai_source_fivetran-0.1.0a4/README.md
+-rw-r--r--   0        0        0     1178 2023-07-03 12:54:00.828412 grai_source_fivetran-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-07-03 12:54:04.685762 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     9094 2023-06-29 12:38:00.323844 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2417 2023-06-30 17:13:40.674956 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-17 18:10:50.922218 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   451222 2023-06-06 17:35:16.808504 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    69211 2023-06-06 17:35:16.809499 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    16866 2023-06-06 17:35:16.809718 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     2173 2023-06-06 17:35:16.809859 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     5452 2023-06-06 17:35:16.809979 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.810077 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-17 18:10:50.924423 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a4/PKG-INFO
```

### Comparing `grai_source_fivetran-0.1.0a2/pyproject.toml` & `grai_source_fivetran-0.1.0a4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
@@ -12,15 +12,15 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a7", allow-prereleases = true}
+grai-client = {version = "^0.3.0a10", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
 python-dotenv = "^0.21.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 from typing import List, Optional, Tuple
 
-from grai_client.endpoints.client import BaseClient
 from grai_client.integrations.base import (
     CombinedNodesAndEdgesMixin,
-    GraiIntegrationImplementationV1,
+    GraiIntegrationImplementation,
 )
 from grai_schemas.base import SourcedEdge, SourcedNode
-from grai_schemas.v1.source import SourceSpec
+from grai_schemas.v1.source import SourceV1
 
 from grai_source_fivetran.adapters import adapt_to_client
 from grai_source_fivetran.loader import FivetranConnector, NamespaceTypes
 
 
-class FivetranIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementationV1):
+class FivetranIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementation):
     def __init__(
         self,
-        client: Optional[BaseClient] = None,
-        source_name: Optional[str] = None,
-        source: Optional[SourceSpec] = None,
+        source: SourceV1,
+        version: Optional[str] = None,
         namespaces: Optional[NamespaceTypes] = None,
         default_namespace: Optional[str] = None,
         parallelization: int = 10,
         api_key: Optional[str] = None,
         api_secret: Optional[str] = None,
         endpoint: Optional[str] = None,
         limit: Optional[int] = None,
     ):
-        super().__init__(client, source_name, source)
+        super().__init__(source, version)
 
         self.connector = FivetranConnector(
             namespaces=namespaces,
             default_namespace=default_namespace,
             parallelization=parallelization,
             api_key=api_key,
             api_secret=api_secret,
             endpoint=endpoint,
             limit=limit,
         )
 
-    def validate_nodes_and_edges(
-        self, nodes: List[SourcedNode], edges: List[SourcedEdge]
-    ):
+    def validate_nodes_and_edges(self, nodes: List[SourcedNode], edges: List[SourcedEdge]):
         """
 
         Args:
             nodes (List[Node]):
             edges (List[Edge]):
 
         Returns:
```

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a2/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a2/PKG-INFO` & `grai_source_fivetran-0.1.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.1.0a2
+Version: 0.1.0a4
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fivetran (>=0.7.0,<0.8.0)
-Requires-Dist: grai-client (>=0.3.0a7,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran
```


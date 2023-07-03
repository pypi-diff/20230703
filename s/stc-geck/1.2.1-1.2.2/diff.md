# Comparing `tmp/stc-geck-1.2.1.tar.gz` & `tmp/stc-geck-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.2.1.tar", last modified: Mon Jul  3 18:33:32 2023, max compression
+gzip compressed data, was "stc-geck-1.2.2.tar", last modified: Mon Jul  3 18:44:53 2023, max compression
```

## Comparing `stc-geck-1.2.1.tar` & `stc-geck-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:33:32.317750 stc-geck-1.2.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:33:32.317459 stc-geck-1.2.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.2.1/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-03 18:33:11.000000 stc-geck-1.2.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-03 15:18:02.000000 stc-geck-1.2.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-03 18:33:32.317882 stc-geck-1.2.1/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:33:32.314843 stc-geck-1.2.1/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6152 2023-06-18 14:44:03.000000 stc-geck-1.2.1/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     6112 2023-07-03 18:32:19.000000 stc-geck-1.2.1/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.1/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:33:32.317092 stc-geck-1.2.1/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:44:53.117548 stc-geck-1.2.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:44:53.117309 stc-geck-1.2.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.2.2/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-03 18:44:43.000000 stc-geck-1.2.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-03 15:18:02.000000 stc-geck-1.2.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-03 18:44:53.117642 stc-geck-1.2.2/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:44:53.115074 stc-geck-1.2.2/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6140 2023-07-03 18:42:15.000000 stc-geck-1.2.2/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6106 2023-07-03 18:38:08.000000 stc-geck-1.2.2/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.2/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:44:53.116931 stc-geck-1.2.2/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.2.1/pyproject.toml` & `stc-geck-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.2.1"
+version = "1.2.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.2.1/stc_geck/cli.py` & `stc-geck-1.2.2/stc_geck/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,44 +27,44 @@
 
 
 class StcGeckCli:
     def __init__(
         self,
         ipfs_http_endpoint: str,
         ipfs_data_directory: str,
-        index_alias: str,
+        index_name: str,
         grpc_api_endpoint: str,
         embed: bool,
         timeout: int,
     ):
         self.geck = StcGeck(
             ipfs_http_base_url=ipfs_http_endpoint,
             ipfs_data_directory=ipfs_data_directory,
-            index_aliases=(index_alias,),
+            index_names=(index_name,),
             grpc_api_endpoint=grpc_api_endpoint,
             embed=embed,
         )
-        self.index_alias = index_alias
+        self.index_name = index_name
         self.timeout = timeout
 
     async def search(self, query: str, limit: int = 1):
         """
         Searches in STC using default Summa match queries.
         Examples: `doi:10.1234/abc, isbns:9781234567890, "fetal hemoglobin"`
 
         :param query: query in Summa match format
         :param limit: how many results to return, higher values incurs LARGE performance penalty.
 
         :return: metadata records
         """
-        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
+        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_name}...")
         async with self.geck as geck:
             print(f"{colored('INFO', 'green')}: Searching {query}...")
             response = await geck.get_summa_client().search([{
-                "index_alias": self.index_alias,
+                "index_alias": self.index_name,
                 "query": {
                     "match": {"value": query}
                 },
                 "collectors": [{"top_docs": {"limit": limit}}],
                 "is_fieldnorms_scoring_enabled": False,
             }])
             documents = list(map(lambda x: json.loads(x.document), response.collector_outputs[0].documents.scored_documents))
@@ -72,17 +72,17 @@
 
     async def documents(self):
         """
         Stream all STC documents.
 
         :return: metadata records
         """
-        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
+        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_name}...")
         async with self.geck as geck:
-            async for document in geck.get_summa_client().documents(self.index_alias):
+            async for document in geck.get_summa_client().documents(self.index_name):
                 print(document)
 
     async def download(self, query: str, output_path: str):
         """
         Download file from STC using default Summa match queries.
         Examples: `doi:10.1234/abc, isbns:9781234567890`
 
@@ -122,17 +122,17 @@
         name_template: str = '{id}.{extension}',
     ):
         """
         Stream all STC documents.
 
         :return: metadata records
         """
-        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
+        print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_name}...")
         async with self.geck as geck:
-            return await geck.create_ipfs_directory(self.index_alias, output_car, query, limit, name_template)
+            return await geck.create_ipfs_directory(self.index_name, output_car, query, limit, name_template)
 
 
 async def stc_geck_cli(
     ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
     ipfs_data_directory: str = '/ipns/standard-template-construct.org/data/',
     index_alias: str = 'nexus_science',
     grpc_api_endpoint: str = '127.0.0.1:37082',
```

### Comparing `stc-geck-1.2.1/stc_geck/client.py` & `stc-geck-1.2.2/stc_geck/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,22 @@
 
 
 class StcGeck(AioThing):
     def __init__(
         self,
         ipfs_http_base_url: str = 'http://localhost:8080',
         ipfs_data_directory: str = '/ipns/standard-template-construct.org/data',
-        index_aliases: Tuple[str, ...] = ('nexus_free', 'nexus_science'),
+        index_names: Tuple[str, ...] = ('nexus_science',),
         grpc_api_endpoint: str = '127.0.0.1:10082',
         embed: bool = True,
     ):
         super().__init__()
         self.ipfs_http_base_url = canonoize_base_url(ipfs_http_base_url)
         self.ipfs_data_directory = '/' + ipfs_data_directory.strip('/') + '/'
-        self.index_aliases = index_aliases
+        self.index_names = index_names
         self.grpc_api_endpoint = grpc_api_endpoint
         self.embed = embed
         self.summa_embed_server = None
         self.summa_client = SummaClient(
             endpoint=self.grpc_api_endpoint,
             max_message_length=2 * 1024 * 1024 * 1024 - 1,
         )
@@ -93,29 +93,29 @@
     async def start(self):
         self.temp_dir = tempfile.TemporaryDirectory()
         if self.embed:
             server_config = get_config()
             server_config['api']['grpc_endpoint'] = self.grpc_api_endpoint
             server_config['data_path'] = self.temp_dir.name
             server_config['log_path'] = self.temp_dir.name
-            for index in self.index_aliases:
+            for index_name in self.index_names:
                 query_parser_config = {
                     'default_fields': ['abstract', 'title']
                 }
-                full_path = self.ipfs_http_base_url + self.ipfs_data_directory + index + '/'
+                full_path = self.ipfs_http_base_url + self.ipfs_data_directory + index_name + '/'
                 headers_template = {'range': 'bytes={start}-{end}'}
                 remote_index_config = {'remote': {
                     'method': 'GET',
                     'url_template': f'{full_path}{{file_name}}',
                     'headers_template': headers_template,
                     'cache_config': {'cache_size': 536870912},
                 }}
                 if host_header := await detect_host_header(full_path):
                     headers_template['host'] = host_header
-                server_config['core']['indices'][index] = {
+                server_config['core']['indices'][index_name] = {
                     'query_parser_config': query_parser_config,
                     'config': remote_index_config,
                     'field_triggers': {},
                 }
             self.summa_embed_server = summa_embed.SummaEmbedServerBin(server_config)
             await self.summa_embed_server.start()
         await self.summa_client.start()
```

### Comparing `stc-geck-1.2.1/stc_geck/utils.py` & `stc-geck-1.2.2/stc_geck/utils.py`

 * *Files identical despite different names*


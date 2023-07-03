# Comparing `tmp/stc-geck-1.2.0.tar.gz` & `tmp/stc-geck-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.2.0.tar", last modified: Mon Jul  3 16:34:05 2023, max compression
+gzip compressed data, was "stc-geck-1.2.1.tar", last modified: Mon Jul  3 18:33:32 2023, max compression
```

## Comparing `stc-geck-1.2.0.tar` & `stc-geck-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 16:34:05.631859 stc-geck-1.2.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 16:34:05.631604 stc-geck-1.2.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.2.0/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-03 16:33:46.000000 stc-geck-1.2.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-03 15:18:02.000000 stc-geck-1.2.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-03 16:34:05.631993 stc-geck-1.2.0/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 16:34:05.629471 stc-geck-1.2.0/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6152 2023-06-18 14:44:03.000000 stc-geck-1.2.0/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     6236 2023-06-18 18:47:15.000000 stc-geck-1.2.0/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.0/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 16:34:05.631202 stc-geck-1.2.0/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-03 16:34:05.000000 stc-geck-1.2.0/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:33:32.317750 stc-geck-1.2.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:33:32.317459 stc-geck-1.2.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.2.1/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-03 18:33:11.000000 stc-geck-1.2.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-03 15:18:02.000000 stc-geck-1.2.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-03 18:33:32.317882 stc-geck-1.2.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:33:32.314843 stc-geck-1.2.1/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6152 2023-06-18 14:44:03.000000 stc-geck-1.2.1/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6112 2023-07-03 18:32:19.000000 stc-geck-1.2.1/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.1/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:33:32.317092 stc-geck-1.2.1/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-03 18:33:32.000000 stc-geck-1.2.1/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.2.0/pyproject.toml` & `stc-geck-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.2.0"
+version = "1.2.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.2.0/stc_geck/cli.py` & `stc-geck-1.2.1/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.0/stc_geck/client.py` & `stc-geck-1.2.1/stc_geck/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
                     parsed_url = urlparse(redirection_url)
                     return re.search(r'(.*)\.localhost.*', parsed_url.netloc).group(0)
 
 
 class StcGeck(AioThing):
     def __init__(
         self,
-        ipfs_http_base_url: str,
-        ipfs_data_directory: str,
-        index_aliases: Tuple[str],
-        grpc_api_endpoint: str,
+        ipfs_http_base_url: str = 'http://localhost:8080',
+        ipfs_data_directory: str = '/ipns/standard-template-construct.org/data',
+        index_aliases: Tuple[str, ...] = ('nexus_free', 'nexus_science'),
+        grpc_api_endpoint: str = '127.0.0.1:10082',
         embed: bool = True,
     ):
         super().__init__()
         self.ipfs_http_base_url = canonoize_base_url(ipfs_http_base_url)
         self.ipfs_data_directory = '/' + ipfs_data_directory.strip('/') + '/'
         self.index_aliases = index_aliases
         self.grpc_api_endpoint = grpc_api_endpoint
@@ -95,20 +95,14 @@
         if self.embed:
             server_config = get_config()
             server_config['api']['grpc_endpoint'] = self.grpc_api_endpoint
             server_config['data_path'] = self.temp_dir.name
             server_config['log_path'] = self.temp_dir.name
             for index in self.index_aliases:
                 query_parser_config = {
-                    'field_aliases': {
-                        'isbns': 'metadata.isbns',
-                        'issns': 'metadata.issns',
-                        'rd': 'references.doi',
-                        'lang': 'language',
-                    },
                     'default_fields': ['abstract', 'title']
                 }
                 full_path = self.ipfs_http_base_url + self.ipfs_data_directory + index + '/'
                 headers_template = {'range': 'bytes={start}-{end}'}
                 remote_index_config = {'remote': {
                     'method': 'GET',
                     'url_template': f'{full_path}{{file_name}}',
```

### Comparing `stc-geck-1.2.0/stc_geck/utils.py` & `stc-geck-1.2.1/stc_geck/utils.py`

 * *Files identical despite different names*


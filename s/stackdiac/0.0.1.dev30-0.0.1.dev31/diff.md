# Comparing `tmp/stackdiac-0.0.1.dev30.tar.gz` & `tmp/stackdiac-0.0.1.dev31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackdiac-0.0.1.dev30.tar", max compression
+gzip compressed data, was "stackdiac-0.0.1.dev31.tar", max compression
```

## Comparing `stackdiac-0.0.1.dev30.tar` & `stackdiac-0.0.1.dev31.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/LICENSE
--rw-r--r--   0        0        0     1415 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/README.md
--rw-r--r--   0        0        0      616 2023-06-19 07:21:04.916380 stackdiac-0.0.1.dev30/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/__init__.py
--rw-r--r--   0        0        0       23 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/api/server.py
--rw-r--r--   0        0        0     1789 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/__init__.py
--rw-r--r--   0        0        0      729 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/build.py
--rw-r--r--   0        0        0     1594 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/create.py
--rw-r--r--   0        0        0      464 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/cli/ui.py
--rw-r--r--   0        0        0      381 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/backend.py
--rw-r--r--   0        0        0     2582 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/binary.py
--rw-r--r--   0        0        0    12716 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/cluster.py
--rw-r--r--   0        0        0     2769 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/config.py
--rw-r--r--   0        0        0     2594 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/operation.py
--rw-r--r--   0        0        0      161 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/provider.py
--rw-r--r--   0        0        0     5276 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/repo.py
--rw-r--r--   0        0        0      411 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/secret.py
--rw-r--r--   0        0        0     1716 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/spec.py
--rw-r--r--   0        0        0    13166 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/models/stack.py
--rw-r--r--   0        0        0      108 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/__init__.py
--rw-r--r--   0        0        0      193 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/filters.py
--rw-r--r--   0        0        0      297 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/sdmod.py
--rw-r--r--   0        0        0    11931 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/stackd/stackd.py
--rw-r--r--   0        0        0   164360 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/ui/4753c5ba57962b4d7bf8.woff
--rw-r--r--   0        0        0   121340 2023-06-19 07:20:35.955692 stackdiac-0.0.1.dev30/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
--rw-r--r--   0        0        0  2216513 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js
--rw-r--r--   0        0        0     3087 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      415 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/ui/index.html
--rw-r--r--   0        0        0        0 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/views/__init__.py
--rw-r--r--   0        0        0      780 2023-06-19 07:20:35.971693 stackdiac-0.0.1.dev30/stackdiac/views/module.py
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev30/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/LICENSE
+-rw-r--r--   0        0        0     1415 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/README.md
+-rw-r--r--   0        0        0      616 2023-07-03 08:57:46.684435 stackdiac-0.0.1.dev31/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/api/server.py
+-rw-r--r--   0        0        0     1789 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/cli/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/cli/build.py
+-rw-r--r--   0        0        0     1594 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/cli/create.py
+-rw-r--r--   0        0        0      464 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/cli/ui.py
+-rw-r--r--   0        0        0      381 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/__init__.py
+-rw-r--r--   0        0        0     1145 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/backend.py
+-rw-r--r--   0        0        0     3222 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/binary.py
+-rw-r--r--   0        0        0    12657 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/cluster.py
+-rw-r--r--   0        0        0     3075 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/config.py
+-rw-r--r--   0        0        0     2594 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/operation.py
+-rw-r--r--   0        0        0      161 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/provider.py
+-rw-r--r--   0        0        0     5276 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/repo.py
+-rw-r--r--   0        0        0      411 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/secret.py
+-rw-r--r--   0        0        0     1716 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/spec.py
+-rw-r--r--   0        0        0    13166 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/models/stack.py
+-rw-r--r--   0        0        0      108 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/stackd/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/stackd/filters.py
+-rw-r--r--   0        0        0      297 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/stackd/sdmod.py
+-rw-r--r--   0        0        0    12032 2023-07-03 08:57:26.116067 stackdiac-0.0.1.dev31/stackdiac/stackd/stackd.py
+-rw-r--r--   0        0        0   164360 2023-07-03 08:57:26.120067 stackdiac-0.0.1.dev31/stackdiac/ui/4753c5ba57962b4d7bf8.woff
+-rw-r--r--   0        0        0   121340 2023-07-03 08:57:26.120067 stackdiac-0.0.1.dev31/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
+-rw-r--r--   0        0        0  2216513 2023-07-03 08:57:26.132067 stackdiac-0.0.1.dev31/stackdiac/ui/bundle.js
+-rw-r--r--   0        0        0     3087 2023-07-03 08:57:26.132067 stackdiac-0.0.1.dev31/stackdiac/ui/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      415 2023-07-03 08:57:26.132067 stackdiac-0.0.1.dev31/stackdiac/ui/index.html
+-rw-r--r--   0        0        0        0 2023-07-03 08:57:26.132067 stackdiac-0.0.1.dev31/stackdiac/views/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-03 08:57:26.132067 stackdiac-0.0.1.dev31/stackdiac/views/module.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev31/PKG-INFO
```

### Comparing `stackdiac-0.0.1.dev30/LICENSE` & `stackdiac-0.0.1.dev31/LICENSE`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/README.md` & `stackdiac-0.0.1.dev31/README.md`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/pyproject.toml` & `stackdiac-0.0.1.dev31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stackdiac"
-version = "0.0.1-dev30"
+version = "0.0.1-dev31"
 description = ""
 authors = ["sysr9 <38893296+sysr9@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `stackdiac-0.0.1.dev30/stackdiac/api/server.py` & `stackdiac-0.0.1.dev31/stackdiac/api/server.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/cli/__init__.py` & `stackdiac-0.0.1.dev31/stackdiac/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/cli/build.py` & `stackdiac-0.0.1.dev31/stackdiac/cli/build.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/cli/create.py` & `stackdiac-0.0.1.dev31/stackdiac/cli/create.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/backend.py` & `stackdiac-0.0.1.dev31/stackdiac/models/backend.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/binary.py` & `stackdiac-0.0.1.dev31/stackdiac/models/binary.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,16 +44,23 @@
         response = requests.get(url, stream=True)
         start_time = time.time()
 
         logger.info(f"{self} downloading from {url}")
         
         if self.extract:
             # If the binary is within a zip archive, extract it
-            zip_archive = zipfile.ZipFile(io.BytesIO(response.content))
-            binary_content = zip_archive.read(self.extract)
+            if url.endswith(".zip"):
+                zip_archive = zipfile.ZipFile(io.BytesIO(response.content))
+                binary_content = zip_archive.read(self.extract)
+            elif url.endswith(".tar.gz"):
+                import tarfile
+                tar_archive = tarfile.open(fileobj=io.BytesIO(response.content))
+                binary_content = tar_archive.extractfile(self.extract).read()
+            else:
+                raise ValueError(f"Unknown archive type for {url}")
         else:
             # If the binary is not within a zip archive, simply use the response content
             binary_content = response.content
         
         # Save the binary to a file in the `os.path.join(self.stackd.datapath, "bin")` folder
         os.makedirs(os.path.dirname(self.abspath), exist_ok=True)
         
@@ -64,13 +71,18 @@
         download_time = time.time() - start_time
         download_size = len(binary_content)
         os.chmod(self.abspath, stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH | stat.S_IXOTH)
         logger.info(f"{self} binary downloaded from {url} ({download_size} bytes) and saved to {self.abspath} in {download_time:.2f} seconds")
 
 
 class Binaries(BaseModel):
+    kustomize: Binary = Binary(binary="kustomize",
+        version = "5.1.0",        
+                url = "https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize/v{version}/kustomize_v{version}_linux_amd64.tar.gz",
+                extract="kustomize")
     terraform: Binary = Binary(binary="terraform", 
         url="https://releases.hashicorp.com/terraform/{version}/terraform_{version}_linux_amd64.zip", 
         extract="terraform", version="1.4.4")
     terragrunt: Binary = Binary(binary="terragrunt", 
         url="https://github.com/gruntwork-io/terragrunt/releases/download/v{version}/terragrunt_linux_amd64",
-        version="0.45.0")
+        version="0.45.0")
+
```

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/cluster.py` & `stackdiac-0.0.1.dev31/stackdiac/models/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 
 @api_app.get("/clusters/", operation_id="get_clusters", response_model=list[ClusterModel], tags=["cluster"])
 async def _api_get_clusters() -> list[Cluster]:    
     from stackdiac.stackd import Stackd
     sd = Stackd()
     sd.configure()
-    logger.debug(f"get_clusters: {sd.clusters['data'].dict()}")
+    
     return list(sd.clusters.values())
 
 @api_app.get("/build/{cluster_name}", operation_id="build_cluster", response_model=ClusterModel, tags=["cluster"])
 async def build_cluster(cluster_name:str) -> Cluster:
     """
     cluster.stacks will setup while bulding
     """
```

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/config.py` & `stackdiac-0.0.1.dev31/stackdiac/models/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,11 +95,17 @@
                 version="1.4.4",
             ),
             terragrunt = Binary(
                 version = "0.45.2",
                 url = "https://github.com/gruntwork-io/terragrunt/releases/download/v{version}/terragrunt_linux_amd64",
                 binary = "terragrunt",
             ),
+            kustomize = Binary(
+                version = "5.1.0",
+                binary = "kustomize",
+                url = "https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize/v{version}/kustomize_v{version}_linux_amd64.tar.gz",
+                extract="kustomize",
+            ),
         )
     )
```

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/operation.py` & `stackdiac-0.0.1.dev31/stackdiac/models/operation.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/repo.py` & `stackdiac-0.0.1.dev31/stackdiac/models/repo.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/spec.py` & `stackdiac-0.0.1.dev31/stackdiac/models/spec.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/models/stack.py` & `stackdiac-0.0.1.dev31/stackdiac/models/stack.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/stackd/stackd.py` & `stackdiac-0.0.1.dev31/stackdiac/stackd/stackd.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,21 @@
                                     token=os.environ['TF_VAR_vault_token'])
         except KeyError:
             logger.error(f"{self} vault not configured. set TF_VAR_vault_token")
             raise ProcessException("vault not configured. set TF_VAR_vault_token")
         else:
             logger.debug(f"{self} vault configured: {self.conf.vars['vault_address']}")
 
-        self.vault.secrets.kv.v2.configure(
-            max_versions=20,
-            mount_point='kv',
-        )
+        try:
+            self.vault.secrets.kv.v2.configure(
+                max_versions=20,
+                mount_point='kv',
+            )
+        except Exception as e:
+            logger.error(f"kv err: {e}")
 
         # with open(self.config_file) as f:
         #     conf_data = models.get_initial_config(name="unconfigured", domain="example.com", vault_address="http://127.0.0.1:9090").dict()
         #     initial = copy.deepcopy(conf_data)
         #     data = yaml.safe_load(f.read())
         #     conf_data = always_merger.merge(conf_data, data)
         #     self.conf = parse_obj_as(config.Config, conf_data)
```

### Comparing `stackdiac-0.0.1.dev30/stackdiac/ui/4753c5ba57962b4d7bf8.woff` & `stackdiac-0.0.1.dev31/stackdiac/ui/4753c5ba57962b4d7bf8.woff`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/ui/6d63d0501e5ed7b79dab.woff2` & `stackdiac-0.0.1.dev31/stackdiac/ui/6d63d0501e5ed7b79dab.woff2`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js` & `stackdiac-0.0.1.dev31/stackdiac/ui/bundle.js`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/ui/bundle.js.LICENSE.txt` & `stackdiac-0.0.1.dev31/stackdiac/ui/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/stackdiac/views/module.py` & `stackdiac-0.0.1.dev31/stackdiac/views/module.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev30/PKG-INFO` & `stackdiac-0.0.1.dev31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackdiac
-Version: 0.0.1.dev30
+Version: 0.0.1.dev31
 Summary: 
 License: MIT
 Author: sysr9
 Author-email: 38893296+sysr9@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


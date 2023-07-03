# Comparing `tmp/ytkubevault-0.1.2.tar.gz` & `tmp/ytkubevault-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytkubevault-0.1.2.tar", last modified: Mon Jul  4 22:04:10 2022, max compression
+gzip compressed data, was "ytkubevault-0.2.0.tar", last modified: Mon Jul  3 15:50:04 2023, max compression
```

## Comparing `ytkubevault-0.1.2.tar` & `ytkubevault-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wenrudong   (503) staff       (20)        0 2022-07-04 22:04:10.858396 ytkubevault-0.1.2/
--rw-r--r--   0 wenrudong   (503) staff       (20)     1063 2022-07-04 20:33:23.000000 ytkubevault-0.1.2/LICENSE
--rw-r--r--   0 wenrudong   (503) staff       (20)     1929 2022-07-04 22:04:10.858506 ytkubevault-0.1.2/PKG-INFO
--rw-r--r--   0 wenrudong   (503) staff       (20)     1202 2022-03-08 15:21:32.000000 ytkubevault-0.1.2/README.md
--rw-r--r--   0 wenrudong   (503) staff       (20)      106 2022-03-08 15:23:30.000000 ytkubevault-0.1.2/pyproject.toml
--rw-r--r--   0 wenrudong   (503) staff       (20)      801 2022-07-04 22:04:10.858990 ytkubevault-0.1.2/setup.cfg
-drwxr-xr-x   0 wenrudong   (503) staff       (20)        0 2022-07-04 22:04:10.857062 ytkubevault-0.1.2/ytkubevault/
--rw-r--r--   0 wenrudong   (503) staff       (20)      419 2022-07-04 22:03:38.000000 ytkubevault-0.1.2/ytkubevault/__init__.py
--rw-r--r--   0 wenrudong   (503) staff       (20)     5313 2022-07-04 22:02:49.000000 ytkubevault-0.1.2/ytkubevault/vault.py
-drwxr-xr-x   0 wenrudong   (503) staff       (20)        0 2022-07-04 22:04:10.858198 ytkubevault-0.1.2/ytkubevault.egg-info/
--rw-r--r--   0 wenrudong   (503) staff       (20)     1929 2022-07-04 22:04:10.000000 ytkubevault-0.1.2/ytkubevault.egg-info/PKG-INFO
--rw-r--r--   0 wenrudong   (503) staff       (20)      261 2022-07-04 22:04:10.000000 ytkubevault-0.1.2/ytkubevault.egg-info/SOURCES.txt
--rw-r--r--   0 wenrudong   (503) staff       (20)        1 2022-07-04 22:04:10.000000 ytkubevault-0.1.2/ytkubevault.egg-info/dependency_links.txt
--rw-r--r--   0 wenrudong   (503) staff       (20)       15 2022-07-04 22:04:10.000000 ytkubevault-0.1.2/ytkubevault.egg-info/requires.txt
--rw-r--r--   0 wenrudong   (503) staff       (20)       12 2022-07-04 22:04:10.000000 ytkubevault-0.1.2/ytkubevault.egg-info/top_level.txt
+drwxr-xr-x   0 wenrudong   (503) staff       (20)        0 2023-07-03 15:50:04.118810 ytkubevault-0.2.0/
+-rw-r--r--   0 wenrudong   (503) staff       (20)     1063 2022-07-04 20:33:23.000000 ytkubevault-0.2.0/LICENSE
+-rw-r--r--   0 wenrudong   (503) staff       (20)     3145 2023-07-03 15:50:04.118915 ytkubevault-0.2.0/PKG-INFO
+-rw-r--r--   0 wenrudong   (503) staff       (20)     2347 2023-07-03 13:21:04.000000 ytkubevault-0.2.0/README.md
+-rw-r--r--   0 wenrudong   (503) staff       (20)      106 2022-03-08 15:23:30.000000 ytkubevault-0.2.0/pyproject.toml
+-rw-r--r--   0 wenrudong   (503) staff       (20)      891 2023-07-03 15:50:04.119454 ytkubevault-0.2.0/setup.cfg
+drwxr-xr-x   0 wenrudong   (503) staff       (20)        0 2023-07-03 15:50:04.117012 ytkubevault-0.2.0/ytkubevault/
+-rw-r--r--   0 wenrudong   (503) staff       (20)      455 2023-07-03 11:47:36.000000 ytkubevault-0.2.0/ytkubevault/__init__.py
+-rw-r--r--   0 wenrudong   (503) staff       (20)    10645 2023-07-03 15:47:48.000000 ytkubevault-0.2.0/ytkubevault/vault.py
+drwxr-xr-x   0 wenrudong   (503) staff       (20)        0 2023-07-03 15:50:04.118616 ytkubevault-0.2.0/ytkubevault.egg-info/
+-rw-r--r--   0 wenrudong   (503) staff       (20)     3145 2023-07-03 15:50:04.000000 ytkubevault-0.2.0/ytkubevault.egg-info/PKG-INFO
+-rw-r--r--   0 wenrudong   (503) staff       (20)      261 2023-07-03 15:50:04.000000 ytkubevault-0.2.0/ytkubevault.egg-info/SOURCES.txt
+-rw-r--r--   0 wenrudong   (503) staff       (20)        1 2023-07-03 15:50:04.000000 ytkubevault-0.2.0/ytkubevault.egg-info/dependency_links.txt
+-rw-r--r--   0 wenrudong   (503) staff       (20)       38 2023-07-03 15:50:04.000000 ytkubevault-0.2.0/ytkubevault.egg-info/requires.txt
+-rw-r--r--   0 wenrudong   (503) staff       (20)       12 2023-07-03 15:50:04.000000 ytkubevault-0.2.0/ytkubevault.egg-info/top_level.txt
```

### Comparing `ytkubevault-0.1.2/LICENSE` & `ytkubevault-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ytkubevault-0.1.2/PKG-INFO` & `ytkubevault-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ytkubevault
-Version: 0.1.2
+Version: 0.2.0
 Summary: A convenient wrapper for getting secrets from HashiCorp Vault in Kubernetes
 Home-page: https://github.com/y-tree-limited/ytkubevault
 Author: Wenru Dong
 Author-email: wenru@y-tree.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # ytkubevault
 ytkubevault is a light wrapper of abilities to read secrets
 from HashiCorp Vault running in Kubernetes.
 
 When the microservice needs to fetch the secret value from 
@@ -52,7 +54,39 @@
 set it to be `"true"`, case-insensitive. And then,
 
 ```python
 from ytkubevault import get_secret_or_env
 
 db_password = get_secret_or_env("DATABASE_PASSWORD")
 ```
+
+Since Version 0.2.0, a `VaultClient` is added, and you can explicitly create 
+such a client:
+```python
+from ytkubevault import VaultClient
+
+vault_client = VaultClient()
+# login first
+try:
+    vault_client.login()
+except Exception as e:
+    print(f"Failed to login: {e}")
+
+# Then you can do encryption, for example:
+vault_client.encrypt(encrypt_key="some_key", plaintext="my_secret_message")
+```
+
+The old functions now use an implicitly created global `VaultClient`. Note that 
+`VaultClient` is not multithread-safe.
+
+## Fetching secrets from outside the cluster
+To be able to fetch secrets from outside the Kubernetes cluster, you need to install 
+the package with
+```shell
+pip install 'ytkubevault[dev]'
+```
+This will also install `kubernetes` package, which allows us to get the service account
+token. Additionally, 4 environment variables need to be set:
+* VAULT_DEV_REMOTE_MODE: this needs to be `true`, which is `false` by default
+* VAULT_DEV_REMOTE_CLUSTER: the cluster string you want to connect to
+* VAULT_DEV_REMOTE_NAMESPACE: the namespace the service is in
+* VAULT_DEV_REMOTE_SERVICE_ACCOUNT: the service account name of the service
```

### Comparing `ytkubevault-0.1.2/setup.cfg` & `ytkubevault-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 license = MIT License
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Intended Audience :: Developers
 	Topic :: Utilities
 url = https://github.com/y-tree-limited/ytkubevault
 
 [options]
 packages = ytkubevault
 python_requires = >=3.8
 install_requires = 
-	hvac >= "0.11.2"
+	hvac >= 1.0.0
+
+[options.extras_require]
+dev = 
+	kubernetes>=26.1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ytkubevault-0.1.2/ytkubevault.egg-info/PKG-INFO` & `ytkubevault-0.2.0/ytkubevault.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ytkubevault
-Version: 0.1.2
+Version: 0.2.0
 Summary: A convenient wrapper for getting secrets from HashiCorp Vault in Kubernetes
 Home-page: https://github.com/y-tree-limited/ytkubevault
 Author: Wenru Dong
 Author-email: wenru@y-tree.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # ytkubevault
 ytkubevault is a light wrapper of abilities to read secrets
 from HashiCorp Vault running in Kubernetes.
 
 When the microservice needs to fetch the secret value from 
@@ -52,7 +54,39 @@
 set it to be `"true"`, case-insensitive. And then,
 
 ```python
 from ytkubevault import get_secret_or_env
 
 db_password = get_secret_or_env("DATABASE_PASSWORD")
 ```
+
+Since Version 0.2.0, a `VaultClient` is added, and you can explicitly create 
+such a client:
+```python
+from ytkubevault import VaultClient
+
+vault_client = VaultClient()
+# login first
+try:
+    vault_client.login()
+except Exception as e:
+    print(f"Failed to login: {e}")
+
+# Then you can do encryption, for example:
+vault_client.encrypt(encrypt_key="some_key", plaintext="my_secret_message")
+```
+
+The old functions now use an implicitly created global `VaultClient`. Note that 
+`VaultClient` is not multithread-safe.
+
+## Fetching secrets from outside the cluster
+To be able to fetch secrets from outside the Kubernetes cluster, you need to install 
+the package with
+```shell
+pip install 'ytkubevault[dev]'
+```
+This will also install `kubernetes` package, which allows us to get the service account
+token. Additionally, 4 environment variables need to be set:
+* VAULT_DEV_REMOTE_MODE: this needs to be `true`, which is `false` by default
+* VAULT_DEV_REMOTE_CLUSTER: the cluster string you want to connect to
+* VAULT_DEV_REMOTE_NAMESPACE: the namespace the service is in
+* VAULT_DEV_REMOTE_SERVICE_ACCOUNT: the service account name of the service
```


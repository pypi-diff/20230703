# Comparing `tmp/py_sec_vault-0.1.5.tar.gz` & `tmp/py_sec_vault-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.1.5.tar", max compression
+gzip compressed data, was "py_sec_vault-0.1.6.tar", max compression
```

## Comparing `py_sec_vault-0.1.5.tar` & `py_sec_vault-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.5/LICENSE
--rw-r--r--   0        0        0     3347 2023-06-30 08:34:41.532823 py_sec_vault-0.1.5/README.md
--rw-r--r--   0        0        0      916 2023-06-30 08:28:08.979442 py_sec_vault-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      190 2023-06-30 08:25:36.575393 py_sec_vault-0.1.5/vault/__init__.py
--rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.5/vault/client.py
--rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.5/vault/config.py
--rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.5/vault/exceptions.py
--rw-r--r--   0        0        0     1851 2023-06-30 08:32:06.011213 py_sec_vault-0.1.5/vault/utils.py
--rw-r--r--   0        0        0     3609 2023-06-30 08:12:09.227387 py_sec_vault-0.1.5/vault/vault.py
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 py_sec_vault-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3347 2023-06-30 08:34:41.532823 py_sec_vault-0.1.6/README.md
+-rw-r--r--   0        0        0      920 2023-07-03 18:48:18.329146 py_sec_vault-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-06-30 08:25:36.575393 py_sec_vault-0.1.6/vault/__init__.py
+-rw-r--r--   0        0        0     2643 2023-07-03 19:00:05.413181 py_sec_vault-0.1.6/vault/client.py
+-rw-r--r--   0        0        0      433 2023-07-03 19:00:52.195085 py_sec_vault-0.1.6/vault/config.py
+-rw-r--r--   0        0        0      784 2023-07-03 18:25:44.942964 py_sec_vault-0.1.6/vault/exceptions.py
+-rw-r--r--   0        0        0     1851 2023-06-30 08:32:06.011213 py_sec_vault-0.1.6/vault/utils.py
+-rw-r--r--   0        0        0     3075 2023-07-03 18:59:35.787434 py_sec_vault-0.1.6/vault/vault.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 py_sec_vault-0.1.6/PKG-INFO
```

### Comparing `py_sec_vault-0.1.5/LICENSE` & `py_sec_vault-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.5/README.md` & `py_sec_vault-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.5/pyproject.toml` & `py_sec_vault-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-sec-vault"
-version = "0.1.5"
+version = "0.1.6"
 description = "Vault implementation in python software (Hashicorp)"
 authors = ["CISolutions B.V. <info@cisolutions.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vault"}]
 homepage = "https://github.com/cisolutions-nl/py-sec-vault"
 repository = "https://github.com/cisolutions-nl/py-sec-vault"
@@ -19,15 +19,15 @@
 include = [
     "LICENSE",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-hvac = "^1.1.0"
+requests = "2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `py_sec_vault-0.1.5/vault/utils.py` & `py_sec_vault-0.1.6/vault/utils.py`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.5/vault/vault.py` & `py_sec_vault-0.1.6/vault/vault.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import logging
 from functools import lru_cache
-from typing import Mapping, Optional, Tuple
-
-from hvac import Client
-from hvac.exceptions import InvalidPath, Forbidden
+from typing import Mapping, Optional, Tuple, Union
 
 from . import config
-from .client import get_client
+from .client import get_client, TokenClient, AppRoleClient
 from .exceptions import VaultClientImproperlyConfiguredError
 
 logger = logging.getLogger(__name__)
 
 
 def _validate_vault_config(
     auth_method: str,
@@ -34,15 +31,15 @@
             )
         return True
     raise VaultClientImproperlyConfiguredError("Missing variable VAULT_AUTH_METHOD.")
 
 
 class Vault:
     _variables: Mapping[str, str] = dict()
-    _client: Optional[Client] = None
+    _client: Optional[Union[TokenClient, AppRoleClient]] = None
 
     def __init__(
         self,
         host: str = config.VAULT_HOST,
         engine_name: str = config.VAULT_ENGINE_NAME,
         path: str = config.VAULT_PATH,
         auth_method: str = config.VAULT_AUTH_METHOD,
@@ -58,19 +55,18 @@
                 secret_id=secret_id,
             )
         except VaultClientImproperlyConfiguredError as e:
             logger.exception(e, exc_info=True)
             return
 
         self._client = get_client(
-            auth_method=auth_method,
             host=host,
-            token=token,
             role_id=role_id,
             secret_id=secret_id,
+            token=token,
         )
         if not self._client:
             raise ConnectionError(
                 "Could not connect to vault. Check your vault configuration."
             )
 
         logger.debug(f"Connected to vault with auth method {auth_method}.")
@@ -80,30 +76,15 @@
         )
 
     def __getitem__(self, key: str) -> Optional[str]:
         return self._variables[key]
 
     @lru_cache
     def _fetch_variables(self, engine_name: str, vault_path: str) -> Mapping[str, str]:
-        try:
-            response = self._client.secrets.kv.v2.read_secret(
-                mount_point=engine_name,
-                path=vault_path,
-            )
-        except InvalidPath:
-            raise Exception(
-                f"Your path ({vault_path}) has not been created yet "
-                f"or there are no credentials in it."
-            )
-        except Forbidden:
-            raise Exception(
-                f"Your client does not have access to the path '{vault_path}'."
-            )
-
-        variables = response["data"]["data"]
+        variables = self._client.read_secrets(engine_name, vault_path)
         logger.info(f"Fetched {len(variables.keys())} secret(s) from vault.")
         return variables
 
     def get(self, key: str, default: str = None) -> Optional[str]:
         try:
             return self[key]
         except KeyError:
```

### Comparing `py_sec_vault-0.1.5/PKG-INFO` & `py_sec_vault-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sec-vault
-Version: 0.1.5
+Version: 0.1.6
 Summary: Vault implementation in python software (Hashicorp)
 Home-page: https://github.com/cisolutions-nl/py-sec-vault
 License: MIT
 Keywords: vault,hashicorp,security
 Author: CISolutions B.V.
 Author-email: info@cisolutions.nl
 Requires-Python: >=3.9
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: hvac (>=1.1.0,<2.0.0)
+Requires-Dist: requests (==2.31.0)
 Project-URL: Repository, https://github.com/cisolutions-nl/py-sec-vault
 Description-Content-Type: text/markdown
 
 # PySecVault
 Hashicorp Vault implementation in python software
```


# Comparing `tmp/nsj_flask_auth-0.4.0.tar.gz` & `tmp/nsj_flask_auth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_flask_auth-0.4.0.tar", max compression
+gzip compressed data, was "nsj_flask_auth-0.5.0.tar", max compression
```

## Comparing `nsj_flask_auth-0.4.0.tar` & `nsj_flask_auth-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       72 2022-12-28 20:58:19.637881 nsj_flask_auth-0.4.0/nsj_flask_auth/__init__.py
--rw-r--r--   0        0        0    16733 2022-12-28 21:28:46.019668 nsj_flask_auth-0.4.0/nsj_flask_auth/auth.py
--rw-r--r--   0        0        0      430 2022-12-19 17:34:11.665863 nsj_flask_auth-0.4.0/nsj_flask_auth/caching.py
--rw-r--r--   0        0        0      135 2022-12-28 21:04:57.577516 nsj_flask_auth-0.4.0/nsj_flask_auth/exceptions.py
--rw-r--r--   0        0        0      521 2022-12-28 21:33:20.640802 nsj_flask_auth-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 nsj_flask_auth-0.4.0/setup.py
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 nsj_flask_auth-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/__init__.py
+-rw-r--r--   0        0        0    16982 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/auth.py
+-rw-r--r--   0        0        0      430 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/caching.py
+-rw-r--r--   0        0        0      135 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/exceptions.py
+-rw-r--r--   0        0        0      601 2023-07-03 15:18:00.717279 nsj_flask_auth-0.5.0/nsj_flask_auth/settings.py
+-rw-r--r--   0        0        0      521 2023-07-03 15:18:25.925167 nsj_flask_auth-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 nsj_flask_auth-0.5.0/PKG-INFO
```

### Comparing `nsj_flask_auth-0.4.0/nsj_flask_auth/auth.py` & `nsj_flask_auth-0.5.0/nsj_flask_auth/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from functools import wraps
 from urllib.parse import urljoin
 
 from flask import request, abort, jsonify, g
 
 from nsj_flask_auth.caching import Caching
 from nsj_flask_auth.exceptions import Forbidden, MissingAuthorizationHeader, Unauthorized
+from nsj_flask_auth.settings import log_time
 
 
 class Scope(Enum):
     TENANT = 0
     GRUPO_EMPRESARIAL = 1
     EMPRESA = 2
     ESTABELECIMENTO = 3
@@ -140,14 +141,15 @@
             self._verify_permission_by_scope(
                 self._user_scope_permissions, email, scope=self._scope
             )
             return
 
         return
 
+    @log_time('Pegar profile do diretório')
     def _get_user_profile_diretorio(self, email):
         user_profile = None
 
         if self._cache:
             user_profile = self._cache.get(email)
 
         if not user_profile:
@@ -273,14 +275,15 @@
         except MissingAuthorizationHeader:
             pass
 
         self._verify_access_token(
             user_internal_permissions, scope, user_scope_permissions
         )
 
+    @log_time('Pegar profile a partir do access token')
     def _get_user_profile(self, access_token):
 
         if self._cache:
             user_profile = self._cache.get(access_token)
             if user_profile:
                 return user_profile
 
@@ -293,15 +296,16 @@
         if response.status_code != 200:
             raise Unauthorized("O token do usuário não é válido")
 
         if self._cache:
             self._cache.set(access_token, response.json())
 
         return response.json()
-
+    
+    @log_time('Pegar profile a partir da apikey')
     def _get_app_profile(self, api_key):
 
         if self._cache:
             app_profile = self._cache.get(api_key)
             if app_profile:
                 return app_profile
 
@@ -320,14 +324,15 @@
             raise Unauthorized("A api-key do sistema não é válida")
 
         if self._cache:
             self._cache.set(api_key, response.json())
 
         return response.json()
 
+    @log_time('Pegar permissões por funções')
     def _get_permissions_by_function(self, function_id):
 
         permissions = None
 
         if self._cache:
             permissions = self._cache.get(function_id)
             if permissions:
```

### Comparing `nsj_flask_auth-0.4.0/pyproject.toml` & `nsj_flask_auth-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsj-flask-auth"
-version = "0.4.0"
+version = "0.5.0"
 description = "Modulo básico para autenticação de aplicações Flask no contexto da Nasajon"
 authors = ["Lucas Assis <lucasassis@nasajon.com.br>", "Sergio Silva <sergiosilva@nasajon.com.br>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Flask = "*"
 requests = "*"
```

### Comparing `nsj_flask_auth-0.4.0/PKG-INFO` & `nsj_flask_auth-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-flask-auth
-Version: 0.4.0
+Version: 0.5.0
 Summary: Modulo básico para autenticação de aplicações Flask no contexto da Nasajon
 Author: Lucas Assis
 Author-email: lucasassis@nasajon.com.br
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


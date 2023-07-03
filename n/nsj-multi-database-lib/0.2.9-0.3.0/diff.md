# Comparing `tmp/nsj_multi_database_lib-0.2.9.tar.gz` & `tmp/nsj_multi_database_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_multi_database_lib-0.2.9.tar", max compression
+gzip compressed data, was "nsj_multi_database_lib-0.3.0.tar", max compression
```

## Comparing `nsj_multi_database_lib-0.2.9.tar` & `nsj_multi_database_lib-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       74 2023-03-20 17:20:24.769414 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/__init__.py
--rw-r--r--   0        0        0      288 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/crypt_key_sample.py
--rw-r--r--   0        0        0      268 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/crypt_util.py
--rw-r--r--   0        0        0        0 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dao/__init__.py
--rw-r--r--   0        0        0     1891 2023-04-05 18:59:17.463320 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dao/database.py
--rw-r--r--   0        0        0      746 2023-03-20 15:23:18.477000 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dao/usuario.py
--rw-r--r--   0        0        0     1815 2023-04-04 13:38:20.905178 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/db_pool_config.py
--rw-r--r--   0        0        0        0 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/decorator/__init__.py
--rw-r--r--   0        0        0     3187 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/decorator/multi_database.py
--rw-r--r--   0        0        0        0 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dto/__init__.py
--rw-r--r--   0        0        0     1536 2023-03-20 15:23:28.959000 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dto/database.py
--rw-r--r--   0        0        0        0 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/entity/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/entity/database.py
--rw-r--r--   0        0        0      892 2023-04-04 13:38:20.905178 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/env_config.py
--rw-r--r--   0        0        0       45 2023-04-04 13:38:18.605144 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/exception.py
--rw-r--r--   0        0        0     1837 2023-03-20 17:41:38.321573 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/injector_factory.py
--rw-r--r--   0        0        0      447 2023-04-05 18:58:22.270978 nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/settings.py
--rw-r--r--   0        0        0      574 2023-04-05 18:59:52.271534 nsj_multi_database_lib-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 nsj_multi_database_lib-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/crypt_key_sample.py
+-rw-r--r--   0        0        0      268 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/crypt_util.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dao/__init__.py
+-rw-r--r--   0        0        0     1989 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dao/database.py
+-rw-r--r--   0        0        0      838 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dao/usuario.py
+-rw-r--r--   0        0        0     1815 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/db_pool_config.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/decorator/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/decorator/multi_database.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dto/__init__.py
+-rw-r--r--   0        0        0     1536 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dto/database.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/entity/__init__.py
+-rw-r--r--   0        0        0     1036 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/entity/database.py
+-rw-r--r--   0        0        0      930 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/env_config.py
+-rw-r--r--   0        0        0       45 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/exception.py
+-rw-r--r--   0        0        0     1837 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/injector_factory.py
+-rw-r--r--   0        0        0      913 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/settings.py
+-rw-r--r--   0        0        0      592 2023-07-03 15:15:17.733994 nsj_multi_database_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 nsj_multi_database_lib-0.3.0/PKG-INFO
```

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dao/database.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dao/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 from nsj_rest_lib.dao.dao_base import DAOBase
 from nsj_gcf_utils.db_adapter2 import DBAdapter2
 from nsj_rest_lib.entity.entity_base import EntityBase
 from nsj_rest_lib.exception import NotFoundException
 
 from nsj_multi_database_lib.crypt_util import decrypt
+from nsj_multi_database_lib.settings import log_time
 
 
 class DatabaseDAO(DAOBase):
     def __init__(self, db: DBAdapter2, entity_class: EntityBase):
         super().__init__(db, entity_class)
     
+    @log_time('Coletar banco ERP do tenant')
     def get_by_tenant(self, tenant):
         sql = """
             select host, porta, nome, "user", password
             from multibanco.database
             where tenant = :tenant;
         """
```

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dao/usuario.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dao/usuario.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from nsj_rest_lib.dao.dao_base import DAOBase
 from nsj_gcf_utils.db_adapter2 import DBAdapter2
 from nsj_rest_lib.entity.entity_base import EntityBase
 from nsj_rest_lib.exception import NotFoundException
+from nsj_multi_database_lib.settings import log_time
 
 
 class UsuarioDAO():
     def __init__(self, db: DBAdapter2):
         self._db = db
-    
+
+    @log_time('Coletar senha do usuário')
     def get_by_email(self, email):
         sql = """
             select login, senha
             from ns.usuarios
             where email ilike :email;
         """
```

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/db_pool_config.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/dto/database.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/dto/database.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/entity/database.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/entity/database.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/env_config.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/env_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
     def __init__(self):
         self.multi_database_host = os.getenv("MULTI_DATABASE_HOST", "localhost")
         self.multi_database_name = os.getenv("MULTI_DATABASE_NAME", "multibanco")
         self.multi_database_user = os.getenv("MULTI_DATABASE_USER", "multibanco")
         self.multi_database_password = os.getenv("MULTI_DATABASE_PASS", "mysecretpassword")
         self.multi_database_port = os.getenv("MULTI_DATABASE_PORT", "5432")
-        self.default_external_database_user = os.getenv("DEFAULT_EXTERNAL_DATABASE_USER", "nsj_integratto_admin")
-        self.default_external_database_password = os.getenv("DEFAULT_EXTERNAL_DATABASE_PASSWORD", "temp%24P4ssw0rd46281937%24")
+        self.default_external_database_user = os.getenv("DEFAULT_EXTERNAL_DATABASE_USER", "nsj_integratto_admin").replace('@','%40')
+        self.default_external_database_password = os.getenv("DEFAULT_EXTERNAL_DATABASE_PASSWORD", "temp%24P4ssw0rd46281937%24").replace('@','%40')
 
     @staticmethod
     def instance():
         if (EnvConfig._instance == None):
             EnvConfig._instance = EnvConfig()
 
         return EnvConfig._instance
```

### Comparing `nsj_multi_database_lib-0.2.9/nsj_multi_database_lib/injector_factory.py` & `nsj_multi_database_lib-0.3.0/nsj_multi_database_lib/injector_factory.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.2.9/pyproject.toml` & `nsj_multi_database_lib-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "nsj-multi-database-lib"
-version = "0.2.9"
+version = "0.3.0"
 description = "Modulo que permite o uso de múltiplos bancos de dados na mesma aplicação."
 authors = ["Wallace Pinho <wallacepinho@nasajon.com.br>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Flask = "*"
-nsj_rest_lib = "^0.1.6"
-nsj_flask_auth = "^0.3.0"
+nsj_rest_lib = ">=0.1.6, <2.0.0"
+nsj_flask_auth = ">=0.3.0, <1.0.0"
 nsj_gcf_utils = "^1.0.9"
 SQLAlchemy = "^1.4.32"
 pg8000 = "^1.24.1"
 cryptography = "40.0.1"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.14.4"
```

### Comparing `nsj_multi_database_lib-0.2.9/PKG-INFO` & `nsj_multi_database_lib-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nsj-multi-database-lib
-Version: 0.2.9
+Version: 0.3.0
 Summary: Modulo que permite o uso de múltiplos bancos de dados na mesma aplicação.
 Author: Wallace Pinho
 Author-email: wallacepinho@nasajon.com.br
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0)
 Requires-Dist: cryptography (==40.0.1)
-Requires-Dist: nsj_flask_auth (>=0.3.0,<0.4.0)
+Requires-Dist: nsj_flask_auth (>=0.3.0,<1.0.0)
 Requires-Dist: nsj_gcf_utils (>=1.0.9,<2.0.0)
-Requires-Dist: nsj_rest_lib (>=0.1.6,<0.2.0)
+Requires-Dist: nsj_rest_lib (>=0.1.6,<2.0.0)
 Requires-Dist: pg8000 (>=1.24.1,<2.0.0)
```


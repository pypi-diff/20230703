# Comparing `tmp/starlite_users-0.7.1.tar.gz` & `tmp/starlite_users-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlite_users-0.7.1.tar", max compression
+gzip compressed data, was "starlite_users-0.8.0.tar", max compression
```

## Comparing `starlite_users-0.7.1.tar` & `starlite_users-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-06-09 08:27:17.411144 starlite_users-0.7.1/LICENSE
--rw-r--r--   0        0        0      809 2023-06-09 08:27:17.411144 starlite_users-0.7.1/README.md
--rw-r--r--   0        0        0     4317 2023-06-09 08:27:17.411144 starlite_users-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/__init__.py
--rw-r--r--   0        0        0     1522 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/guid.py
--rw-r--r--   0        0        0     1517 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/mixins.py
--rw-r--r--   0        0        0     8141 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/repository.py
--rw-r--r--   0        0        0    13032 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/config.py
--rw-r--r--   0        0        0     2660 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/dependencies.py
--rw-r--r--   0        0        0     2830 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/exceptions.py
--rw-r--r--   0        0        0     5046 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/generics.py
--rw-r--r--   0        0        0     1485 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/guards.py
--rw-r--r--   0        0        0     6734 2023-06-09 08:27:17.411144 starlite_users-0.7.1/starlite_users/main.py
--rw-r--r--   0        0        0     1350 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/password.py
--rw-r--r--   0        0        0    14243 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/route_handlers.py
--rw-r--r--   0        0        0     2356 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/schema.py
--rw-r--r--   0        0        0    15754 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/service.py
--rw-r--r--   0        0        0     3354 2023-06-09 08:27:17.415145 starlite_users-0.7.1/starlite_users/user_handlers.py
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 starlite_users-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-03 09:19:53.524420 starlite_users-0.8.0/LICENSE
+-rw-r--r--   0        0        0      809 2023-07-03 09:19:53.524420 starlite_users-0.8.0/README.md
+-rw-r--r--   0        0        0     4317 2023-07-03 09:19:53.528420 starlite_users-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/__init__.py
+-rw-r--r--   0        0        0     1522 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/adapter/sqlalchemy/guid.py
+-rw-r--r--   0        0        0     1517 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/adapter/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0     8141 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/adapter/sqlalchemy/repository.py
+-rw-r--r--   0        0        0    13099 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/config.py
+-rw-r--r--   0        0        0     2660 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/dependencies.py
+-rw-r--r--   0        0        0     2830 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/exceptions.py
+-rw-r--r--   0        0        0     5046 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/generics.py
+-rw-r--r--   0        0        0     1485 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/guards.py
+-rw-r--r--   0        0        0     6734 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/main.py
+-rw-r--r--   0        0        0     1350 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/password.py
+-rw-r--r--   0        0        0    14243 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/route_handlers.py
+-rw-r--r--   0        0        0     2356 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/schema.py
+-rw-r--r--   0        0        0    15754 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/service.py
+-rw-r--r--   0        0        0     3876 2023-07-03 09:19:53.528420 starlite_users-0.8.0/starlite_users/user_handlers.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 starlite_users-0.8.0/PKG-INFO
```

### Comparing `starlite_users-0.7.1/LICENSE` & `starlite_users-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/README.md` & `starlite_users-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/pyproject.toml` & `starlite_users-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starlite-users"
-version = "0.7.1"
+version = "0.8.0"
 description = "Authentication and user management for Starlite"
 authors = ["Michael Bosch <michael@lonelyviking.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "starlite_users"}]
 
 [tool.poetry.dependencies]
```

### Comparing `starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/guid.py` & `starlite_users-0.8.0/starlite_users/adapter/sqlalchemy/guid.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/mixins.py` & `starlite_users-0.8.0/starlite_users/adapter/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/adapter/sqlalchemy/repository.py` & `starlite_users-0.8.0/starlite_users/adapter/sqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/config.py` & `starlite_users-0.8.0/starlite_users/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,35 +292,35 @@
 
     @property
     def auth_config(self) -> JWTAuth | JWTCookieAuth | SessionAuth:
         return self._auth_config or self._get_auth_config()
 
     def _get_auth_config(self) -> JWTAuth | JWTCookieAuth | SessionAuth:
         if self.auth_backend == "session":
-            return SessionAuth(
+            return SessionAuth(  # pyright: ignore
                 retrieve_user_handler=get_session_retrieve_user_handler(
                     user_model=self.user_model,
                     role_model=self.role_model,
                     user_repository_class=self.user_repository_class,
                 ),
-                session_backend_config=self.session_backend_config,  # type: ignore
+                session_backend_config=self.session_backend_config,  # type: ignore[arg-type]
                 exclude=self.auth_exclude_paths,
             )
         if self.auth_backend == "jwt":
-            return JWTAuth(
+            return JWTAuth(  # pyright: ignore
                 retrieve_user_handler=get_jwt_retrieve_user_handler(
                     user_model=self.user_model,
                     role_model=self.role_model,
                     user_repository_class=self.user_repository_class,
                 ),
                 token_secret=self.secret.get_secret_value(),
                 exclude=self.auth_exclude_paths,
             )
 
-        return JWTCookieAuth(
+        return JWTCookieAuth(  # pyright: ignore
             retrieve_user_handler=get_jwt_retrieve_user_handler(
                 user_model=self.user_model,
                 role_model=self.role_model,
                 user_repository_class=self.user_repository_class,
             ),
             token_secret=self.secret.get_secret_value(),
             exclude=self.auth_exclude_paths,
```

### Comparing `starlite_users-0.7.1/starlite_users/dependencies.py` & `starlite_users-0.8.0/starlite_users/dependencies.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/exceptions.py` & `starlite_users-0.8.0/starlite_users/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/generics.py` & `starlite_users-0.8.0/starlite_users/generics.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/guards.py` & `starlite_users-0.8.0/starlite_users/guards.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/main.py` & `starlite_users-0.8.0/starlite_users/main.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/password.py` & `starlite_users-0.8.0/starlite_users/password.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/route_handlers.py` & `starlite_users-0.8.0/starlite_users/route_handlers.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/schema.py` & `starlite_users-0.8.0/starlite_users/schema.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/service.py` & `starlite_users-0.8.0/starlite_users/service.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.7.1/starlite_users/user_handlers.py` & `starlite_users-0.8.0/starlite_users/user_handlers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable
 
+from starlite.exceptions import ImproperlyConfiguredException
+from starlite.plugins.sql_alchemy.plugin import SQLAlchemyPlugin
+
 from starlite_users.exceptions import RepositoryNotFoundException
 
 __all__ = ["get_jwt_retrieve_user_handler", "get_session_retrieve_user_handler"]
 
 
 if TYPE_CHECKING:
     from starlite import ASGIConnection
@@ -33,25 +36,31 @@
     ) -> UserModelType | None:
         """Get a user from the database based on session info.
 
         Args:
             session: Starlite session.
             connection: The ASGI connection.
         """
-        async_session_maker = connection.app.state.session_maker_class
-
-        async with async_session_maker() as async_session:
-            async with async_session.begin():
-                repository = user_repository_class(session=async_session, user_model=user_model, role_model=role_model)
-                try:
-                    user = await repository.get_user(session.get("user_id", ""))
-                    if user.is_active and user.is_verified:
-                        return user  # type: ignore[no-any-return]
-                except RepositoryNotFoundException:
-                    pass
+        db_config = None
+        for plugin in connection.app.plugins:
+            if isinstance(plugin, SQLAlchemyPlugin):
+                db_config = plugin._config
+                break
+        if db_config is None:
+            raise ImproperlyConfiguredException("sqlalchemy plugin is not registered")
+
+        async_session = db_config.create_db_session_dependency(state=connection.app.state, scope=connection.scope)
+
+        repository = user_repository_class(session=async_session, user_model=user_model, role_model=role_model)
+        try:
+            user = await repository.get_user(session.get("user_id", ""))
+            if user.is_active and user.is_verified:
+                return user  # type: ignore[no-any-return]
+        except RepositoryNotFoundException:
+            return None
         return None
 
     return retrieve_user_handler
 
 
 def get_jwt_retrieve_user_handler(
     user_model: type[UserModelType],
@@ -69,21 +78,27 @@
     async def retrieve_user_handler(token: Token, connection: ASGIConnection[Any, Any, Any]) -> user_model | None:  # type: ignore[valid-type]
         """Get a user from the database based on JWT info.
 
         Args:
             token: Encoded JWT.
             connection: The ASGI connection.
         """
-        async_session_maker = connection.app.state.session_maker_class
-
-        async with async_session_maker() as async_session:
-            async with async_session.begin():
-                repository = user_repository_class(session=async_session, user_model=user_model, role_model=role_model)
-                try:
-                    user = await repository.get_user(token.sub)
-                    if user.is_active and user.is_verified:
-                        return user  # type: ignore[no-any-return]
-                except RepositoryNotFoundException:
-                    pass
+        db_config = None
+        for plugin in connection.app.plugins:
+            if isinstance(plugin, SQLAlchemyPlugin):
+                db_config = plugin._config
+                break
+        if db_config is None:
+            raise ImproperlyConfiguredException("sqlalchemy plugin is not registered")
+
+        async_session = db_config.create_db_session_dependency(state=connection.app.state, scope=connection.scope)
+
+        repository = user_repository_class(session=async_session, user_model=user_model, role_model=role_model)
+        try:
+            user = await repository.get_user(token.sub)
+            if user.is_active and user.is_verified:
+                return user  # type: ignore[no-any-return]
+        except RepositoryNotFoundException:
+            return None
         return None
 
     return retrieve_user_handler
```

### Comparing `starlite_users-0.7.1/PKG-INFO` & `starlite_users-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlite-users
-Version: 0.7.1
+Version: 0.8.0
 Summary: Authentication and user management for Starlite
 License: MIT
 Author: Michael Bosch
 Author-email: michael@lonelyviking.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

